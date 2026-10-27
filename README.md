# Privacy in Statistics and Machine Learning

Static course website developed by Adam Smith and Jonathan Ullman.

## Editing

- `index.html` is the landing page, including the instructor websites, YouTube channel, and links to each offering.
- `2021-spring/`, `2023-spring/`, and `2025-spring/` contain the semester pages and their original course materials.
- Each offering's `index.html` contains Course Information, including instructor contact details. Its former `contact.html` redirects to `index.html#instructors` for existing bookmarks.
- `css/dpcourse.css` is the shared stylesheet for every page. Its colors, typography, and section layout follow the Boston Area Differential Privacy website.
- Root-level `schedule.html` and `syllabus.html` preserve old links by redirecting to the Spring 2021 pages.

Edit the HTML directly. There is no build step, JavaScript dependency, or external font dependency. Preserve historical course content and material URLs when updating the presentation. Each page has its own navigation; keep the active link's `aria-current="page"` attribute aligned with the page.

HTML and CSS use two-space indentation, configured in `.editorconfig`. Keep CSS declarations on separate lines and wrap long HTML prose where practical; keep URLs and attribute values intact. The shared stylesheet is organized by navigation, page content, instructor profiles, responsive layouts, and print styles.

Identify offerings by both semester and institution in landing-page links, page titles, and offering headers. Spring 2021 was offered at Northeastern University (NU) and Boston University (BU); Spring 2023 and Spring 2025 were offered at BU. Use distinct directories for any future separate offerings in the same semester.

## Preview

Open `index.html` in a browser, or serve the repository locally:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then visit `http://127.0.0.1:8000/`. Check both desktop and phone widths. Wide data tables scroll within their own region on small screens and can receive keyboard focus.

Publishing uses the repository's existing static hosting setup; no generated files are required.
