# Prototype: Validate pantry → recipes → grocery-list flow

Status: resolved
Type: prototype

## Question

What is the smallest prototype that validates the end-to-end user flow from adding pantry items (with expiry) to seeing recipe suggestions and generating a grocery list? Specify screens, minimal data model, and acceptance criteria.

## Answer

The prototype core flow consists of 3 screens:
1. **Pantry Screen**: Add/remove items with name, category, quantity, and expiry date. Visual color-code for items expiring within 3 days.
2. **Recipes Screen**: List simple recipes with required ingredients. Filter by available pantry items ("Can I cook this now?").
3. **Grocery List Screen**: Automatically lists missing ingredients for selected recipes, grouped by category.

**Acceptance criteria**:
- Adding milk expiring in 2 days highlights it red in pantry.
- Selecting a recipe with missing eggs adds eggs to the grocery list.
