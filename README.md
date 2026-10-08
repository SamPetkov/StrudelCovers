# Strudel Covers

Strudel live-coding covers and notation-to-Strudel experiments. Each song has its own folder (or, for an existing independent project, a link).

## Covers

| Song | Project | Status |
| --- | --- | --- |
| **Vildhjarta — Den Helige Anden** | [Strudel arrangement and GP8 converter](./vildhjarta/den-helige-anden/) | Full-score, score-derived transcription; browser sound design needs further auditioning |
| **Aphex Twin — Xtal** | [Xtal-Strudel-Cover](https://github.com/SamPetkov/Xtal-Strudel-Cover) ([`xtal.js`](https://github.com/SamPetkov/Xtal-Strudel-Cover/blob/main/xtal.js)) | Existing independent cover; linked rather than duplicated |

## Den Helige Anden

The [Vildhjarta folder](./vildhjarta/den-helige-anden/) contains a Strudel arrangement derived from a user-supplied Guitar Pro 8 (`.gp`) score, plus a reusable Python GPIF-to-Strudel converter, generated score metadata, and an offline event-scheduler test. The source Guitar Pro file is not included.

To play, paste [`den-helige-anden.js`](./vildhjarta/den-helige-anden/den-helige-anden.js) into the [Strudel REPL](https://strudel.cc/) and press Play. To check score timing offline:

```bash
node vildhjarta/den-helige-anden/tests/runtime_test.cjs
```

For the converter's CLI, source provenance, limitations, playback modes and MIDI channel assignments, see the [song README](./vildhjarta/den-helige-anden/README.md).

## Attribution and scope

Music and original compositions belong to their respective rights holders. These are unofficial learning/transcription projects, not artist-endorsed releases. The repository's software license does not grant rights to the underlying musical works. The Den Helige Anden conversion preserves score-event timing and pitches, but guitar articulations, amp/cabinet tone, slides, bends and final mixing are approximations that require further auditioning.

A MIDI-routing design reference is [Alvaro Cáceres's Meshuggah Strudel cover](https://github.com/alvaro-caceres-munoz/live-coding-metal/blob/main/new-millenium-cyanide-christ/new-millenium-cyanide-christ.js).
