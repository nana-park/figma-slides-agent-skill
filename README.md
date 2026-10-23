# Figma Slides Agent Skill

A Korean-language skill for planning slides and assembling a clear production prompt for Figma or presentation tools.

It collects requirements across ten input sections. It is a set of instructions and templates, not a standalone app.

## Quick start

1. Download or clone this repository and open it in your agent workspace.
2. Ask the agent to read [SKILL.md](SKILL.md).
3. Provide the topic, audience, goal, source material, and desired output.
4. Fill in the required inputs. The agent should ask only for missing information.
5. For prompt-only work, the output is `outputs/final-prompt.md`. For slide production, connect a supported Figma or presentation tool and provide the target file.

Korean example request:

> SKILL.md를 읽고 신제품 소개 발표의 요구사항을 정리해줘. 우선 제작 프롬프트만 만들어줘.

## Input sections

| Section | Purpose |
| --- | --- |
| [01 Design system](01-design-system/README.md) | Size, colors, typography |
| [02 Common layout](02-common-layout/README.md) | Grid, components, text |
| [03 Slide types](03-slide-types/README.md) | Covers, contents, chapter dividers |
| [04 Charts and tables](04-charts-and-tables/README.md) | Data and visual rules |
| [05 References](05-references/README.md) | What to reuse from a reference |
| [06 Purpose](06-purpose/README.md) | Audience, goal, key message |
| [07 Source material](07-source-materials/README.md) | Evidence and research scope |
| [08 Storytelling](08-storytelling/README.md) | Narrative and transitions |
| [09 Slide content](09-slide-content/README.md) | Content for each slide |
| [10 Production and review](10-production-rules/README.md) | Editing, layout, checks, export |

## Set up your own references

No private Figma files, node links, lecture conversations, student records, personal contact details, or brand assets are included. Supply references that you have permission to use. Sample-based rules require your own reference; the agent must not claim to have inspected an unavailable file.

The numeric tables are reusable default presets. Keep project-specific inputs and links in `private/` or `outputs/`, which are ignored by Git. Review staged files before publishing: .gitignore does not protect files already tracked.

## Requirements and limits

The core guides are in Korean. Actual slide creation needs a compatible tool, access to the target file, and the required fonts. Editable charts, shapes, and exports depend on that tool.

This public edition has not been tested through a complete deck production run. Prompt completion, file creation, and visual review are separate results and must be verified separately.

This is a clean public edition with fresh history. Personal records and the original repository history are excluded. No executable code was changed; project-specific documentation was generalized.
