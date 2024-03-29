---
layout: layouts/right
title: Header
tags: pattern
summary:

---

## Design
{% include 'patterns/header/header.md' %}

### Extended header
{% include 'patterns/header/header-ext.md' %}

Please note that mega menus were not added to the library. Even though this pattern exist in the USWDS, megamenus have usability and accessiblity issues. They are also becoming old fashion. See more about this from [NNGroup](https://www.nngroup.com/articles/mega-menus-work-well/). However, if the solution for you web properity needs a mega menu, the code and specifications can be found on the [header spec](https://designsystem.digital.gov/components/header/) for the USDWS.  

## Theme Settings
These aspects of the header can be set within the theme settings.
- __$theme-header-font-family__  _default: ui_
{: .usa-list}
- __$theme-header-logo-text-width__ _default: 33%_  Width of the logo text area at desktop width as a percentage of the total header width.
{: .usa-list}
- __$theme-header-max-width__ _default: destop_ Maximum width of the header.
{: .usa-list}
- __$theme-header-min-width__ _default: desktop_ - smallest breakpoint before showing mobile menu
{: .usa-list}

For this library we've set the `$theme-header-max-width` to "widescreen", to fit with our [Grid](/library/styles/grid) strategy.

All other aspects to brand the header will have to be overwritten using CSS.

## Search Widget
Please see the [search](/library/patterns/search) documentation for more information on how search works in the header (note, this is not functional out of the box)

## Nex+ Library prototyping notes
The library and prototype use the same header which is set in the `_layouts/base.html` file. At default it's using the regular partial header, this can be updated to use the extended header by changing `header.md` to `header-ext.md`.

The navigation for the library is in `_data/lib-nav.yml` and for the prototype in `_data/nav.yml`. Settings for the logo and site name are in the `_data/settings.yml` file.

