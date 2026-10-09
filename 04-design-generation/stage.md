# 04 · Design generation

**Purpose:** Turn the approved visual brief into image files.
**Input:** The concept that passed `03-smm-ai-review` (concept mode), plus `05-output/<post>/review.md` if the output review sent image fixes back here
**Output:** Images and a `design.md` note, saved to `05-output/`

## Approach (pick one per post, and record which)
- **HTML/CSS → PNG**: render a branded template (e.g. Playwright screenshot). Best for text-heavy posts and carousels, and gives exact fonts.
- **Image model**: for illustrative or photo-style backgrounds, then overlay the text with the HTML template.
- **Design tool API** (Canva/Figma/Bannerbear): fill a template you already have.

## Rules
- On-image text must match the approved copy exactly.
- Export the right size for each channel.
- File naming: `<channel>-<slide#>-<WxH>.png`
