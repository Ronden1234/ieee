# PRD - IEEE CYB Conf 2027 website

## Original problem
User provided GitHub repo https://github.com/SWC-IEEE-2026/SWC-IEEE-2026.github.io (Jekyll site for IEEE SWC 2026) and PPT "PresentationCalabria_CYBConf27.pptx". Goal: create the site for IEEE CYB Conf 2027 from the PPT contents, keeping the visual layout as close as possible to the original.

## Architecture
- Static Jekyll site at /app/cybconf (git repo, original history + 1 commit)
- Preview: frontend supervisor runs `bundle exec jekyll serve --watch` on port 3000 (package.json start script)
- Data files: _data/cyb_data.json (dates/theme), committee.yml, cfp_topics.yml, calabria.yml, navigation.yml, sponsors.yml
- PPT images extracted to assets/images_27/ppt/

## Implemented (Oct 2026)
- Home, Call for Papers, Program, Committee (+TPC), Discover Calabria (tourism, cuisine, food gallery), Social Event (MAB + Cosenza Castle), Accommodation (Socrates + 4 hotels), Getting There (PPT flight info), Registration (coming soon), Contact, Venue, Visa, Sponsors
- Removed SWC-specific pages (co-located conferences, workshops, keynotes, tutorials, hackathon, slides, etc.)

## Backlog
- P1: real keynote speakers, workshops/special sessions, submission system link, registration fees
- P1: contact emails for TPC/local arrangement/web chairs, committee photos
- P2: CFP PDF flyer, push to a new GitHub repo / GitHub Pages
