# BetterAltay static website

A responsive, buildless website for GitHub Pages. No PHP backend, Node installation, build step, API key or database is needed.

## Publish on GitHub Pages

1. Extract this archive and upload the **contents** of `betteraltay-site` to your repository root. Include `.nojekyll`.
2. Commit the files to your main branch.
3. In GitHub, open Settings → Pages → Build and deployment.
4. Select **Deploy from a branch**, choose your branch and **/(root)**, then Save.
5. Open the Pages URL after GitHub finishes deployment.

All internal links are relative, so both `username.github.io` and `username.github.io/repository/` work. No custom domain is assumed.

## Files

- `index.html`: homepage with original gold-toned SVG terrain illustration.
- `docs.html`: installation, configuration, connection, commands, plugins, backups and troubleshooting.
- `downloads.html`: server releases and platform installation tabs.
- `php.html`: prebuilt runtime releases and verification instructions.
- `plugins.html`: searchable and filterable project discovery library.
- `assets/plugins.js`: editable plugin catalog.
- `assets/app.js`: navigation, clipboard, platform tabs, filters and GitHub release loading.
- `assets/style.css`: responsive shared design.

## Downloads

The site links to BetterAltayBedrock/BetterAltay and BetterAltayBedrock/PHP-Binaries. It fetches public GitHub release metadata in the browser, then displays the first non-prerelease release among the latest ten returned entries. It does not execute or install software. GitHub rate limits or network failures show an explicit fallback with an always-available release page link. There are no bundled PHAR files or PHP executables in this website archive. Those are downloaded from upstream.

Do not hardcode a “latest Minecraft version” claim without maintaining it. The project release notes remain authoritative. A runtime must match the selected BetterAltay build, OS and architecture.

## Plugin catalog

Edit `assets/plugins.js` to add entries. Each has `name`, `category`, `icon`, `description`, `url` and `kind`. Add matching select options in `plugins.html` for new categories. Entries are real project discovery links, **not tested compatibility endorsements**. Historical API 3 releases may be required; modern releases may be incompatible. Developer libraries are not necessarily standalone plugins. Before claiming compatibility, test the exact plugin version with the exact BetterAltay release and record both.

## Preview

Open `index.html` directly, or serve this directory with `python3 -m http.server 8000`. Clipboard support depends on a secure context. Navigation, documentation and upstream download links work without JavaScript; live assets, tabs and filtering use JavaScript.

## Maintenance / sources

Installation flow: https://github.com/BetterAltayBedrock/BetterAltay
Runtime distribution: https://github.com/BetterAltayBedrock/PHP-Binaries
Plugin sources are linked in the catalog. Documentation should be reviewed against the selected server release before publication. Generic troubleshooting and maintenance guidance is not a guarantee of support for every world format, block or plugin.

This is a community resource template, not a claim of official project ownership. BetterAltay software has its own upstream LGPL-3.0 license. Minecraft belongs to its respective owners.

## Branding

`assets/icon.png` is the supplied BetterAltay badge, used in the header, footer and favicon. Replace this PNG to change the logo. Colours are charcoal, warm gold and bronze; key theme variables are at the top of `assets/style.css`.
