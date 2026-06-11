# PokeDoGam Animated Assets

This repository stores remote animated Pokemon GIF files for the PokeDoGam app.

## URL Pattern

The app downloads high-quality animated files by Pokemon number:

```text
https://raw.githubusercontent.com/woozy-A/pokedogam-assets/main/animated/025.gif
```

## Folder Layout

```text
animated/
  001.gif
  002.gif
  003.gif
  ...
  1025.gif
```

Current coverage:

- Primary GIFs: most Pokemon from `001.gif` through `1025.gif`
- Bonus local-style GIFs are kept when available, such as `001-1.gif`
- Missing animated GIFs fall back in the app to Pokemon Showdown and then PokeAPI official-artwork PNG.

Known missing primary GIFs:

```text
990, 991, 992, 993, 994, 995,
1001, 1002, 1003, 1004, 1006, 1008, 1010,
1014, 1015, 1016, 1017,
1022, 1023, 1024, 1025
```

## App Fallback Order

The app does not depend on this repository as its only image source.

1. App bundle `AnimatedAssets`
2. Local high-quality cache
3. This GitHub repository
4. Pokemon Showdown animated sprite fallback
5. PokeAPI official-artwork PNG fallback

## Notes

These files are intended for the PokeDoGam TestFlight/study workflow.
Review asset rights before any public App Store distribution.
