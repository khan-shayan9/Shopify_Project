# Little Steps — Shopify Theme

Shopify storefront theme for **Little Steps**, a baby-products store. Built on Shopify's Dawn theme and customized with a visual page builder for the homepage, product, and collection pages.

## Overview

- **Base theme:** [Dawn](https://github.com/Shopify/dawn) (Shopify's reference theme)
- **Page building:** [GemPages](https://apps.shopify.com/gempages) — the homepage, product, and collection templates each have a GemPages-generated version alongside a preserved Dawn default/backup template
- **Fonts:** [Fontio](https://apps.shopify.com/fontio) for custom web font embedding
- **Extras:** wishlist section, back-to-top and decorative section blocks added via installed apps

## Structure

```
My-theme/
├── assets/     # Dawn's CSS/JS, largely unmodified
├── config/     # Theme editor settings (colors, fonts, layout) + schema
├── layout/     # theme.liquid and checkout layout
├── locales/    # Dawn's default translations (30+ languages, unmodified)
├── sections/   # Dawn sections + app-injected sections (GemPages, wishlist, etc.)
├── snippets/   # Reusable Liquid partials
└── templates/  # Page templates — includes GemPages variants and backups
                # for index/product/collection pages
```

## Notes

- Template files with `.gem-*` or `.gp-template-bk-*` suffixes are GemPages-generated page variants and preserved Dawn backups — kept so the original Dawn layout can be restored if needed.
- `config/settings_data.json` still has password-page section settings configured, which usually means the storefront was (or still is) in password-protected pre-launch mode at the time of export.

## License

All rights reserved. This repository contains proprietary branding, content, and paid app integrations for a specific client's store. It is not licensed for reuse, redistribution, or reference as a template.
