# Strike accounts replaced by codes (23 Oct 2026)

Two pre-record files held Strike account ids as Strike's discover and lead-trader lists return them. TUG never lists
Strike traders one by one, so before this repository was made public each Strike account id became a salted code
(s-<16 hex>), each Strike wallet address a code (w-<16 hex>), and handles, names and avatar links were removed. These
are the same codes the hourly records use. Hyperliquid data and every other file are unchanged.

The 7-day figures are identical before and after. `python3 -I stats_7d.py .` prints:
top-250 copy picks: active on Strike markets 93, gained 71; fade picks: active on Strike markets 100, lost 74.
They are computed from Hyperliquid fills; the Strike rows only feed the crowd lists.

| File | SHA-256 recorded on 22 Oct (original) | SHA-256 now |
|---|---|---|
| discover_all.json.gz | eae974d679f85512bbd75d41ce45772581fddbca50a483dc1418f5c6b3af039c | ac20bad5afcbd3e627bd7e5e29aed4f9425492aa5f9ac4809fd06216ae1f173d |
| lt.json | 85b918774bd35202e26f82bc6cc6d90f00950b92910a8463cad70166454363a0 | 383d4d4741ed318b3d11f0f2f151b16b3ff3d97870ed2427c2cabfd7d773dd48 |

Every other file keeps the SHA-256 recorded on 22 Oct (MANIFEST.sha256).
