fs-styles
=========
Stylus files used by FamilySearch.org.

# Folder Organization
To help organize a large CSS code base, we have split the files into different folders. Each file is then compiled into `familysearch-styles.styl` which is what is used on the site.
*see [Architecture SASS Project](http://www.sitepoint.com/architecture-sass-project/) and [SMACSS Categorizing](http://smacss.com/book/categorizing) for more details*

Folder   | Contents
---------|---------
Helpers  | Variables, mixins, and functions.
Elements | Default styles applied to an HTML element any time it's used on a page.
Modules  | Groupings of HTML elements that form a reusable component.
Layout   | Styles for content layout such as grids, headers, footers, etc.
Themes   | Theme specific styles (colors, typography, etc.) applied to elements and modules.

# File Organization
A little effort goes a long way. Please take the time to organize your CSS file so that others may quickly find what they are looking for. Divide your code into meaningful sections that denote what the rules are affecting.
*see [CSS Guidelines](https://github.com/csswizardry/CSS-Guidelines) for more details*

## Recommended Guidelines
1. Table of contents at the top of the stylesheet denoting sections
```javascript
/*------------------------------------*\
  $CONTENTS
\*------------------------------------*/
/**
 * CONTENTS..............Section description
 * SECTION-NAME..........Section description
 * ...
 */
```
2. Section headings start with $ to make searching easier (`$SECTION-NAME`)
```javascript
/*------------------------------------*\
  $SECTION-NAME
\*------------------------------------*/
```

# Naming Conventions

## Files
When naming files, `_filename` denotes that the file is only a partial file and should not be compiled into a CSS file. These files are used by other files to create a fully complied CSS file. Examples include `_mixins` which is a list of mixins and has no selectors that would produce a CSS file.

## Class Names
To be determined. Possible considerations are [BEM](http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/) and [SMACSS](http://smacss.com/).