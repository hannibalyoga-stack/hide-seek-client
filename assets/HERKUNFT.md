# Herkunft der Assets unter `apps/client/public/assets/`

Provenienz-Nachweis für alle in `apps/client/public/assets/` kopierten Binärdateien (Felix-
Auftrag 2026-07-10). Quelle je Datei ist der Hauptbaum `/Users/felixhannibal/Projekt_Hide_Seek/`
(**read-only**, nie beschrieben) — Asset-ID + `sha256` sind aus dem jeweiligen `.meta.json`-
Sidecar am Quellpfad übernommen und im Worktree per `shasum -a 256` gegen die kopierte Datei
geprüft (Ergebnis: alle unten gelistet Dateien stimmen exakt überein). Die Sidecars selbst
wurden dabei nicht angefasst.

## Charaktere: Zauberschülerin — Sprint-Sprite (8 Richtungen)

Quelle: `assets-src/characters/zauberschuelerin/ludo_output/sprint/<richtung>/spritesheet.webp`
(Ludo.ai, Motion-Transfer-Preset „sprint", 384×384 px, 3×3-Grid = 9 Frames à 128×128 px,
transparent freigestellt).

**Freigabe Playtest-Einsatz: Felix 2026-07-10** (Status in `assets-src` bleibt `vorschlag` bis
zur Live-Sichtung — die Freigabe gilt für den Playtest-Einsatz im Client, nicht als
Endabnahme des Kunst-Assets selbst).

| Datei | Asset-ID | sha256 | Quell-Status |
|---|---|---|---|
| `characters/zauberschuelerin/sprint_south.webp` | `characters.zauberschuelerin.ludo.sprint.south` | `cde0460658655694609f46c059e4fdc4bcd47668f196ab0da64dc65f9ec31605` | vorschlag |
| `characters/zauberschuelerin/sprint_south_east.webp` | `characters.zauberschuelerin.ludo.sprint.south_east` | `8f90f5b0dcb476e9739eb7ed461d7f9ff41accded695724b808094c33a409a18` | vorschlag |
| `characters/zauberschuelerin/sprint_east.webp` | `characters.zauberschuelerin.ludo.sprint.east` | `cdb3a9711025116e7088b14436d5e3d2a261b7ddf1d2cff40dd8070964750ef9` | vorschlag |
| `characters/zauberschuelerin/sprint_north_east.webp` | `characters.zauberschuelerin.ludo.sprint.north_east` | `356548c63979fe6d52f142c7b6b360b20806266ecd71ea7c1ea4c0a78f24fa01` | vorschlag |
| `characters/zauberschuelerin/sprint_north.webp` | `characters.zauberschuelerin.ludo.sprint.north` | `fcfb13fce47913be87fca8974447cddb09bfc56e3a9c4345c047c8800f2fd9e9` | vorschlag |
| `characters/zauberschuelerin/sprint_north_west.webp` | `characters.zauberschuelerin.ludo.sprint.north_west` | `410012e3160131f3025a2c2f3986cc58a0e833ad42d7248f92aaf0ea23a09dd3` | vorschlag |
| `characters/zauberschuelerin/sprint_west.webp` | `characters.zauberschuelerin.ludo.sprint.west` | `35aa6c89896892b5f051eb11c7f049a27591272a7c1a9d93bb9a3a26065eb451` | vorschlag |
| `characters/zauberschuelerin/sprint_south_west.webp` | `characters.zauberschuelerin.ludo.sprint.south_west` | `6f673fb32a4c3621c9904c45886cffdccde2b23b2cd958fdaaaabce26cc97d6c` | vorschlag |

## Audio: Schritt-Geräusche Verstecker (Laufen + Schleichen, je 5 Round-Robin-Takes)

Quelle: `assets-src/audio/schritt-laufen-verstecker/` bzw. `assets-src/audio/schritt-schleichen-
verstecker/` (ElevenLabs). Je Verzeichnis `-v3.mp3` = abgenommener Referenz-Take, `-t2`…`-t5` =
zusätzliche Round-Robin-Varianten desselben Klangbilds — `apps/client/src/audio/
footstepSamples.ts`s `selectRoundRobinSampleIndex` wählt bei jeder Wiedergabe zufällig einen der
5 Takes, nie denselben zweimal direkt hintereinander.

