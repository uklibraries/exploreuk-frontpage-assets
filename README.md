exploreuk-frontpage-assets
==========================

This is a collection of images and logos used by the [ExploreUK web application](https://github.com/uklibraries/exploreuk-web-app/).

## Layout

- `shared/` holds static assets shared by
  [exploreuk-web-app](https://github.com/uklibraries/exploreuk-web-app/)
  and [findingaid](https://github.com/uklibraries/findingaid). Both
  include this repository as a git submodule and copy `shared/` into their Docker
  images at build time, so a change here reaches a site only after that app bumps
  its submodule pointer and redeploys.
- `files/` is seed data for ExploreUK's `/files` directory in local development.
  Production's `/files` is restored from backups, not from this repository.
