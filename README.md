# Inclusive Web Design Checklist

Aims to be the **biggest** checklist of inclusive design considerations for the web _ever_. Includes items for accessibility, performance, device support, interoperability, and language. Pull requests welcome!

## Assumed Already Part of Our Process

## Development

- [ ] [Minify CSS and JS, and remove unused/redundant code](https://developers.google.com/speed/docs/insights/MinifyResources)
- [ ] [Use screen reader and keyboard accessible HTML](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)
- [ ] [Compress raster images](https://www.html5rocks.com/en/tutorials/speed/img-compression/)
- [ ] [Optimize SVG path data](https://web-design-weekly.com/2014/10/22/optimizing-svg-web/)
- [ ] [Make sure heading levels describe a logical section/subsection structure](https://webaim.org/techniques/semanticstructure/)
- [ ] Only include heading elements where they introduce sections of content
- [ ] Support 'pinch zoom' (remove `user-scalable=no` if present)
- [ ] Use relative units (`em`, `rem`, and `ch`), especially for font metrics
- [ ] [Make sure styles and scripts are not render blocking](https://csabapalfi.github.io/eliminate-render-blocking/)
- [ ] Use data tables (`<table>`) for data only, not visual layout purposes
- [ ] Make scrollable elements focusable for keyboard users
- [ ] Lazy load large image assets
- [ ] Do not hijack standard scrolling behavior
- [ ] Match semantics to behavior for assistive technology users
- [ ] Move focus between dialogs and the controls that invoked them
- [ ] Provide status and error messages as WAI-ARIA live regions
- [ ] Make sure all content belongs to a landmark element (`<header>`, `<footer>`, `<nav>`, `<main>`, etc)
- [ ] Ensure content is not obscured through zooming (no fixed widths)
- [ ] Make sure data tables wider than their container can be scrolled horizontally
- [ ] [Provide a skip link if necessary](https://webaim.org/techniques/skipnav/)
- [ ] Instead of obstructing users with CAPTCHAs, use [honeypots](https://en.wikipedia.org/wiki/Honeypot_(computing))
- [ ] [Make content easier to find and improve search results with structured data](https://developers.google.com/search/docs/guides/prototype)

### Design

- [ ] [Make sure main body (paragraph) text is no smaller than the default (user agent) size](https://www.smashingmagazine.com/2011/10/16-pixels-body-copy-anything-less-costly-mistake/)
- [ ] Employ well-balanced, highly legible fonts (not too complex or elaborate)
- [ ] Do not use very thin font faces
- [ ] Include only clear, meaningful animations
- [ ] Make sure text and background colors contrast sufficiently
- [ ] Provide large touch 'targets' for interactive elements
- [ ] Make controls look like controls; give them strong perceived affordance
- [ ] Underline links — at least in body copy
- [ ] Avoid pure white or pure black shades
- [ ] Do not rely on color for differentiation of visual elements
- [ ] Use the same design patterns to solve the same problems
- [ ] Make sure controls do not elicit unexpected or jarring behavior
- [ ] Give all form elements permanently visible labels
- [ ] Give grouped form elements group labels
- [ ] Place labels above form elements
- [ ] Do not instate 'infinite scroll' by default; provide buttons to load more items
- [ ] [Avoid justified body text](https://www.w3.org/TR/WCAG20-TECHS/F88.html)
- [ ] [Provide enough spacing between lines of text (`line-height`)](https://www.w3.org/TR/WCAG20-TECHS/C21.html)
- [ ] Ensure primary calls to action are easy to recognize and reach
- [ ] Use well-established, therefore recognizable, icons and symbols

### Content

- [ ] Provide alternative text for salient images
- [ ] Provide `<title>`s that name the site and the specific page
- [ ] Translate / spell out acronyms the first time you use them
- [ ] Label and describe the same things with the same terminology
- [ ] [Avoid all-caps text](https://github.com/humanmade/hm-pattern-library/issues/75)
- [ ] [Ensure that content is written as clearly and simply as possible](https://www.w3.org/TR/UNDERSTANDING-WCAG20/meaning-supplements.html)
- [ ] Provide descriptive captions for figures
- [ ] Use textual labels to make voice activation cues obvious
- [ ] Avoid images of text — text that cannot be translated, selected, or understood by assistive tech

## What We Don't Do

### Development

- [ ] [Install a service worker and cache all applicable assets](https://css-tricks.com/serviceworker-for-offline/)
- [ ] [Use content-based, not device-specific, media queries](http://bradfrost.com/blog/post/7-habits-of-highly-effective-media-queries/#content)
- [ ] Honor requests to remove animation via the `prefers-reduced-motion` media query
- [ ] Provide a `manifest.json` file for identifiable homescreen entries
- [ ] Avoid time constraints where possible; provide a clear warning and option to extend where not possible

### Content

- [ ] [Remove potentially insensitive or uninclusive language (use 'singular they')](http://alexjs.com/)
- [ ] Give video content captions and transcripts
- [ ] Provide transcripts for audio content
- [ ] [Ensure PDF content is accessible (include tags)](https://webaim.org/techniques/acrobat/)
- [ ] Subset fonts to just the characters you need

### Design

- [ ] Provide clear, unambiguous focus styles
- [ ] Do not recreate supported and expected browser behaviors with bespoke scripts
- [ ] Mark invalid fields clearly and provide associated error messages
- [ ] Indicate swipe gesture support clearly, and provide simple tap-based alternatives
- [ ] Warn users of links that have unusual behaviors, like linking off-site, or loading a new tab
- [ ] Ensure keyboard focus order is logical regarding visual layout

## Not Sure We Do

### Development

- [ ] Support Windows high contrast mode (use images, not background images)
- [ ] Apply `alt=""` or `aria-hidden="true"` to decorative images
- [ ] [Honour DNT (Do Not Track) header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/DNT)
- [ ] Ensure states (pressed, expanded, invalid, etc) are communicated to assistive software
- [ ] Ensure disabled controls are not focusable
- [ ] Do not mark up subheadings/straplines with separate heading elements
- [ ] Provide a print stylesheet (single column, with interactive content hidden)

### Design

- [ ] Begin long, multi-section documents with a table of contents

### Content

- [ ] Provide alternatives and/or descriptions for complex visualizations
- [ ] Provide a default language and use `lang="[ISO code]"` for subsections in different languages

### Project Management

- [ ] Do not include third parties that compromise user privacy
