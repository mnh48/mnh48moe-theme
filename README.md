# MNH48 Theme (THEME.MNH48.MOE)

This repository contains the file of the theme used across MNH48 websites. The
theme is written to be used in **Github Pages** environment with the
**kramdown** parser, either directly on Github or by local Jekyll serve
instance that had been setup to run Github Pages gem.


## How to use the theme?

1. Open your `_config.yml` file where you store your Github Page site setting.
2. Paste `remote_theme: mnh48/mnh48moe-theme` in a new line.
3. Save and close it.
4. Copy the `/_data` directory and paste it at your site root.
5. Edit the files in `/_data` to reflect your site, you can safely remove any
language in there that you are not using.


## License

This theme, which is used for the website layout for various MNH48 websites,
is released under The MIT license, this includes the files in the `/_layouts`,
`/_data`, and `/_includes` directories.

The CSS files used has been moved to my server for consistency reason where
source is not available temporarily, but the source will be re-release again
later. They are still licensed under The MIT license even when source is moved
temporarily, people who used the CSS before the move can continue to use it
while I sort it for new version release.

The example website that is generated from this theme, which lives at
https://theme.mnh48.com, and its source markdown files in this repository,
are also all licensed under The MIT license.
