# HEASE 2027 logo kit

Logo option B, "Agent in a harness": a robot agent wearing a harness whose straps form the H of HEASE.
Text in every logo is converted to outlines, so the files look the same without any font installed.

## Which file to use

| Need | File |
|---|---|
| Site header or navigation bar | `svg/hease-logo-compact.svg` (on dark backgrounds: `-on-dark`) |
| Home page hero, posters, slides | `svg/hease-logo-full.svg` (on dark backgrounds: `-on-dark`) |
| Icon on its own (avatars, footers, buttons) | `svg/hease-mark.svg`, `-on-dark`, `-black` or `-white` |
| The name without the icon | `svg/hease-wordmark.svg` |
| Browser tab, home-screen and app icons | everything in `favicon/` |
| Link previews on social media and chat apps | `social/og-image.png` (1200 x 630) |
| Word, PowerPoint, email signatures | the matching file in `png/` (transparent, high resolution) |

Prefer the SVG files on the website. The PNGs are for tools that don't accept SVG.

## HTML snippets

Put the files in `favicon/` at the root of the site, then add this to `<head>`:

```html
<link rel="icon" href="/favicon.ico" sizes="32x32">
<link rel="icon" href="/favicon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="theme-color" content="#0B3C49">
<meta property="og:title" content="HEASE 2027">
<meta property="og:description" content="1st International Workshop on Harness Evaluation and Assessment for Software Engineering, co-located with EASE 2027">
<meta property="og:image" content="https://YOUR-SITE/og-image.png">
<meta name="twitter:card" content="summary_large_image">
```

`og:image` must be a full URL, including `https://`. `favicon.svg` switches to a white robot when the browser is in dark mode.

Logo in a header, sized by height:

```html
<a href="/"><img src="/hease-logo-compact.svg" alt="HEASE 2027" height="40"></a>
```

## Colors

| Name | Hex | Use |
|---|---|---|
| Ink | `#0B3C49` | Robot, text, dark backgrounds |
| Harness red | `#E8503A` | Straps and antenna only |
| White | `#FFFFFF` | Eyes, backgrounds, text on dark |
| Muted teal | `#A9C7CF` | Secondary text on Ink |

## Typography

The logo uses IBM Plex Sans Bold (HEASE) and Medium (2027 and the subtitle). Use IBM Plex Sans for website text to match.
It is free under the SIL Open Font License, and you can load it from Google Fonts.

## Rules of thumb

- Keep clear space around the logo at least as wide as the robot's head.
- Keep the compact logo at least 32 px tall. Below 48 px, use `favicon/favicon.svg`, which drops the antenna and buckle so it stays legible.
- Don't recolor the straps, stretch the logo or put the colored version on busy photos. Use `-white` or `-black` there.
