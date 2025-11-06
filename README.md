# Kjendseth Lab Website

This repository hosts the source for [kjendseth.github.io](https://kjendseth.github.io), the academic homepage for Åsmund Røhr Kjendseth and the Kjendseth Lab at the Norwegian University of Life Sciences (NMBU). The site is powered by [Jekyll](https://jekyllrb.com/) with the [al-folio](https://github.com/alshedivat/al-folio) theme and customized for research on lytic polysaccharide monooxygenases (LPMOs), redox enzymes, and related spectroscopy and computational chemistry.

## Local development

The site uses Jekyll 4 and Ruby 3.1+ (see `Gemfile.lock`). If your system Ruby is older, install a newer toolchain (via `rbenv`, `asdf`, or `ruby-install`) before running the commands below.

```bash
bundle install
bundle exec jekyll serve
```

Visit <http://localhost:4000> to see the development build. Hot reloading is enabled for most content edits.

### Docker (alternative)

If you prefer containerized builds:

```bash
docker compose up
```

This will mount the workspace and run `jekyll serve` inside the official container declared in `docker-compose.yml`.

## Content structure

- `_pages/` – main site sections (about, projects, publications, teaching, etc.)
- `_news/` – short announcements surfaced on the home page
- `_projects/` – research highlights linked to publications
- `_bibliography/papers.bib` – publication list rendered via `jekyll-scholar`
- `_data/` – structured data (social links, CV highlights, repositories)
- `assets/img/` – lab imagery and profile photos

## Licensing

The al-folio theme is distributed under the MIT license. See `LICENSE` for details.
