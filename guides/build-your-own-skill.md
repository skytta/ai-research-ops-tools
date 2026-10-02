# Build Your Own Claude Skill

A skill is a set of instructions Claude loads automatically when a task matches. Think of it like a standard operating procedure: you write it once, and Claude follows it every time the situation comes up, so you stop retyping the same long prompt.

Good candidates are tasks you do repeatedly where you keep correcting Claude the same way. A compliance email format, how you want statistical output explained, a checklist for reviewing a document.

## 1. Make the file

Create a folder named for your skill (lowercase, hyphens, like `compliance-emails`). Inside it, create a text file named `SKILL.md` that starts like this:

```markdown
---
name: compliance-emails
description: Draft compliance emails to study teams in my preferred format. Use when I ask for an email about a deviation, CAPA, or IRB requirement.
---

# Compliance Emails

Your instructions go here.
```

The two lines at the top matter most. The `name` can be up to 64 characters. The `description` (200 characters max) is how Claude decides when to use the skill, so say both what it does and when to use it.

## 2. Write the instructions

Write the body the way you'd train a new team member. Cover:

- **The goal.** What a good result looks like.
- **The steps.** What to do, in order, if order matters.
- **The rules.** What to always do and what to never do.
- **An example.** One real sample of good output teaches more than a page of rules.

Start short. You can add to it every time Claude gets something wrong.

Shortcut: ask Claude to write the first draft. Describe the task, paste a couple of examples of output you liked, and ask it to turn that into a SKILL.md. Then edit it yourself so it reflects your judgment, not Claude's guesses.

## 3. Package it

Zip the **folder**, not just the file. The zip should contain your skill folder with `SKILL.md` inside it.

## 4. Upload it

In [Claude](https://claude.ai), go to **Customize > Skills**, click **Add**, and upload the zip. Code execution needs to be turned on for skills to work.

## 5. Test and refine

Start a new chat and ask for the task without naming the skill. If Claude doesn't pick it up, make the description more specific. If the output is off, add a rule or an example to the instructions and re-upload.

## Learn more

- Anthropic's guide: [How to create custom skills](https://support.claude.com/en/articles/12512198-how-to-create-custom-skills)
- Example skills: [github.com/anthropics/skills](https://github.com/anthropics/skills)
- For a working example, see [`skills/humanize-writing`](../skills/humanize-writing/) in this repo.

*Check your institution's AI policy before using Claude with work documents.*
