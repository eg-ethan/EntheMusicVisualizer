# ENTHE

A real-time psychedelic music visualizer built on WebGL2 and Web Audio. 29 visual modes driven by your music — all computed from actual neuroscience and mathematics, not pre-made textures or loops. Single HTML file, zero dependencies, no build step.

![WebGL2](https://img.shields.io/badge/WebGL2-single%20file-b48bff?style=flat-square)
![deps](https://img.shields.io/badge/dependencies-ZERO-62e6c9?style=flat-square)
![license](https://img.shields.io/badge/license-AGPL--3.0-black?style=flat-square)
![modes](https://img.shields.io/badge/modes-29-b48bff?style=flat-square)

---

## What it is

ENTHE simulates the visual patterns produced by the brain during altered states — Klüver's four form constants (tunnels, spirals, lattices, cobwebs), reaction-diffusion systems, Kleinian group geometry, elliptic functions, and more — then drives them in real time from your audio.

Everything is computed on the GPU from first principles. The patterns respond to frequency, beat, and drop detection in your music.

---

## Quickstart

Open `index.html` in Chrome or Edge. That's it.

- Press **A** for autopilot, or pick a substance preset to load its visual signature
- Load audio: mic input, a local file, or a browser tab (YouTube, SoundCloud, etc.)
- Press **F** for fullscreen

> Best in Chrome/Edge/Brave — full WebGL2, tab audio capture, and MIDI. Firefox/Safari work minus tab capture and MIDI.

---

## Visual modes

| Category | Modes |
|---|---|
| Cortical / hallucination | Form Constants (Bressloff–Cowan) · Neural Field (Wilson–Cowan) · Entoptic |
| Reaction–diffusion | Turing (Gray–Scott) · Dragonscales · Defect Gas |
| Waves & tilings | Quasicrystal · Cymatics · Pentagrid Loom · Wave Crystal |
| Geometry / fractal | Sacred Geometry · Hyperspace · Hyperbolic · Fractal (Mandelbox) · Indra's Necklace |
| Complex analysis | Weierstrass Wells · Blaschke Rosette · Phase Portal |
| Number theory | Gaussian Halo · Denominator Descent |
| Dynamics & physics | Arnold Tongues · Quantum Orbitals · Vortex Condensate |
| Flow & texture | Particle Flow (50k GPU particles) · Voronoi · Vines · Breathing Walls |
| Instrument | Waveform (polar oscilloscope) · Image Warp |

Any mode can be folded through the 17 crystallographic wallpaper groups (pmm, p4m, p6m, p6) for periodic lattice variations.

---

## Audio features

- 7-band frequency choreography with BPM sync
- Full waveform analysis on file load — drop detection is predictive, not reactive
- 9 drop effects: Wormhole, Supernova, Kaleido Shatter, Negative, Zoom Punch, Glitch, Shockwave, Mandala Burst, Time Echo
- Binaural/isochronic entrainment drone
- MIDI-learn support
- Scene snapshots and autopilot transitions

| Audio source | How |
|---|---|
| Mic | Aim at your speakers |
| File | Drag in a track — full waveform gets analysed upfront |
| Browser tab | Chrome: pick tab + enable "Share tab audio" |
| System audio | Route through BlackHole or Loopback |

> DRM players (Spotify web, Apple Music, Tidal) mute on tab capture — use their desktop app with a loopback device instead. All audio processing is local; nothing leaves your machine.

---

## Substance presets

14 presets map visual signatures to phenomenology by research:
LSD · Psilocybin · DMT · Mescaline · Ayahuasca · 2C-B · Ketamine · Salvia · MDMA · Cannabis · Nitrous · 5-MeO-DMT · Amanita · Ibogaine

Each loads a visual mode combination and runs a timed come-up → peak arc.

---

## Controls

```
space    cycle mode        A    autopilot         F    fullscreen        D    fire drop effect
up/down  dose              K    10 Hz flicker     W    wallpaper lens    V    waveform scope
T        trip arc          B    breath pacer      =    math HUD          R    reseed
1–8      jump to mode      M    audio on          H    hide UI           i    science panel
```

---

## Hosting

It's a static file — host it anywhere:

```bash
python3 -m http.server 8080
```

Works on GitHub Pages, Netlify, Vercel, S3, or a USB stick.

---

## Disclaimer

ENTHE is a visual simulator. It is not medical advice, dosing guidance, or sourcing assistance. The substance presets are artistic interpretations of reported visual phenomenology, not prescriptions.

**Photosensitive epilepsy warning:** the app flickers and pulses. The flicker mode is off by default; reduce intensity or look away if you are sensitive.

---

## Math references

- Bressloff, Cowan et al. (2001) — geometric visual hallucinations and the V1 model
- Ermentrout & Cowan (1979) — Wilson–Cowan neural fields
- Turing (1952) / Gray–Scott — reaction-diffusion; Manukyan et al. (2017, *Nature*) — lizard-scale CA
- Klüver (1966) form constants · Schwartz retino-cortical map · Ottosson OKLab
- de Bruijn (1981) pentagrid · Weierstrass ℘ · Blaschke products · Mumford–Series–Wright *Indra's Pearls*
- Arnol'd circle map · Abrikosov (1957) vortex lattice · ABC flow · Mandelbox

Full bibliography and per-mode equations are in `SCIENCE.md` and the in-app science panel.

---

## License

AGPL-3.0
