# 05 · Output

**Purpose:** Collect the final, ready-to-publish post: captions plus images.
**Contents (one subfolder per post, e.g. `2026-10-09-my-topic/`):**
- `post.md`: final caption per channel, CTA, hashtags, scheduled time
- `*.png`: images from `04-design-generation`

- `review.md`: written by the `smm-reviewer` agent (03, output mode). Don't edit it by hand.

When the folder is complete, run the `smm-reviewer` agent in output mode on it. Only posts in this folder whose `review.md` verdict is `pass` can be published by `06-publish`.
