# UI Design Rules Skill

A Claude Code skill that makes an AI build interfaces with a real spacing system, sensible buttons, consistent icons and correct social share images, instead of random pixel values and one-off styles.

Left alone, AI-generated front end code tends to use `13px` here, `19px` there, three different button styles on one page, and icons that shift the layout when you swap them. This skill gives the AI a short rulebook to check against, plus the reasoning, so it can make good calls on cases the rules do not cover.

## What it covers

| Area | Reference file |
| --- | --- |
| 4px spacing scale, micro and macro rhythm | `references/spacing-4pt.md` |
| Material Design 3 spacing tokens and breakpoints | `references/spacing-material-3.md` |
| Button hierarchy, placement, copy and touch targets | `references/buttons.md` |
| Icon library choice, sizing, naming, SVG and hit areas | `references/icons.md` |
| Social share (Open Graph) image specs | `references/og-images.md` |
| File and class naming | `references/naming.md` |
| QA checklist before showing UI work | `references/qa-checklist.md` |

## Install

For Claude Code, copy the skill folder into your skills directory:

```bash
git clone https://github.com/rifatnewajrazin/ui-design-rules-skill.git
mkdir -p ~/.claude/skills
cp -r ui-design-rules-skill/skills/ui-design-rules ~/.claude/skills/
```

For a single project, copy it to `.claude/skills/` inside the project instead.

The skill loads when you ask for UI work. You can also call it by name: "use the ui-design-rules skill to build this page".

## Using it without Claude

The reference files are plain markdown. Paste the ones you need into any assistant's instructions, or use them as a human checklist.

## Try it

`examples/tokens.css` is a ready-to-use set of spacing tokens. `examples/button.css` shows the button rules applied to real CSS.

## Where the rules come from

These are my own working rules, shaped by these sources. Read them, they are good:

- [UX Planet: Principles of spacing in UI design](https://uxplanet.org/principles-of-spacing-in-ui-design-a-beginners-guide-to-the-4-point-spacing-system-6e88233b527a)
- [Google Material Design 3: Spacing](https://m3.material.io/styles/spacing/overview)
- [Balsamiq: Button design best practices](https://balsamiq.com/blog/button-design-best-practices/)
- [Koala UI: Guide to using icons in UX/UI](https://www.koalaui.com/blog/ultimate-guide-best-practices-icons-2024)

The wording here is mine. The ideas belong to their authors.

## Contributing

Pull requests welcome. See `CONTRIBUTING.md`. Please back any new rule with a reason.

## License

MIT. Written by [Rifat Newaj Razin](https://github.com/rifatnewajrazin).
