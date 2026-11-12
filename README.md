# Biology SBA Designer

A reusable AI skill for teachers collaboratively designing Hong Kong Diploma of Secondary Education (HKDSE) Biology school-based assessment (SBA) investigations.

It supports experimental-design questions (Area B1), reporting questions (Area B2), and teacher marking guidance aligned with the applicable official assessment descriptors.

## What it does

- Reviews the official handbook, sample tasks and their marking schemes, and existing teacher materials.
- Proposes a blueprint and question map for teacher approval before substantial drafting.
- Develops questions one at a time, with one target descriptor per question.
- Provides Basic / Good / Excellent marking tables, illustrative answers and acceptance notes.
- Tracks the agreed question count and distribution of target performance levels.
- Checks scientific accuracy, feasibility, safety, authentication, repeated assessment and question dependencies.

## Repository structure

The skill is stored under [skills/biology-sba-designer](skills/biology-sba-designer/):

| File or folder | Purpose |
|---|---|
| `SKILL.md` | Core workflow and quality requirements |
| `agents/openai.yaml` | Skill display metadata and example starting prompt |
| `assets/` | Display icon |
| `references/marking-format.md` | Question and marking-table format |
| `references/worked-example.md` | Illustrative smartwatch task and question maps |
| `references/source-guide.md` | Official handbook link, source requirements and descriptor checks |

## Before starting

Provide the examination year and applicable official SBA handbook, topic, student level, available equipment, practical time and any existing task materials. Include a sample task and its marking scheme if you want a particular format followed.

The source guide links to the 2027 HKEAA handbook. The PDF and extracted handbook text are not redistributed in this public repository. Obtain the handbook for the intended cohort and check for amendments.

## Using the skill

In an environment that supports skills, install or load the complete `skills/biology-sba-designer/` folder using that environment's supported procedure. Saving it on GitHub alone does not install it in ChatGPT or another application.

If the skill is installed in ChatGPT, select `@biology-sba-designer` and describe the task. For example:

> Help me design an HKDSE Biology SBA investigation about osmosis. Read the attached handbook and sample marking scheme first. Propose a blueprint and question map, then develop the questions one at a time after approval.

After approving the map, continue with requests such as `Q2 please` or `Part 3, Q2(b)` in the same conversation.

If skill installation is unavailable, provide the core instructions and relevant references to your AI assistant as task guidance. This is a manual fallback, not an installed skill.

## Marking principles

Each question has one target descriptor. Its marking table can recognise lower performance without changing that target. Columns above the target are marked as not targeted.

Question-level observations contribute evidence to the overall B1 or B2 judgement out of 10. The skill does not invent an arithmetic conversion from question labels to the final mark.

Question counts and Basic / Good / Excellent distributions are agreed with the teacher. The worked example's distributions are preferences for that example, not official requirements.

## Teacher review and confidentiality

This is a teacher-facing design aid, not an official HKEAA product or an automatic student-grading system. Teachers remain responsible for assessment decisions, scientific accuracy, safety and compliance with the applicable handbook.

Keep suggested answers separate from student task sheets. Do not upload identifiable student work, health information or personal device records to this public repository. Label hypothetical data as illustrative.

## Maintenance

Check official requirements when the examination year changes. Recheck descriptor mappings and examples after revisions. Copies installed elsewhere must be updated separately when this repository changes.
