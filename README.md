# Lattice

A dark, motion-led one-page site for a creative developer or a small studio. The contact form posts to Formgong and shows "received" only when the server answers success: true; any other answer shows the server's message.

![Lattice](https://raw.githubusercontent.com/formgong-hq/lattice-hugo-theme/main/images/screenshot.png)

Demo: https://lattice.formgong.com

## Install

As a Hugo module:

```sh
hugo mod init example.com/site
```

```toml
# hugo.toml
[module]
  [[module.imports]]
    path = "github.com/formgong-hq/lattice-hugo-theme"
```

Or as a git submodule:

```sh
git submodule add https://github.com/formgong-hq/lattice-hugo-theme.git themes/lattice
echo 'theme = "lattice"' >> hugo.toml
```

Every text of the page lives in `data/content.json`. Copy `exampleSite/data/content.json` into your site's `data/` folder and edit it there; without it the theme uses its own copy.

Hugo 0.156.0 or newer, no npm packages and no Hugo extended needed. Posts, tags, categories and the RSS feed use the theme's list and single layouts.

## Run the example site

```sh
cd exampleSite
hugo server --themesDir ../..
```

## Contact form

The contact form posts to Formgong (free plan): put your access key in `form.access_key` in `data/content.json`. To send it anywhere else, change `params.formAction` in `hugo.toml`.

## Fonts

Montserrat, IBM Plex Mono: bundled as WOFF2 files (Latin and Latin Extended), no requests to Google Fonts. SIL Open Font License 1.1, the licence texts are next to the font files.

## License

MIT
