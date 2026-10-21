# Watchman Pets

Optional pets for [Watchman](https://github.com/incordai/Watchman)'s break strip
and runner. Watchman itself ships only its own pet, Kai. These are kept here,
apart from Watchman, and are downloaded only by people who choose to, from
Settings › Appearance › Pet.

## Third-party notice — please read

**The pets in this repository are third-party works and likenesses. They are
not made, owned, licensed or endorsed by Incord or by Watchman.**

- Several depict characters owned by others (for example from *Dragon Ball*,
  *Genshin Impact*, *Crayon Shin-chan*, *Chiikawa* and *Goddess of Victory:
  NIKKE*). Those characters and their names belong to their respective owners.
- Several are caricatures of real people. They are fan art, not statements by
  or about those people, and imply no endorsement.
- They are shared as fan-made pets for **personal, non-commercial use only**.
  No rights in the underlying characters, names or likenesses are granted by
  this repository, and none are claimed.
- **You choose to download and use them, at your own discretion.** If you are
  a rights holder and want a pet removed, open an issue and it will be taken
  down.

## Layout

- `catalog.json` — every pet: its id, name, description, sheet path, size and
  SHA-256. Watchman reads it and checks each download against the hash.
- `pets/<id>/pet.json` and `pets/<id>/spritesheet.webp` — one pet. Every sheet
  uses the same grid as Kai: 8 columns by 9 rows of 192 × 208 frames
  (1536 × 1872), one animation per row.

## Adding a pet

Add `pets/<id>/` with both files on Kai's grid, then add its entry to
`catalog.json` with the sheet's size in bytes and its SHA-256.
