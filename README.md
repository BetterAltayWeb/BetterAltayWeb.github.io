# BetterAltay static website

A responsive, buildless website for GitHub Pages. No PHP backend, Node installation, build step, API key or database is needed.

The site links to BetterAltayBedrock/BetterAltay and BetterAltayBedrock/PHP-Binaries. It fetches public GitHub release metadata in the browser, then displays the first non-prerelease release among the latest ten returned entries. It does not execute or install software. GitHub rate limits or network failures show an explicit fallback with an always-available release page link. There are no bundled PHAR files or PHP executables in this website archive. Those are downloaded from upstream.

## Plugin catalog

Plugin sources are linked in the catalog. Documentation should be reviewed against the selected server release before publication. Generic troubleshooting and maintenance guidance is not a guarantee of support for every world format, block or plugin.

This is a community resource template, not a claim of official project ownership. BetterAltay software has its own upstream LGPL-3.0 license. Minecraft belongs to its respective owners.

## Branding

`assets/icon.png` is the supplied BetterAltay badge, used in the header, footer and favicon. Replace this PNG to change the logo. Colours are charcoal, warm gold and bronze; key theme variables are at the top of `assets/style.css`.
