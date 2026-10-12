# arj-social-kort

Bilder till ARJ Distributions sociala inlägg.

## Vad repot är till för

Metricools API tar bara emot bilder via **publik adress** — det går inte att skicka en fil. Det här repot är den publika adressen.

Flödet, som körs av den schemalagda uppgiften *Veckans inläggsidéer till Metricool*:

1. Kortet renderas som PNG (mall och skript finns i Claude-projektet *ARJ Distribution*, dokumentet `rutiner/metricool-inlagg.md`).
2. PNG:en committas hit, under `kort/`.
3. Adressen `https://raw.githubusercontent.com/janssonroger-art/arj-social-kort/main/kort/<fil>.png` skickas som `media` när utkastet skapas.
4. **Metricool hämtar hem bilden och lägger den på sitt eget CDN** (`static.metricool.com`). Utkastet pekar därefter dit, inte hit.

## Repot är en hållplats, inte ett arkiv

Steg 4 är poängen. Bilden behöver bara vara nåbar i sekunden då utkastet skapas. När Metricool väl hämtat den kan filen tas bort härifrån utan att utkastet påverkas — det är verifierat: testbilden som användes när flödet provades 12 oktober 2026 är borttagen, och utkastet den skapades till har sin bild kvar.

Rensa därför gärna `kort/` med jämna mellanrum.

## Varför publikt

`raw.githubusercontent.com` kräver token för privata repon, och en token kan Metricool inte använda. Innehållet är bilder som ändå ska publiceras på Facebook, så det är inget som döljs.

**Lägg inget annat här.** Inga kunduppgifter, inga priser, inga interna dokument. Bara bilder avsedda för publicering.

## Namngivning

`kort/<ÅÅÅÅ>-v<vecka>-<kort-beskrivning>.png` — till exempel `kort/2026-v42-ews-avveckling.png`.

Format enligt rutinen: 1080 × 1080 för Facebook och Instagram, 1200 × 630 liggande.
