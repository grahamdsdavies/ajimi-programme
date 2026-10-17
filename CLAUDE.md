# ajimi academy Owase 2026: chef programme

Phone-first programme for the ajimi academy 2026 chef cohort (18–25 October 2026, Owase, Mie).
Live at https://ajimi.ishinoko.jp (GitHub Pages from this repo, branch `main`, root). A push to `main` is live in about a minute.

## Files
- `programme.md`: all the text chefs read. Almost every change happens here. The comment at the top explains the syntax.
- `index.html`: page template, styles and the parser that turns `programme.md` into the page. Only touch for layout or design changes.
- `logo.png`, `map.png`: ajimi logo and hand-drawn Owase map.
- `CNAME` (ajimi.ishinoko.jp), `robots.txt` (blocks search engines and AI crawlers), `.nojekyll`. Leave as they are.

## programme.md syntax (quick reference)
- `# Owase 2026 programme` is the info page; `## Heading` makes a section there.
- `# Sun 18 · Title` starts a day. `Flexible: yes` under it adds the dot in the date bar.
- Day intro: first paragraph = lede; `- Label: value` lines = the four at-a-glance boxes; `> **Bold.** text` = notice.
- `### 09:00–11:00 · Title` = session (time optional). Fields under it: `Place: Name · map-url`, `Learn:`, `Group:`, `Tags: a; b` (comma or semicolon), `Style: key` or `Style: free`. Then a blank line and the description.
- `! **Bold.** text` inside a session = warning box. `> text` inside a session = notice box.
- `--> 09:00 · text` = departure (highlighted; walk/bus/car icon chosen from the words). `--> 15 min drive` without a time = plain travel line.
- `=== Title` / `== Group A · Label` / `===` = split block for group mornings.
- Info page: `+ **Title** text` = tap-to-open box; `==word==` highlights a word. `- **18** label` lists render as big numbers; short plain lists render as pills.
- Inline: `**bold**`, `*italic*`, `[text](url)`. `<!-- -->` hides text (must close at the end of a line).

## Writing rules
- UK English (programme, colour). No em dashes.
- Warm, clear, professional. This is an educational course: keep the learning framing.
- No Japanese characters in chef-facing text; use romaji (most chefs can't read kanji). Place names in English with a map link.
- No chef names, phone numbers or prices on the page: it is public. Private details go in the WhatsApp community.
- "Self paid" (not "pay your own"). "ajimi academy" and "ajimi open table" are always lowercase.

## Workflow
- Pull before editing; use VS Code Source Control "Sync Changes" to publish.
- Do not deploy anything via the ishinoko.jp Netlify site: its free plan has run out of build credits. This page must stay on GitHub Pages.
- To preview locally: VS Code Live Preview on `index.html` (it fetches `programme.md`, so open it through a server, not as a file).
