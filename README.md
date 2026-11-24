# Coherent instrument support

Static Jekyll pages for instrument software and connection instructions.

## Preview locally

Open the repository directory in your terminal. The site uses `/dev/`, including locally, to match GitHub Pages.

### Docker on Linux or Windows

Start Docker Desktop with Linux containers. In PowerShell, run:

```powershell
docker compose run --rm -e BUNDLE_FROZEN=true site bundle install
docker compose up
```

Open **http://127.0.0.1:4000/dev/**. Jekyll rebuilds when you edit content; LiveReload refreshes the browser.

### Native Ruby (without Docker)

Use Ruby **4.0.7** and Bundler **4.0.20**, matching `.ruby-version` and `Gemfile.lock`.

On Windows, install Ruby with DevKit using RubyInstaller and complete its development-tools setup. Reopen your terminal so Ruby is on PATH. If the required Bundler version is missing, run `gem install bundler -v 4.0.20`.

```sh
bundle install
bundle exec jekyll serve --livereload --host 127.0.0.1 --baseurl /dev
```

Open **http://127.0.0.1:4000/dev/** to see the live preview

## Build and review

```sh
docker compose run --rm -e JEKYLL_ENV=production -e BUNDLE_FROZEN=true site bundle exec jekyll build --strict_front_matter --baseurl /dev
```

With native Ruby, set `JEKYLL_ENV=production` and run `bundle exec jekyll build --strict_front_matter --baseurl /dev`.

Before merging, inspect the homepage and each changed product page at desktop and phone widths. Follow product links, check the real software-sharing destination, expand Ethernet instructions, and try keyboard navigation. A successful Jekyll build does not establish that hardware instructions or an external installer are correct.

## Pull requests and production

Use the local `dev` branch for this refresh, then open a pull request into `main`. Future changes can use short-lived topic branches; a permanent integration branch is not required.

`.github/workflows/pages.yml` defines:

- **Pull requests targeting `main`:** install locked dependencies and build. No deployment or Pages write permissions.
- **Pushes to `dev`:** build only.
- **Pushes to `main`:** build, upload the generated site, then deploy that artifact through the `github-pages` environment. The deploy job requires a successful build.

For a bad release, revert the offending change through a PR and merge it. The resulting successful `main` build republishes the prior content. Changing an external download share is a separate release operation; reverting this site does not roll back a file replaced there.
