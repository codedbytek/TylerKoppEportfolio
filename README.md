# Tyler Kopp – e-Portfolio

Professional e-Portfolio for CNT 3004 – Computer Network Concepts (UCF).
Live site: https://tylerkopp.netlify.app/

A plain static site (HTML/CSS with a small JS file). There is no build step.

| Page | File | Assignment requirement |
| --- | --- | --- |
| Home / About / Interests | `index.html` | Part 1: bio, professional photo |
| CNT 3004 | `cnt3004.html` | Course tab: HW reflections, quizzes and discussions, overall reflection |
| Resume | `resume.html` (+ `files/Tyler-Kopp-Resume.pdf`) | Resume |
| Professional Goals | `goals.html` | Professional goals |
| Certifications & Activities | `certifications.html` | Certifications and activities |

## Deploying with Netlify

`netlify.toml` tells Netlify to publish the repository root with no build command,
and it adds security headers. Every push to the production branch redeploys the site.

## Updating the resume

Replace `files/Tyler-Kopp-Resume.pdf`, then regenerate the preview image:

```bash
pdftoppm -r 130 -jpeg -singlefile files/Tyler-Kopp-Resume.pdf images/resume-preview
```
