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

## UI-Theme: Titel-Schriftart Cinzel (Übernahme-Manifest R3-1, Felix-Freigabe 2026-07-12)

Andere Quelle als die übrigen Einträge dieser Datei: `assets-src/fonts/cinzel/Cinzel.ttf`
(Variable Font, Achse `wght` 400–900, Copyright 2020 The Cinzel Project Authors, Designer
Natanael Gama, SIL Open Font License 1.1 — Lizenz-Metadaten direkt aus der TTF-`name`-Table
ausgelesen, siehe `.meta.json`-Sidecar am Quellpfad; auch auf Google Fonts verfügbar), selbst
kopiert aus dem **read-only MVP-Ordner** `/Users/felixhannibal/Verstecken Spiel/assets/fonts/
Cinzel.ttf` (Übernahme-Manifest §4, Posten R3-1). Abgeleitetes Derivat (Asset-Budget-Disziplin
Regel 8 — das Spiel lädt NIE die Master-Datei): `fonts/cinzel-latin.woff2`, erzeugt mit
`fonttools`s `pyftsubset` (Subset auf Basic Latin + Latin-1 Supplement + Latin Extended-A +
allgemeine Interpunktion `U+0000-00FF, U+0100-017F, U+2000-206F`, `--flavor=woff2`,
Variable-Font-Achse erhalten) — `125.468` Byte Master → `41.608` Byte Derivat.

**Abnahme-Status: von Felix abgenommen 2026-07-12** (Felix-Mensch-Gate, Regel 8). `status` im
`.meta.json`-Sidecar am Quellpfad steht jetzt auf `"abgenommen"` (`abgenommen_am: "2026-07-12"`) —
Einsatz im Client ist verdrahtet (`apps/client/index.html`, `@font-face`).

| Datei | Asset-ID | sha256 | Quell-Status |
|---|---|---|---|
| `fonts/cinzel-latin.woff2` | `fonts.cinzel` (Derivat) | `5ed9f580d5621b350182e473be350bad07f91d1c8037fc1d40aac36f1a9f0c9c` | abgenommen |

## Dash-Animation + statisches Steh-Sprite (Felix-Freigabe Playtest 2026-07-11)
- `characters/zauberschuelerin/dash_start_<richtung>.webp` (8) — Quelle `assets-src/.../ludo_output/dash_start/<richtung>/spritesheet.webp` (Provenienz ludo, Status assets-src bleibt „vorschlag" bis Live-Sichtung). One-Shot-Dash-Animation.
- `characters/zauberschuelerin/stand_<richtung>.png` (8) — Quelle `assets-src/.../cut/zauberschuelerin_walking_<richtung>.png` (64×96, Provenienz gpt), von mir transparent auf 128×128 gepaddet (Füße auf Sprint-Origin 0.8 ausgerichtet, Offset 32/6) als Drop-in-Steh-Sprite. „Das normale Sprite" für Stillstand (Felix-Entscheid 2026-07-11: statisches Steh-Sprite statt Idle-Animation).

## Portal-Endgame: Sounds + Vortex-Animation (Felix-Auftrag 2026-07-13)

Alle drei von Felix extern erzeugt (ElevenLabs / ludo.ai), Status in `assets-src` bleibt `vorschlag`
bis zur Live-Sichtung/Hörprobe. **Freigabe Einsatz im Spiel: Felix-Auftrag 2026-07-13.**

- **Summen** (`audio/portal-summen/portal-summen.m4a`, ElevenLabs, Original `a_buzzing_magical_po_#2…mp3`):
  Dauer-Summen-Loop (16 s), das jedes aktive Flucht-Portal positional in einem Radius **über einen
  Raum hinaus** (`PORTAL_SOUND_RADIUS_UNITS = 20`) abgibt. Mono-AAC (`afconvert -f m4af -d aac -b 96000 -c 1`,
  Stereo-Master → Mono für positionalen Sound), ~195 KB.
- **Wirbel** (`audio/portal-wirbel-aktivierung/portal-wirbel-aktivierung.m4a`, ElevenLabs, Original
  `Swirling_vortex_of_i_#4…mp3`): One-Shot beim erfolgreichen Escape (Portal-Aktivierung), positional
  für alle in Reichweite; löst das Verstummen des Summen-Loops aus. Mono-AAC, ~36 KB.
- **Vortex-Animation** (`effects/portal-vortex/portal-vortex.webp`, ludo.ai, Original
  `sprite-max-px-frames-16-rows-4-cols-4`): dauerhaft laufende Portal-Darstellung (ersetzt den
  Platzhalter-Ring). Master-Sheet 1184×2088 (16 Frames 296×522, 232 ms/Frame ≈ 3,7 s Loop). Derivat
  aus den 16 EINZEL-Frames gebaut (Pillow, LANCZOS — kein Frame-Bleed): je auf 96×168 skaliert, als
  uniformes 4×4-Atlas (384×672) gepackt, **verlustfreies WebP VP8L** (~379 KB, budget-konform,
  projektüblich). Effekt-Budget dafür von 128 auf 512 KB angehoben (siehe `asset-budgets.json`).

| Datei | Asset-ID | Master-sha256 | Derivat-sha256 | Quell-Status |
|---|---|---|---|---|
| `audio/portal-summen/portal-summen.m4a` | `audio.portal-summen` | `47674043c0d3efb96df6e4a02cab236e3ab0d6f4ab0a3a4168c0ab1b6878a869` | `8f02d9425f35faa7633eb724abfd91f4a480b26df3b0e9c438663683890bd380` | vorschlag |
| `audio/portal-wirbel-aktivierung/portal-wirbel-aktivierung.m4a` | `audio.portal-wirbel-aktivierung` | `92ae0d82dc754482071fb5bc5de8586fff7c3696b6b56ccec0b05dbe74cf10ea` | `e1109f0d0b7881ceb35fa32f9694e02a62ac24342182d86f563847616066e891` | vorschlag |
| `effects/portal-vortex/portal-vortex.webp` | `effects.portal-vortex` | `4cc7156ad793dc92a446bd27992217acb929aaa6816dd692054ed914c33fb32d` | `3f240a40b9c3798734403a3b19cf69a579993e6f7ec42c3660f941c375b8a3c2` | vorschlag |