**Freigabe Einsatz im Spiel: Felix 2026-07-10** (Status der `-t2`…`-t5`-Takes in `assets-src`
bleibt `vorschlag` — nur `-v3` ist bereits `abgenommen`; die Freigabe gilt für den Einsatz als
Round-Robin-Pool im Client, nicht als Einzel-Endabnahme jedes Takes).

| Datei | Asset-ID | sha256 | Quell-Status |
|---|---|---|---|
| `audio/schritt-laufen-verstecker/schritt-laufen-verstecker-v3.mp3` | `audio.schritt-laufen-verstecker-v3` | `88089f7d84e3ad9cafcbd025f3a0909d987a1d4ad789a9826080c9116817e1b9` | abgenommen |
| `audio/schritt-laufen-verstecker/schritt-laufen-verstecker-t2.mp3` | `audio.schritt-laufen-verstecker-t2` | `c85c0adb9f49f4b4c0fa83031c9e59ac3906af7ca9fff31279f6fa247d3bd94d` | vorschlag |
| `audio/schritt-laufen-verstecker/schritt-laufen-verstecker-t3.mp3` | `audio.schritt-laufen-verstecker-t3` | `a1ebeb4653c76f543a4aeb06ae6a352743671afee1bae43ded917edd3fc01ce6` | vorschlag |
| `audio/schritt-laufen-verstecker/schritt-laufen-verstecker-t4.mp3` | `audio.schritt-laufen-verstecker-t4` | `66b680eeff72aea78b1a0c7b1c6f09c79d179568f67ec48b7cce87098b7dfb2f` | vorschlag |
| `audio/schritt-laufen-verstecker/schritt-laufen-verstecker-t5.mp3` | `audio.schritt-laufen-verstecker-t5` | `c1dd1575469bd4d55149d8453d3b3168fa659373a5b685f7a032d06e40cc701b` | vorschlag |
| `audio/schritt-schleichen-verstecker/schritt-schleichen-verstecker-v3.mp3` | `audio.schritt-schleichen-verstecker-v3` | `c9296fcdfcce8b05494cda4c96cfc9413ed7e4b715232d857ff710c58b88677d` | abgenommen |
| `audio/schritt-schleichen-verstecker/schritt-schleichen-verstecker-t2.mp3` | `audio.schritt-schleichen-verstecker-t2` | `f7eaabae724cc096a61a578236dcb1ccb477494d2da4902aef24b4ae5d269cd8` | vorschlag |
| `audio/schritt-schleichen-verstecker/schritt-schleichen-verstecker-t3.mp3` | `audio.schritt-schleichen-verstecker-t3` | `59a4f30a0749b5dc8a73f3f8ec2a2b161a5ff23dfa9fb848ab8a168801a3291c` | vorschlag |
| `audio/schritt-schleichen-verstecker/schritt-schleichen-verstecker-t4.mp3` | `audio.schritt-schleichen-verstecker-t4` | `b04ea5585d78e48469a0e8b8f35a63edbf8dbaf3466ff447d76479eb82b1bddf` | vorschlag |
| `audio/schritt-schleichen-verstecker/schritt-schleichen-verstecker-t5.mp3` | `audio.schritt-schleichen-verstecker-t5` | `5f42f6be509e9dfa802d161858c17fbb93c78eb67a3ee3ba97c57fd6f01c2911` | vorschlag |

## Dash-Animation + statisches Steh-Sprite (Felix-Freigabe Playtest 2026-07-11)
- `characters/zauberschuelerin/dash_start_<richtung>.webp` (8) — Quelle `assets-src/.../ludo_output/dash_start/<richtung>/spritesheet.webp` (Provenienz ludo, Status assets-src bleibt „vorschlag" bis Live-Sichtung). One-Shot-Dash-Animation.
- `characters/zauberschuelerin/stand_<richtung>.png` (8) — Quelle `assets-src/.../cut/zauberschuelerin_walking_<richtung>.png` (64×96, Provenienz gpt), von mir transparent auf 128×128 gepaddet (Füße auf Sprint-Origin 0.8 ausgerichtet, Offset 32/6) als Drop-in-Steh-Sprite. „Das normale Sprite" für Stillstand (Felix-Entscheid 2026-07-11: statisches Steh-Sprite statt Idle-Animation).
