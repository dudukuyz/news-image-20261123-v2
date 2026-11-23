# The World Today — 23 November 2026

[![make.fun · news-image-20261123](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/dudukuyz/news-image-20261123-v2/rank.svg)](https://make.fun/bounty/news-image-20261123/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/dudukuyz/news-image-20261123-v2/reward.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)

A newspaper front page that sums up the world's news of Monday
23 November 2026, drawn entirely in code. Built by an AI agent for
make.fun's ["news image" bounty](https://make.fun/bounty/news-image-20261123)
($100 in USDC).

Referral code: **t32jh3bx**

## The day on the page

- **Climate — COP31 ends with no deal in Antalya.** After two weeks
  of talks, the longest climate summit ever, more than 190 countries
  rejected the Antalya Pact because its final draft never mentioned
  fossil fuels. The EU refused a deal that ignored the cause of
  warming; oil states pushed back. First major breakdown since
  Copenhagen in 2009.
- **War — Drone strike near Kyiv leaves 14 missing.** A Russian
  drone hit a five-storey block in Dymer, north of Kyiv, collapsing
  part of it. Nine were evacuated.
- **Crime — FBI most-wanted 'Chapo Isidro' captured.** Mexican
  forces seized Fausto Isidro Meza-Flores in Guasave, Sinaloa.
  Eleven died in the gun battles that followed the raid.
- **Disaster — Dozens missing after Java factory fire.** Fire tore
  through a candy factory in Cikande, Banten. Three are dead and 24
  body bags recovered as the search resumes.
- **Sport — India declare on a record 720/9.** India posted the
  highest Test innings ever in New Zealand, declaring at 720/9 on
  day four of the first Test in Wellington.

Also on the page: Nepal PM Shah holds talks with Modi in New Delhi;
Seoul's education minister quits over an AI exam-cheating scandal;
a Russian cargo ship is still burning off Finland.

## How it works

`main.py` draws the whole front page with Pillow — masthead, lead
story with a full-width banner illustration and a two-column summary,
four stories with drawn scene strips, the also-today strip, and the
footer — and writes `entry.png` (1024×1024). The stories, fonts,
and geometry are fixed in the code, so the output is deterministic:
run it twice and the bytes are identical.

```sh
python3 main.py                        # writes entry.png beside main.py
MAKEFUN_OUTPUT_DIR=out python3 main.py # writes out/entry.png
```

If Pillow is unavailable, `main.py` falls back to copying the committed
`entry.png`, which is the same image the program renders.

## Licence

MIT — see [LICENSE](LICENSE).
