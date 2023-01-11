# Moonwalk Template
Template for generating a Jekyll website based on the Moonwalk (@abhinavs/moonwalk) theme

I personally use the [Moonwalk](https://github.com/abhinavs/moonwalk) Jekyll theme by [abhinavs](https://github.com/abhinavs) a lot, so this is a GitHub template that you can use to quickly create a Moonwalk website.

# Getting Started
- Click the `Use this template` button on the top of this repo
- Wait a couple of minutes for the GitHub Actions workflow to finish running
- Go to `Settings` and enable GitHub Pages to deploy from the `gh-pages` branch
- Your site should be up and running!
- For local development, fork this repo
- Make sure Jekyll and Ruby is up-to-date
- Run `bundle exec jekyll serve`
- Your site should be locally live

# Customization
## Download an asset from the internet
You can edit the `/.github/workflows/download.yml` file to routinely download an asset file from the internet before deploying your site.
- Uncomment the `push` workflow trigger (three lines)
- To download from a server other than GitHub, edit the url within the quotations on the `curl "..." -o ./assets/{SOMETHING}.md` line, replacing `{SOMETHING}.md` with a file path of your choice
- To download from GitHub, replace `{USER}` with a GitHub username, `{REPO}` with a GitHub repo, and `{SOMETHING}.md}` with a file path such as `README.md` or `assets/asset.png`, also replacing `./assets/{SOMETHING}.md` with a file path of your choice
## Home layout
Edit `/_data/home.yml` as per [Moonwalk](https://github.com/abhinavs/moonwalk)'s specification. 
## Site config
Edit `_config.yml` as per [Moonwalk](https://github.com/abhinavs/moonwalk)'s or Jekyll's specification. 
## Add pages
Edit `about.md` and `project1.md`, as well as add/remove markdown files for additional pages.
