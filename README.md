# Sisa Creative CSS Cheat Sheet
Built to be an add on to Bootstrap, this cheat sheet allows for some super simple and powerful CSS classes to be used, making website styling within HTML very very easy!

## Usage

Add the stylesheet to your project within the `<head></head>` tag, then apply classes directly to your HTML elements. Always place as the last linked CSS file so that it can overide other CSS files, like Bootstrap.

Add via remote load:

```html
<link rel="stylesheet" href="https://dev.sisacreative.com/css/v1/sisa-cheat-sheet.min.css">
```
Or download and manually add: 

```html
<link rel="stylesheet" href="/your/path/to/sisa-cheat-sheet.min.css">
```

Example:

```html
<section class="tile w80c text-center pt-3 pb-3">
  <h1 class="f36 mf28 fw700 lh1p2">Welcome</h1>
  <p class="f16 mf14 lh1p5">This is a responsive utility-styled block.</p>
</section>
```

## Font Size

Desktop font-size utilities use the format:

```html
.f{size}
```

Available sizes: `f1` through `f100`.

```html
<h1 class="f48">Large heading</h1>
<p class="f16">Body text</p>
```

Mobile font-size utilities use:

```html
.mf{size}
```

Available sizes: `mf1` through `mf100`.

These apply only on screens up to `600px` wide.

```html
<h1 class="f48 mf32">Responsive heading</h1>
```

There are also inherited mobile font-size reset classes:

```html
.mf-1
.mf-2
...
.mf-100
```

These set:

```css
font-size: inherit;
```

## Font Weight

Use `.fw100` through `.fw900`.

```html
<p class="fw300">Light text</p>
<p class="fw700">Bold text</p>
```

## Text Colour

```html
<p class="text-white">White text</p>
<p class="text-black">Black text</p>
```

Important override versions:

```html
<p class="text-whiteIMP">Forced white text</p>
<p class="text-blackIMP">Forced black text</p>
```

## Line Height

Available classes:

```html
.lh1
.lh1p1
.lh1p2
.lh1p3
.lh1p4
.lh1p5
.lh1p6
.lh1p7
.lh1p8
.lh1p9
.lh2
```

Example:

```html
<p class="lh1p5">Comfortable paragraph line height.</p>
```

## Text Alignment

```html
.text-left
.text-center
.text-right
```

Important override versions:

```html
.text-leftIMP
.text-centerIMP
.text-rightIMP
```

Example:

```html
<div class="text-center">Centered content</div>
<div class="text-right">Right aligned content</div>
<div class="text-left">Left aligned content</div>
```

## Text Shadow

```html
<h1 class="text-shadow text-white">White text with dark shadow</h1>
<h1 class="text-shadowW text-black">Black text with white shadow</h1>
```

## Padding

Desktop padding utilities use `em` units.

All sides:

```html
.p-1 through .p-100
```

Top:

```html
.pt-1 through .pt-100
```

Bottom:

```html
.pb-1 through .pb-100
```

Left:

```html
.pl-1 through .pl-100
```

Right:

```html
.pr-1 through .pr-100
```

Example:

```html
<div class="pt-4 pb-4 pl-2 pr-2">
  Content with spacing
</div>
```

### Mobile Padding

Mobile padding classes apply only below `600px`.

```html
.mp-1 through .mp-100
.mpt-1 through .mpt-100
.mpb-1 through .mpb-100
.mpl-1 through .mpl-100
.mpr-1 through .mpr-100
```

Example:

```html
<section class="pt-6 pb-6 mpt-3 mpb-3">
  Responsive vertical spacing
</section>
```

## Margin

Desktop margin utilities use `em` units.

All sides:

```html
.m-1 through .m-100
```

Top:

```html
.mt-1 through .mt-100
```

Bottom:

```html
.mb-1 through .mb-100
```

Left:

```html
.ml-1 through .ml-100
```

Right:

```html
.mr-1 through .mr-100
```

Example:

```html
<div class="mt-3 mb-3">
  Content with vertical margin
</div>
```

### Mobile Margin

Mobile margin classes apply only below `600px`.

```html
.mm-1 through .mm-100
.mmt-1 through .mmt-100
.mmb-1 through .mmb-100
.mml-1 through .mml-100
.mmr-1 through .mmr-100
```

Example:

```html
<div class="mt-5 mmt-2">
  Smaller top margin on mobile
</div>
```

## Widths

Full and percentage widths:

```html
.w100
.w90
.w80
.w70
.w60
.w50
```

Centered width helpers:

```html
.w90c
.w80c
.w70c
.w60c
.w50c
```

Example:

```html
<div class="w80c">
  Centered block at 80% width
</div>
```

## Borders

