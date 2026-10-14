# Ethics — MENDELEEV

**Project:** MENDELEEV  
**Category:** CHEMICAL_MANUFACTURING  
**Upstream:** see BENCH.json  
**Pinned commit:** `bd4716bff94c7acf22210d6ffb75dbd1fcc4f9bc`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `6bb3b025826c82d006c38ff83770a93b208780163e1cf2e3f13bf06e98911850`  
**Date:** October 2026

## Position

MENDELEEV is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
