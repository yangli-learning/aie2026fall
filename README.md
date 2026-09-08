# AIE1901 (Fall 2026): AI That Learns Throughout Its Lifetime

Course website for **Session 01 of AIE1901 AI Exploration I** at **The Chinese University of Hong Kong, Shenzhen**.

The site uses the Jemdoc project structure:

- `jemdoc_files/` contains the editable source.
- `www/` contains the generated static site.
- `jemdoc` is the local Jemdoc generator.

To regenerate the HTML pages:

```bash
cd jemdoc_files
python ../jemdoc -c mysite.conf -o ../www/ *.jemdoc
```

To preview the generated site locally:

```bash
python -m http.server 8000 --directory www
```

Then visit `http://localhost:8000`.

## Updating course materials

- Edit `jemdoc_files/course-content.jemdoc` to add lecture slides and readings under Lectures, or lab materials and related assignments under Labs.
- Store lecture files in `www/materials/lectures/` and lab files in `www/materials/labs/`, then link to them using paths relative to `www/` (for example, `materials/labs/Lab1.zip`).