Border radius:

```html
.br5
.br10
.br15
.br20
.br25
.br30
.br35
.br40
.br45
.br50
.br55
.br60
```

Border thickness:

```html
.b05
.b1
.b2
.b3
```

Example:

```html
<div class="br20 b1">
  Rounded box with border
</div>
```

## Images

Image utilities:

`.img` to make image full width, `.imgbr` to make image full width with a border radius, `.imgShadow` to add a nice background shadow and keep full width, and `.imgbrShadow` to add a nice background shadow, add full width, and to add a border-radius.

```html
.img
.imgbr
.imgbr05
.imgbr10
.imgbr15
.imgbr20
.imgbr25
.imgbr30
.imgShadow
.imgbrShadow
```

Example:

```html
<img src="image.jpg" class="imgbrShadow" alt="Example image">
```

## Backgrounds

Solid backgrounds:

```html
.bgB
.bgW
```

Background image helpers:

```html
.bgImg
.bgImgC /* Centre the background image */
.bgImgT /* Align the background image to the top */
.bgImgB /* Align the background image to the bottom */
.bgImgL /* Align the background image to the left */
.bgImgR /* Align the background image to the right */
```

Example:

```html
<section class="bgImgC" style="background-image:url('hero.jpg');">
  Hero section
</section>
```

## Z-Index Layers

```html
.zTop
.zMid
.zBot
.zBack
```

Example:

```html
<div class="zTop">Top layer</div>
```

## Tiles

Prebuilt content blocks:

Some nice prebuilt tiles to provide a background context to your content. Super nice to write html with! 

```html
.tile
.tileW
.tileB
.tileG
```

Examples:

```html
<div class="tile">
  Light grey tile
</div>

<div class="tileW">
  White tile
</div>

<div class="tileB text-white">
  Black tile
</div>

<div class="tileG">
  Glassmorphism tile
</div>
```

## Box Shadows

```html
.box-shadow
.box-shadow-thick
.box-shadow-inset
.box-shadowW
.box-shadow-thickW
.box-shadow-insetW
```

Example:

```html
<div class="tile box-shadow">
  Soft shadow card
</div>
```

## Responsive Behaviour

The mobile breakpoint is:

```css
@media only screen and (max-width: 600px)
```

Mobile-specific classes only activate at `600px` or below.

Example:

```html
<h1 class="f56 mf34">Large desktop, smaller mobile</h1>

<section class="pt-8 pb-8 mpt-4 mpb-4">
  Responsive spacing
</section>
```

## Recommended Class Order

For readability, use this order:

```html
<div class="
  w80c
  tile
  pt-4 pb-4 pl-3 pr-3
  mt-3 mb-3
  f16 mf14
  fw400
  lh1p5
  text-center
  box-shadow
">
  Content
</div>
```

Suggested grouping:

1. Layout and width
2. Tile or background
3. Padding
4. Margin
5. Typography
6. Alignment
7. Shadows, borders, extras

## Common Patterns

### Hero Section

```html
<section class="bgImgC pt-10 pb-10 mpt-5 mpb-5 text-center text-white text-shadow">
  <div class="w80c">
    <h1 class="f64 mf38 fw700 lh1p1">Hero Title</h1>
    <p class="f20 mf16 lh1p5">Supporting introduction text.</p>
  </div>
</section>
```

### Card

```html
<div class="tileW br20 box-shadow">
  <h2 class="f28 mf22 fw700 lh1p2">Card title</h2>
  <p class="f16 mf14 lh1p5">Card content goes here.</p>
</div>
```

### Image Card

```html
<div class="tileW box-shadow">
  <img src="image.jpg" class="imgbr mb-2" alt="Example">
  <h3 class="f24 mf20 fw700">Image title</h3>
  <p class="f16 mf14 lh1p5">Image description.</p>
</div>
```

### Glass Tile Over Background

```html
<section class="bgImgC pt-8 pb-8" style="background-image:url('background.jpg');">
  <div class="tileG w70c text-white">
    <h2 class="f36 mf28 fw700">Glass Panel</h2>
    <p class="f16 mf14 lh1p5">Readable text over a blurred glass background.</p>
  </div>
</section>
```

## Notes

- Spacing classes use `em`, so spacing scales with the font size of the element.
- Font-size classes use `pt`.
- Mobile classes are prefixed with `m`.
- Important override classes are suffixed with `IMP`.
- Width classes ending in `c` are centered automatically using side margins.
- This system is best suited for quick page building, landing pages, prototypes, and reusable content sections.

## License

The Sisa Creative CSS Cheat Sheet uses the Apache 2.0 license. It can be used freely in internal or personal projects. Consider getting in touch to showcase how you have used it!
