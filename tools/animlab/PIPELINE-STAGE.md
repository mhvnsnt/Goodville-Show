# AnimLab pipeline stage — Goodville-Show

Staged 2026-11-20 on branch `tools/animlab-wireup-20261120` (AnimLab wire-up, binaries UNFETCHED — see
`tools/animlab/README.md`).

## Where AnimLab slots in

No pipeline doc exists in this repo as of 2026-11-20 (only AGENTS.md / WORKING-METHOD.md at root). AnimLab therefore defines its own standalone stage here: Draw -> Rig/Tween -> Composite -> Finish. Vector drawing, Bone/Game Bone/Curve/Envelope rigging and tweening, node-graph compositing, multi-camera timeline, audio mixer, MP4/PNG export — for Goodville 2D animated content. If a pipeline doc is added later, this stage slots into it at the Draw/Rig/Composite position.

## Stages AnimLab covers (for this show)

1. **Draw** — vector drawing, pegs.
2. **Rig/Tween** — Bone / Game Bone / Curve / Envelope rigging, tweening.
3. **Composite** — node-graph compositing, multi-camera timeline, audio mixer.
4. **Finish** — MP4 / PNG export.

## What AnimLab does NOT do here

- It does not replace this show's existing core pipeline or its locked rules.
- It does not ship unproofed: AnimLab output goes through the same own-eyes / proof
  gate as every other stage before it reaches the owner.
- Binaries are UNFETCHED as of 2026-11-20 (itch 429). Until `fetch-animlab.sh` lands
  them on Release `animlab-v0.2.26`, this stage is docs + fetch route only.
