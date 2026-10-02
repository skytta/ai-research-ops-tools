# AI Tools for Research Operations

Practical AI tools for clinical research teams, built by **Jenny AF Skytta**, Clinical Research Manager at Seattle Children's Research Institute.

These came out of real daily work: drafting IRB submissions, writing compliance correspondence, and teaching colleagues to build their own tools. The core idea behind all of them is that AI compresses the build time, but it doesn't replace the domain knowledge you need to get the output right. Every draft these tools produce still needs a qualified human reviewer.

## What's here

| Folder | What it is | Runs in |
|---|---|---|
| [`irb-gem/`](irb-gem/) | Instructions for a Gemini Gem that walks you through drafting IRB protocol content section by section | Google Gemini, ChatGPT Projects, or Claude Projects |
| [`skills/humanize-writing/`](skills/humanize-writing/) | A Claude skill that strips common AI writing tells out of drafts | Claude |
| [`guides/build-your-own-skill.md`](guides/build-your-own-skill.md) | A short walkthrough for building your own Claude skill from scratch | Claude |

## Before you use the IRB Gem

Check your institution's AI policy first. Many institutions require approval before AI tools are used with research documents. Never paste identifiable participant data or PHI into any AI tool your institution hasn't approved for that use.

The Gem works best when you upload your own IRB's templates and guidance documents as knowledge files. Those aren't included here because they belong to each institution. See [`irb-gem/README.md`](irb-gem/README.md) for setup.

## Credit and license

Shared under [CC BY 4.0](LICENSE). You're welcome to use, adapt, and share these tools, including in your own talks and trainings, as long as you credit the original author:

> Skytta, J. A. F. (2026). *AI Tools for Research Operations*. GitHub. https://github.com/skytta/ai-research-ops-tools

Questions about how any of this was built are welcome. Open an issue on this repo.
