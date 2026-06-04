---
"@joinmonolith/c2pa-node": patch
---

Fix `addIngredient` with a source asset emitting two `parentOf` ingredients
(`manifest.multipleParents`). The imported chain already records a `parentOf`
gathered ingredient, so the additional created `c2pa.ingredient.v3` assertion is
now forced to `componentOf`, leaving a single declared parent while still
representing the ingredient in `created_assertions`.
