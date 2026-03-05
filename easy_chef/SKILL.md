---
name: easy_chef
description: "Use whenever Oliver shares a recipe or asks to simplify, reformat, or explain a dish — even if he just pastes ingredients or mentions a dish name. Produces structured output with emoji-numbered ingredient cross-references, metric units, step-grouped ingredient lists, and a Samin Nosrat culinary critique."
---

# Easy Chef

Transform any recipe into a structured, easy-to-follow format with cross-referenced ingredients and culinary critique.

## Output Format

### Title
Name of the dish.

### Preparation and Cooking Time
Total prep and cook time.

### Serves
Number of people the recipe feeds.

### Ingredients
Number each ingredient sequentially and assign an emoji. Group by cooking step using bold headings. Order items as they appear in the instructions. Add metric units if missing; add Celsius if only Fahrenheit is given.

Format: `(emoji #N) Name: amount (imperial equivalent if added), any prep note`

Example:
```
**Blanch:**
* (🍖 #1) Pork belly: 1200 g (about 1.3 lb), cut into 2-3 cm chunks
* (💧 #2) Cold water: enough to cover pork belly

**Braise:**
* (🍷 #3) Shaoxing rice wine: 500 ml (about 2 cups)
```

### Instructions
Write step-by-step instructions. Reference every ingredient by its emoji and number on first use in each step, including incidentals like salt and oil.

Example:
```
**Blanch the Pork:** Place pork belly (🍖 #1) in a pot, cover with cold water (💧 #2), and bring to a boil. Skim off froth, then drain and rinse.
**Braise:** Transfer pork to a clean pot. Add Shaoxing rice wine (🍷 #3)...
```

### Notes
Substitutions, make-ahead tips, storage advice, and common mistakes to avoid.

### What Would Samin Nosrat Say?
Critique the recipe through the lens of *Salt, Fat, Acid, Heat*. Specifically address:
- **Salt**: Is it added early enough and in the right places?
- **Fat**: Is fat used well for flavour and texture?
- **Acid**: Is there enough acid, and is it balanced?
- **Heat**: Are temperatures and timings appropriate?
- **Overall**: Is this recipe approachable for a home cook?

---

## Additional Modes

**Shopping list** (when asked): Generate a Google Keep-ready list with tick boxes and the ingredient emojis. Group by supermarket section in this order: vegetables → dairy → meat → beverages → staples & spices.

Example:
```
☐ 🍖 Pork belly (1200 g)
☐ 🍷 Shaoxing rice wine (500 ml)
```

**German translation** (when asked): Translate the full recipe into German. Adapt ingredients to what's available in German supermarkets (e.g. replace Kosher salt with Meersalz, adjust cup measures to ml/g).
