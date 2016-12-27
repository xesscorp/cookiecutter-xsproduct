Modifications to [Jekyll documentation theme](http://idratherbewriting.com/documentation-theme-jekyll/index.html)
-------------------------------------------------------------------------------------------------------------------

 1. Place site-wide stuff (product name, version, etc.) into the `_config.yml` file.
 1. New manual sections are stored in the `pages` directory.
 1. Images are placed in the `images` directory.
 1. Place a `schematic.pdf` file (if applicable) in the `misc` directory.
 1. Navigation to manual sections is specified in `_data/sidebars/manual_sidebar.yml`.
 1. Make sure `manual_sidebar` is referenced in `_includes/custom/sidebarconfigs.html`.
 1. Place a link to the schematic in the README at the top of the repo.
 1. Feedback email is configured in `_includes/feedback.html`.
 1. Main theme color is specified in `css/theme-xess.css`.
 1. Product name in top navigation bar is set in `_includes/topnav.html`.
 1. Summary and in-page TOC are disabled in `_layouts/page.html`.
 