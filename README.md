# rigmeshy-by-ricky

A [Claude Code](https://claude.com/claude-code) skill that teaches Claude how
to get clean, animation-ready character rigs out of **Meshy AI**'s Auto-Rig —
and what to do when a rig comes out broken.

It bundles:

- The ideal reference photo checklist (T-pose vs A-pose, framing, lighting)
- The full Image/Text-to-3D → Auto-Rig → export workflow
- A troubleshooting table for the most common rigging failures (collapsing
  shoulders, fused fingers, asymmetric deformation, floating models)
- A pointer to [UniRig](https://github.com/VAST-AI-Research/UniRig), a free,
  self-hosted, open-source alternative for batch/offline rigging

Claude uses this automatically whenever you ask it to rig a character in
Meshy, prep a reference photo for a 3D model, or set up a self-hosted
auto-rigging pipeline — no need to invoke it by name.

## Install

Drop the `meshy-pose-rigging/` folder into your skills directory:

**User-wide** (available in every project):
```bash
cp -r meshy-pose-rigging ~/.claude/skills/
```

**Project-only:**
```bash
cp -r meshy-pose-rigging /path/to/your/project/.claude/skills/
```

Claude Code picks it up automatically — no restart or registration step
needed.

## Why

Most bad Meshy rigs trace back to the source photo or mesh, not the rig step
itself (arms pressed against the torso, hard shadows, wrong camera angle).
This skill front-loads that knowledge so Claude steers you toward a good
input instead of debugging a broken skeleton after the fact.

## License

MIT — see [LICENSE](LICENSE).
