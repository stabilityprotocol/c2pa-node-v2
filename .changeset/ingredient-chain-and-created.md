---
"@joinmonolith/c2pa-node": minor
---

`addIngredient` with a source asset now both imports the ingredient's manifest
chain (preserving the source's existing C2PA provenance via a linked gathered
assertion) and records a self-authored created `c2pa.ingredient.v3` assertion, so
the ingredient is always represented in `created_assertions` regardless of import
path. The no-asset `addIngredient` overload continues to record the created
assertion only.
