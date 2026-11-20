# Kakatua $40.000?! Dikejar Polisi di GTA 6

[![make.fun · gta6-clipper-01](https://make.fun/badge/gta6-clipper-01.svg)](https://make.fun/bounty/gta6-clipper-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)
[![rank](https://make.fun/badge/gta6-clipper-01/fiedysiti/gta6-clipper/rank.svg)](https://make.fun/bounty/gta6-clipper-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)
[![reward](https://make.fun/badge/gta6-clipper-01/fiedysiti/gta6-clipper/reward.svg)](https://make.fun/bounty/gta6-clipper-01?utm_source=github&utm_medium=readme&utm_campaign=gta6-clipper-01)

Entry for [gta6-clipper-01](https://make.fun/bounty/gta6-clipper-01) on make.fun: a GTA 6
clip cut by my AI agent from Windah Basudara's GTA 6 livestream.

## The clip

Jason finds a mystery cockatoo worth $40,000, hides from the police behind a
dumpster at dusk, then walks into the bird-cage yard — and the clip turns to the
viewer: make clips like this with AI and earn money on make.fun.

- Source: Windah Basudara GTA 6 VOD, 17:28–18:12 (kakatua mystery + police chase)
- Cut: 44 seconds, vertical 1080×1920, 30 fps, audio −14.8 LUFS
- Hook text: "KAKATUA $40.000?!" — then the make.fun pitch as an end card:
  "Bikin klip kayak gini pakai AI dan dapat uang di make.fun —
  make.fun/bounty/gta6-clipper-01"
- Made with ffmpeg in the recorded agent session (trim, blur-fill to 9:16,
  drawtext hook + pitch card, loudnorm)

## The video

`VIDEO.json` at the repository root names the public YouTube Short. The video
was published public on YouTube after the bounty opened, its description
carrying the bounty's line and the entrant's play code.

## The program

`main.ts` (Node 22, standard library only) copies `VIDEO.json` to `/output`,
where the gate reads it. That is all it has to do — the video itself is the
entry, and the house reads its views from YouTube.

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

## License

MIT — see `LICENSE`.
