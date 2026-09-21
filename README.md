# Lucky A.I. data

The public files the Lucky A.I. app reads. Nothing here is private: it is lottery results and our own scoreboard.

- `index.json` latest draws, light history, and the lock for the next draw
- `draws/{game}/{year}.json` winning numbers and the full prize breakdown for every draw
- `picks/{game}/{date}.json` **The 5,000**, locked BEFORE the draw: the recipe and a SHA-256 fingerprint of all
  5,000 sets. The commit time of that file is the proof the sets were fixed in advance.
- `pool/{game}/{year}.json` what The 5,000 would have won, per draw, per strategy
- `ledger.json` the scoreboard totals

Games: `lmax` = Lotto Max, `six49` = Lotto 6/49. Not affiliated with any lottery corporation; always check
real tickets with the official lottery.
