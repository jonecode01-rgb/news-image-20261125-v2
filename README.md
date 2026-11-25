# Wednesday 25 November 2026 — the world in one image

A code-rendered dense broadsheet summing up the world's news of
Wednesday 25 November 2026: **36 stories across 6 regions**, each one
verified against Reuters, AP, AFP, BBC, Al Jazeera, The Times, Daily
Trust, SCMP, WSJ, UKHSA, WHO or PTI reporting.

## What is in the image

- **3 hero stories**, each with a flat vector illustration: the WHO pulling
  its Ebola teams out of a hospital in DR Congo (5,775 dead); Australia
  signing a security pact with the Solomon Islands; a 15-year-old,
  Vaibhav Sooryavanshi, hitting 204 off 53 balls for India A in Doha.
- **10 secondary stories** with icons: the CIA's unclassified system
  hacked, the US seeking answers on Nvidia chip sales to China, the Army
  blowing up 5 tonnes of explosives in Iowa, a Pakistani astronaut bound
  for China's Tiangong station, Shanghai party chief Chen Jining probed,
  all hostages freed in Cartagena, a record 5,200 heat deaths in England,
  Britain sanctioning the Houthis, the Bangladesh garment wage up 36%,
  and Kyiv vowing to keep sinking Russian ships.
- **23 more stories** in the "ALSO ON" list, a dotted world map with
  numbered pins, a "THE DAY IN NUMBERS" stat strip, a UTC timeline,
  certainty tags on every story (CONFIRMED / OFFICIAL / REPORTED /
  CLAIM / ONGOING) with a legend, and a footer source list.
- A **DATE CHECK** strip naming the near-miss stories from other days
  that were deliberately left out: Huang rehired (Mon 23 Nov), Huang's
  apology (Tue 24 Nov), the Houthi strike on Riyadh's PIF Tower
  (Tue 24 Nov), Huawei's Brooklyn conviction (Tue 24 Nov), the turkey
  pardons (Tue 24 Nov), the COP31 collapse (Sun 22 Nov), the
  Villavicencio car bomb (Mon 23 Nov), and Senegal's AFCON title
  restored (Tue 24 Nov).

## How it was made

`render.py` draws the whole broadsheet with PIL (no image model, no
photographs): the layout, the three flat hero illustrations, the small
story icons and the dotted world map (from public-domain Natural Earth
country outlines) are all code. `main.ts` copies the rendered
`entry.png` to the output directory; two runs write identical bytes.

## Run

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`entry.png` is 1024x1024, 214,061 bytes, sha256
`deed2be0d91a0f496a3e4157c8e2ff2eadf6fec800856e8b00f3f57665549dea`.

## Licence

MIT — see LICENSE.
