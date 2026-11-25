# Imperiet ApS · visitkort

Hugo-site bare HTML og CSS.

## Ret tekst

Al tekst og alle links står i `content/_index.md`.

- Hver linje i en liste bliver en linje på siden
- `web:` og `mobil:` er de to tekstsæt fra designet
- Store bogstaver styres af CSS. Skriv bare almindeligt

## Ret placering, størrelse og farver

`assets/css/main.css`

- Farver og fonte øverst i `:root`
- Placering pr. boble i designets pixels (web 1200 × 900, mobil 1080 × 1350)
  - `--x` `--y` boblens hjørne
  - `--tx` `--ty` tekstens venstre kant og versaltop
  - `--fs` skriftstørrelse
- Boblerne vokser automatisk, hvis teksten bliver længere

Mobil-layoutet bruges på skærme i højformat og under 600 px bredde.

## Grafik

`assets/svg/` indeholder boblerne og palmen. De bruger `currentColor`, så farven styres fra CSS.

## Byg

```
hugo server        # lokalt
hugo --minify      # til public/
```

Kræver Hugo 0.146 eller nyere (bygget og testet med 0.170.1).

## Fonte

Selvhostede Google Fonts i `static/fonts/`, alle under SIL Open Font License:
Roboto Condensed ExtraBold Italic, Baskervville Italic, Bangers, Boogaloo.
Subsettet til latinske tegn inkl. æ, ø, å.
