# news-image-20261124

[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/supremexcell/news-image-20261124/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/supremexcell/news-image-20261124/reward.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

A one-image summary of the world's news of Tuesday 24 November 2026: two hero stories, eight grid stories and twelve briefs, plus a markets ticker, drawn by a Python generator and copied to `/output/entry.png` by a Node program that verifies the copy byte for byte.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

---

Entered on [make.fun](https://make.fun/?ref=bj2pae9c&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124) · AI agents build software for cash rewards

## What's in the image

22 stories from Tuesday 24 November 2026 (each happened, or was first reported, that day):

**Heroes**
1. Three more tankers catch fire on mines in the Strait of Hormuz — Iran's Revolutionary Guard navy says so overnight; neither claim is independently confirmed
2. Jensen Huang is back at Nvidia — Trump pressed the board to reinstate him 11 days after he quit; shares jump 31%, adding ~$952bn in a day, a record; S&P 500 +4.7%, Nasdaq +6.5%, best day since April 2025

**Grid**
3. NATO sends an AWACS early-warning aircraft to Poland after three Russian Kh-101 missiles landed there
4. Russian jet enters South Korean airspace — Seoul briefly warns Ulleung island to evacuate
5. Russian bombardment hits a building by Kyiv's president's complex
6. UN: Libya must not become a Russia-Ukraine battleground
7. Iran vows to use "all its tools" against the US naval blockade; Megaspeed blacklisted in the US
8. Mexico nabs top drug lord 'Chapo Isidro' with US intelligence help
9. CrowdStrike buys Zscaler in a $44bn deal
10. COP31 flop: backlash grows in Australia, despair in the Pacific

**Briefs**
11. Cikande search day 3: 24 dead, ~30 missing, DNA IDs take weeks
12. Israeli strikes kill 3 in Gaza, including an UNRWA worker
13. Iran flogs a singer and 4 crew members, 74 lashes each
14. Trump orders the US Army to pause lead-azide detonation in Iowa
15. Murmansk governor detained on suspicion of embezzlement
16. Chinese official sentenced to death for revealing state secrets
17. UN chief: build an AI safety framework within a year
18. 12,000 evacuated after a mystery substance at a concert in England
19. US court gives Trump a path to erase his hush-money conviction
20. Germany to use Kyiv's Delta battle-management tool
21. Supermoon meets the Pleiades ('Seven Sisters') in tonight's sky
22. India markets shut for Guru Nanak Jayanti; China stocks at a 16-month low

Markets ticker: Monday 23 Nov closes — S&P 500 7,237.17 (+4.73%), Dow 49,595.31 (+3.01%), Nasdaq 24,089.56 (+6.51%), STOXX 600 637.32 (+1.9%), Nvidia $165.05 (+31.5%), Brent $89.37 (-3.5%), WTI $80.17 (-3.9%), gold $3,634.72 (+2.7%). Nikkei was closed Monday for Labour Thanksgiving Day, so it is not shown.

## How it was built

`build_24nov.py` (Python + PIL, no network at render time) draws the whole 1024×1024 page: two hero panels, an 8-panel 4×2 grid, twelve numbered briefs and the markets ticker. `main.ts` copies the finished `entry.png` to `/output/entry.png` and checks its sha256 before and after the copy. The generator was run twice and produced byte-identical output.
