# Students — MENDELEEV

**Project:** MENDELEEV  
**Category:** CHEMICAL_MANUFACTURING  
**Upstream:** see BENCH.json  
**Pinned commit:** `bd4716bff94c7acf22210d6ffb75dbd1fcc4f9bc`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `6bb3b025826c82d006c38ff83770a93b208780163e1cf2e3f13bf06e98911850`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `bd4716bff94c7acf22210d6ffb75dbd1fcc4f9bc`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `6bb3b025826c82d006c38ff83770a93b208780163e1cf2e3f13bf06e98911850`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
