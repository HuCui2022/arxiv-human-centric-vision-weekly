---
name: arxiv-human-centric-weekly
description: Generate the recurring Chinese weekly digest of newly submitted arXiv cs.CV papers about human-centric vision and lighting, then optionally commit it locally without pushing. Use for this project's weekly Tuesday paper collection or equivalent requests to update the human-centric arXiv digest.
---

# ArXiv Human-Centric Vision Weekly

Create this project's weekly Chinese literature digest from the official arXiv `cs.CV` listings.

## Date window

- Unless the user supplies dates, use the complete previous Monday through Sunday in `Asia/Shanghai` relative to the current date.
- State the resolved inclusive dates before retrieval.
- Treat a paper's first arXiv submission timestamp as its publication date for this digest. Exclude records outside the resolved window even if an API query returns them.

## Scope

Include papers whose main contribution is directly relevant to one or more of:

- action/activity recognition, understanding, detection, anticipation, or anomaly detection;
- gestures, hand gestures, sign-language recognition, translation, generation, or datasets;
- human or hand pose estimation, tracking, motion capture, motion understanding, prediction, editing, or generation;
- human-centric foundation models, human-human interaction, human-object interaction, or egocentric human action understanding;
- 3D/4D human reconstruction, human body/mesh modeling, animatable avatars, or digital humans;
- illumination/lighting estimation, color constancy, relighting, or closely related lighting modeling.

Exclude incidental keyword matches, including camera/object pose estimation, generic point-cloud registration, robotics actions without a human-centric vision contribution, and papers that only cite an in-scope task as background.

## Retrieval and verification

- Prefer the official arXiv API and `https://arxiv.org/list/cs.CV/recent`; paginate until the full date window is covered.
- Search titles and abstracts broadly, then read each candidate's complete metadata before deciding relevance.
- Do not rely on search-engine snippets when official arXiv metadata is available.
- For open-source status, mark `★` only when the arXiv page, abstract, comments, or linked project explicitly provides a currently public source-code repository. A project page, demo, dataset-only release, or promise to release later is insufficient.
- Do not ask the user to approve ordinary arXiv reads. If the execution environment itself requires a network permission dialog, request only the minimum required permission and continue after approval.

## Output

Write one Markdown file in the project root named:

`arxiv_csCV_human_centric_YYYY-MM-DD_to_YYYY-MM-DD.md`

Use this structure:

1. Title containing the inclusive date range.
2. Source, date interpretation, selection scope, and `★` legend.
3. Overview table with submission date, topic, Chinese title, arXiv abstract-page link, and `★` where applicable.
4. Numbered paper details containing:
   - Chinese translated title;
   - original English title;
   - authors;
   - topic tags;
   - clickable `https://arxiv.org/abs/<id>` link;
   - faithful, fluent Chinese translation of the complete abstract.
5. Selection notes, including whether no direct illumination-estimation paper was found and which nearby lighting work was included.

Preserve technical names, dataset names, model names, metrics, and numerical results. Translate meaning rather than adding unsupported interpretation. Perform a final check for date leakage, duplicate papers, malformed links, mistranslations, and inconsistent stars.

## Git boundary

After writing and verifying the digest:

- Check the working tree and preserve unrelated user changes.
- Add only the new or intentionally updated digest and directly related project documentation or skill files.
- Create a local commit with a concise message such as `Add human-centric CV arXiv digest for YYYY-MM-DD to YYYY-MM-DD` when the user asks for the standard weekly workflow.
- Run a normal `git push` only when the current user request or the active automation explicitly requires it. Never force-push, create a remote repository, change remotes, or rewrite history to bypass a failed push; otherwise leave pushing to the user.
- If local Git ownership protection triggers, use the narrowest per-command `safe.directory` handling possible; do not change global Git configuration unless the user explicitly asks.

## Invocation examples

- `$arxiv-human-centric-weekly 生成本周周报并在本地提交，不要 push。`
- `按项目的人体中心视觉周报流程整理上周 arXiv 论文。`

