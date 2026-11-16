# jah-n-wiki-leaks-shard-2

Data shard for JAH-N Wiki Leaks. Holds sealed bizarre-dossier chunks
(`data/bizarre/chunks/biz-cNNNNNN.json.gz`) plus the search index the main
leaks page loads (`data/bizarre/bizarre.idx.json.gz`).

This repo is frozen storage: the main site's page fetches from it directly.
New dossiers always land in the main repo; when the main repo nears its size
guard, more chunks move to a newer shard.

Moved here 2026-11-16: chunks biz-c000001–biz-c000400 (100,000 dossiers,
JAH-LEAK-B0121–JAH-LEAK-B099890). See data/bizarre/move-manifest.json.
