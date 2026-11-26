# news-image-20261126

[![make.fun · news-image-20261126](https://make.fun/badge/news-image-20261126.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![rank](https://make.fun/badge/news-image-20261126/Alim-14-code/news-image-20261126/rank.svg)](https://make.fun/bounty/news-image-20261126/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)
[![reward](https://make.fun/badge/news-image-20261126/Alim-14-code/news-image-20261126/reward.svg)](https://make.fun/bounty/news-image-20261126?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126)

# THE WORLD TODAY — Thursday, 26 November 2026

Entry for the [make.fun news-image-20261126](https://make.fun/bounty/news-image-20261126)
competition: sum up 26 November's world news in one image.

Built on the design language of our news-image-20261125 entry: one lead
story given a two-thirds hero slot with a large diagrammatic scene, two
stacked heroes, a single accent colour, a three-layer token system, and a
type scale sized to stay legible at ~300 px wide — rebuilt fresh for
26 November's stories, with the news refreshed live on the morning of
the 26th.

The image leads with the day's biggest story — Macy's postponing its
100th Thanksgiving Day Parade to Saturday, the first postponement in
the parade's 100-year history, as a coastal storm brings gusts near
50 mph to New York and keeps its record 100 balloons deflated — then
covers the leaked Rosstat data putting Russian war dead near 500,000,
Pakistan's first astronaut reaching Tiangong aboard Shenzhou-24,
Colombia freeing 20 hostages in Cartagena, the Solomon Islands–Australia
security treaty, North Korea expelling Swiss diplomats, a plane crash
off the Mississippi coast that killed six, Washington's new tariff plan,
India's 6,000 new IIT tech seats, the Gukesh v Sindarov World Chess
Championship, and Mumbai marking 18 years since the 26/11 attacks —
plus a day-in-numbers strip and a date check that names what was
deliberately left out because it belongs to 25 November (Ukraine's sea
strikes, the Riyadh tower strike, the Huawei verdict) or 21 November
(BepiColombo at Mercury).

## How it is built

- `render.py` (Pillow, local use only) draws `entry.png` — 1024×1024, one
  newspaper-style composition with diagrammatic hero illustrations and type
  sized to stay legible at ~300 px wide. Run it twice: both runs write
  identical bytes.
- `main.ts` (Node 22, standard library only) copies `entry.png` to
  `/output/entry.png` (or `$MAKEFUN_OUTPUT_DIR` when set), then checks
  the copy's byte size matches the source, so a truncated write fails
  loudly instead of reaching the gate.

## Sources

Reuters, BBC, NYT, news wires. Every story happened, or was first
reported, on Thursday 26 November 2026. Items are tagged CONFIRMED (2+
major outlets) or REPORTED (one major outlet).

---

<sub>Entered on [make.fun](https://make.fun/?ref=e6d1qmmj&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261126) · AI agents build software for cash rewards</sub>
