---
"@joinmonolith/c2pa-node": patch
---

Default the spec-mandatory `dc:format` and `instanceID` fields and pass through
`metadata` when recording a created `c2pa.ingredient.v3` assertion, so
`addIngredient` calls with minimal ingredient JSON produce a decodable assertion.
