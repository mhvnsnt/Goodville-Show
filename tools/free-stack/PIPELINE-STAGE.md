# Pipeline Stage — Goodville-Show

Staged 2026-11-20, branch `tools/free-stack-wireup-20261120` (no merge).
Each tool's exact slot in THIS show's pipeline.

## This repo's pipeline (what already exists)

No pipeline doc lives in this repo — the repo root holds only `AGENTS.md`
and `WORKING-METHOD.md`. The working method: source material is used only
as a construction kit — tools, pipelines, resources, materials,
environments, props, rig systems and conventions — and anything
proprietary (characters, character names, logos or branding) is replaced
with our own original material.

So this show runs a standalone four-stage chain, built from this wire-up:

**Draw → Rig → Composite → Finish**

The tools below ARE the pipeline — there is no existing kit for them to
sit alongside. They compose the same way they do in the other shows
(Tahoma2D spine + Synfig rig/tween + Glaxnimate motion + Kdenlive/Olive
finish), with Grease Pencil (Blender) as the rig/animation core wherever
it is used: these join for cleanup / hand-drawn 2D / compositing / rigging
experiments, NOT as a core replacement unless verified better on our own
shots.

## Stage map — Draw → Rig → Composite → Finish

| Stage | Tool | Slot in THIS pipeline |
|---|---|---|
| Draw | Pencil2D 0.7.2 | Hand-drawn frame-by-frame roughs, timing tests, simple cel cuts — the lightweight TVPaint seat. The pen-first drawing seat of the chain. |
| Draw | Douga build 1116 (Windows-only) | Pen-first cel animation with a real dope sheet (keys, holds, loops, exposure on ones/twos). Free exports carry a small "made with douga.app" watermark. Windows seat; pairs with Pencil2D. |
| Draw | Wick Editor 1.19.0 | Fast Flash-style vector cartoons + interactive/game-like clips (in-editor JavaScript). Desktop builds stale since 2020 — web editor live; quick-sketch seat only. |
| Rig | Synfig Studio 1.5.5 | **Best new pull.** Bone-rigged cut-out characters + automatic vector tweening — the gap-closer. Actively maintained. Rigged characters are the cut-out cast of the chain. |
| Rig | Rigby2D 0.5.1 | 2D skeletal/mesh/IK/physics rigs, JSON/.skel export, game runtimes. The live Spine/Moho cover. GPU route for runs: Kaggle GPU / Colab / Lightning AI / Oracle. |
| Rig | AniCraft 0.2.1 | Clean-room Adobe Animate (Rust, XFL/FLA/SWF per project description). Shape tweens, Bone tool, camera layer; `anicraft-cli` renders headless. FLA-compat test still owed. |
| Rig (spare) | Enve (continuous d919d4d) | **STALE — last push 2022-09-25.** Real vector+rigging seat, kept as a spare/fallback only. Prefer Synfig for anything new. |
| Composite | Glaxnimate 0.6.0 | Motion graphics + Lottie / animated SVG / GIF / WebP. Titles, UI motion — the motion layer composited over the rigged/drawn plates. NOT a character-rigging tool. |
| Composite | (companion) Tahoma2D 1.6.3 | Best overall Harmony equivalent; drawing + Xsheet + compositing spine. Already wired in dream-girl (`tools/tahoma2d/`); pull it in here the same way when the show needs the full production seat. |
| Finish | Kdenlive 26.08.3 | **Primary NLE.** Cut episodes, assemble renders, subtitles, colour, scopes. GPU route for accelerated preview/effects: Kaggle GPU / Colab / Lightning AI / Oracle. |
| Finish | Olive 0.2.0-nightly | Secondary/alpha NLE, node-based experiments + fallback. **PAUSED upstream** — do NOT cut deadline work in it. |

## Get the binaries

```bash
bash tools/free-stack/fetch-verify.sh   # all 10 tools, size + sha256 verified
```

Binaries live on mhvnsnt/dream-girl releases `harmony-equivalents-20261120`
and `production-stack-free-20261120`. Per-tool version, licence, size, and
SHA-256 are in each tool's README under `tools/harmony/` and
`tools/free-stack/`. Licence never gated a pull; licences are logged
honestly next to each item.
