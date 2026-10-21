# Humanize Writing

This skill cleans up the style tells that make a draft read like AI: the stock vocabulary, the throat-clearing phrases, the tidy three-item lists, and the summary paragraph nobody asked for. Install it in Claude and it'll check its own drafts against those rules before handing them back.

## What this skill doesn't do

In August 2026, Anthropic [announced](https://www.anthropic.com/news/claude-text-watermark) that it's watermarking text Claude generates. The watermark lives in Claude's word choices, which means it isn't something you can see or edit out by fixing style. When Claude runs this skill on a draft, Claude is still the one writing the new version, so the rewrite carries its own watermark. This skill makes your writing better. It won't make it untraceable, and it was never meant to.

If you need text that doesn't carry Claude's watermark, the honest route is rewriting it yourself. The more of the final wording that's yours, the less signal there is. For a tool-assisted approach, Guillaume Meyer's MIT-licensed [watermarks-remover](https://github.com/guillaumemeyer/watermarks-remover) strips hidden characters and file metadata, and it can rewrite text with a different model. Point it at a local model through Ollama so your text never leaves your machine. The author describes the rewrite step as best effort, and no one can currently verify that it works, because Anthropic's detection API isn't public.

Before you strip a watermark from anything, check the rules that apply to you. Journals, funders, and institutions are setting their own AI disclosure requirements, and NIH has said it won't consider applications substantially developed by AI to be original ideas ([NOT-OD-25-132](https://grants.nih.gov/grants/guide/notice-files/NOT-OD-25-132.html)). Removing a watermark doesn't change what those policies require.
