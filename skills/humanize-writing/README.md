# Humanize Text – UPDATE *** Oct 2026***

This skill was created to remove common AI indicators like repetitive lexicon, filler phrases, standard three-item sequences, and unneeded summary sections. Once loaded into Claude, the skill can evaluate its output against these standards prior to output.

## Limitations of this Skill

Watermarks are embedded in the text Claude produces, a fact Anthropic [announced](https://www.anthropic.com/news/claude-text-watermark) in August 2026. Because these markers are woven into the model's word choices, they are invisible and cannot be removed through stylistic editing via Claude itself. Even when Claude applies this skill to a draft, the AI remains the author of the new version; thus, the watermark remains. This is also true for other AI operations like OpenAI in an effort to conform to EU regulations.

The most transparent way to produce text without Claude's watermark is to rewrite it yourself. This way, you minimize the detectable watermark signal.

Alternatively, you can use Guillaume Meyer's MIT-licensed [watermarks-remover](https://github.com/guillaumemeyer/watermarks-remover) to strip metadata and hidden characters or to rewrite text via a different model. To keep your data on your own hardware, point the tool at a local model using Ollama (or other local tool). One caveat, because Anthropic’s detection API is not public, the success of the "best effort" rewriting process described by the author cannot be verified.

Always consult the relevant regulations before attempting to strip a watermark. Various institutions, funders, and journals are establishing AI disclosure mandates. For instance, the NIH ([NOT-OD-25-132](https://grants.nih.gov/grants/guide/notice-files/NOT-OD-25-132.html)) has stated that applications largely developed by AI will not be viewed as original ideas. Obscuring a watermark does not change these policy requirements.
