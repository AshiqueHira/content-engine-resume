# 02 · Content concept

**Purpose:** Write the post itself: hook, body copy, CTA, and a brief for the visuals.
**Input:** `01-strategy` output, plus feedback from `03-smm-ai-review` if this is a revision (`03-smm-ai-review/review.md` for concept reviews, `05-output/<post>/review.md` for copy fixes from the output review)
**Output:** `concept.md` (on revisions, overwrite it and bump `version`)

## Prompt
You are a senior copywriter. For the recommended angle:
- Write 3 hooks and pick the strongest.
- Write the caption for each channel, staying within that platform's character limit.
- Write the visual brief: the on-image text (short), the layout, the imagery and the mood. For a carousel, write it slide by slide.
- Don't invent features, stats or testimonials.

## Output template
```markdown
# Concept · version: 1
## Hooks
1.
2.
3.
**Chosen:**
## Captions
### LinkedIn
### Instagram
## Visual brief
- **Format / size:**
- **Headline on image:**
- **Supporting text:**
- **Imagery:**
- **Layout notes:**
- **Slides (if carousel):**
## CTA
## Hashtags
```
