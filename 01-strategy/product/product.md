# Product: Kedilo Resume

<!-- Source of truth for what the product does. Strategy reads this to pick which feature a post promotes.
     Source: the product repo (kedilo-resume: README.md, PROJECT.md, AGENTS.md, templates/registry.ts), Oct 2026.
     Re-check the repo before promoting a feature: the code moves faster than this file.
     Ranks are editable. Change the number in the table and re-sort; nothing else depends on the order. -->

## The idea
**Kedilo Resume** (resume.kedilo.com) is a free resume and cover-letter builder. Fill in a simple form, watch a live preview, and download a clean, **ATS-friendly** PDF in about 5 minutes. You can build and download without an account. Signing in (Google) adds cloud save, more than one resume, and a public share link.

- **North star:** get the user an interview. A resume that looks good but fails an ATS parse has failed.
- **Two gates, every time:** pass ATS/AI screening (the text gets extracted correctly), *and* look professional to the human who reads it next.
- **Price:** completely free: signup, saving and publishing. No watermark, no paywall at download. (Razorpay billing code exists but is switched off. Don't mention pricing or "Pro".)
- **Privacy:** the anonymous draft stays in the browser (localStorage). PDF import runs in the browser too. Nothing leaves the device until the user signs in.

## Features, ranked by priority
Rank = how strongly we lead with it in content (1 = lead message). Ranking logic: it serves the north star, it answers a persona's pain or objection, and it sets us apart from Canva, Naukri and paid builders.

| Rank | Feature | Description | Main persona | Status |
|---|---|---|---|---|
| 1 | **Free, no watermark, no sign-up** | Build and download the full PDF without an account, card or watermark. Answers the objection "free tools always have a catch". | All | Built |
| 2 | **ATS-friendly output** | Real selectable text (never an image), one logical reading order, standard section headings (Summary, Experience, Education, Skills, Projects), web-safe fonts. The parser reads what the recruiter wrote. | Fresher Arjun | Built |
| 3 | **Live preview + 5-minute build** | Form on the left, the finished resume on the right, updating as you type. What you see is exactly what prints. Sample data shows you what good looks like. | All | Built |
| 4 | **Country-specific templates** | Formats per market: Gulf/GCC with photo and without photo (nationality, visa status, DOB, passport), US, UK CV, EU (Europass-style) and Dutch. The form shows the extra fields each format needs. | Gulf-bound Shameer | Built |
| 5 | **Import an existing PDF resume** | Upload your old resume and the fields fill in for you. Runs entirely in the browser (no upload to a server, no AI). Removes the "starting over" barrier. | Shameer, Restarting Anjali | Built |
| 6 | **Share link + peer review comments** | Publish a resume at a public link (kedilo.com/username/slug), send it to a senior or friend, and they leave comments on it. Answers "resume onnu nokkamo?" | Fresher Arjun | Built (needs sign-in) |
| 7 | **Reviewer marketplace** | A public directory of reviewers (with role, employer, experience and LinkedIn shown). Send a resume to one; they can comment on it and edit it directly. Payment, if any, happens off-platform. | Arjun, Anjali | Built (MVP) |
| 8 | **Multiple saved resumes (cloud)** | Save several resumes in one free account, autosave as you type, and rename, duplicate or delete them from the dashboard. Keep an India version and a Gulf version. An anonymous draft is imported automatically on first sign-in. | Gulf-bound Shameer | Built (needs sign-in) |
| 9 | **Template gallery (12 designs)** | Classic, Modern, Crisp, Minimal, Photo, Sidebar plus the 6 regional formats. Switch designs at any time without retyping. ⚠️ Photo and Sidebar are labelled "Not ATS-optimized", so don't use them in ATS-focused posts. | All | Built |
| 10 | **Cover letter builder** | The same form + live preview + PDF flow for cover letters, saved alongside resumes on the dashboard. | Shameer, Anjali | Built |
| 11 | **Section manager + photo upload** | Show, hide and reorder sections; add a profile photo on templates that support one (Gulf, Photo, Sidebar). | Shameer | Built |
| 12 | **Blog / career guides** | Articles on resume writing and job hunting at /blogs. Useful as link targets for content, not as a feature to sell. | All | Built |

### Roadmap: not built, do not promote yet
Listed so strategy doesn't promise these by accident. Ranked by the product team's own priority.

| Rank | Feature | Description |
|---|---|---|
| R1 | **Content guidance** | Inline tips, action-verb hints, "quantify this" nudges and length warnings while you type. |
| R2 | **ATS self-check** | Warnings for empty key sections, missing dates, weak bullets and a resume that runs too long. |
| R3 | **Job-description tailoring (AI)** | Paste a job description to get a keyword-gap analysis and suggested skills and phrasing. |
| R4 | **AI bullet rewriting** | Turns weak duty lists into quantified achievements. |
| R5 | **A4 / Letter toggle + density controls** | Page-size choice and font-size and spacing controls. |

## Claims guardrails
- Never promise interviews or jobs ("Will it actually get me calls?"). Explain *why* ATS-friendly formatting helps, and show a before→after.
- "Every template is ATS-safe" is **false**: Photo and Sidebar are not. Say "ATS-friendly templates" or name one (Classic, Modern, Crisp, Gulf No-Photo, US, UK).
- PDF download goes through the browser's print dialog ("Save as PDF"). Show that step in tutorials so it doesn't surprise anyone.
