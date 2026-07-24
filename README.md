# Inside the LHC — a proton's-eye walkthrough

A first-person browser ride through CERN's Large Hadron Collider, on the path a
proton actually takes: injected into the 27 km ring, bent by superconducting
dipole magnets, accelerated by RF cavities to 6.8 TeV, and steered into a
collision inside the ATLAS detector.

Part of the BYU TTO "places a student can't physically go" demo series.
Three.js, single static page, no build step, no backend, no login.

## Run locally
```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy
Static — deploys as-is to Vercel (no framework, no build command).

## Real substrate
Captions use real LHC figures: 27 km ring, ~100 m underground, 1,232 dipole
magnets at 1.9 K, ~11,245 revolutions/second, 6.8 TeV per beam / 13.6 TeV
collision energy, ATLAS/CMS/ALICE/LHCb interaction points. Exact Run-3 figures
verified at build.

## Status
- [x] On-rails first-person ride (demo path)
- [x] Material realism pass (PBR magnets/tunnel + HDRI reflections)
- [x] Free-roam mode (drag-to-look + WASD fly)
- [x] Distinct components: dipoles, RF cavities, quadrupoles, beam pipe, ATLAS
- [x] Component labels in free-roam (name + one-line description)
- [x] Collision hero shot: held, drag-to-orbit, multi-colour spray, replay
