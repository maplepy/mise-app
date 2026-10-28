## Destination

Prototype plan: a throwaway prototype that validates the core UX flows (add/manage pantry items with expiry, pantry→recipes matching, and grocery list generation).

## Notes

- Base: use the Recipease Obsidian notes in the repo as the domain reference.
- Target: Expo / React Native prototype, local-only storage (SQLite or AsyncStorage).
- Skills to consult when resolving tickets: grilling, domain-modeling.

## Decisions so far

<!-- closed tickets will be listed here as they are resolved -->

- [Prototype: Validate pantry → recipes → grocery-list flow](issues/01-validate-core-flow.md): Core flow validated: Pantry (expiry + category), Recipes (pantry matching), Grocery List (auto-add missing items).

## Not yet specified

- Exact import formats for recipes (web/social) and the priority for each.
- Which subset of UI screens to ship in the prototype (home vs full recipe editor).

## Out of scope

- Backend sync, pricing/nutrition external APIs, advanced AI features.
