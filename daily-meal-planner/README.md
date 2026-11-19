```
### Core Interactions & Design

The page works as a small app: you can filter meals, add them to a plan, and watch the shopping list build itself.

- **Meal library & filters** – Ten sample meals are rendered as cards. The search box and chip filters (meal time, diet, prep time) update the grid instantly, with a clear empty state when nothing matches.
- **Plan builder** – Each card has an “Add to plan” button that toggles the meal in your plan. The plan panel shows a summary of total meals, minutes, and calories, and you can remove items or use “Pick for me” for a random suggestion.
- **Shopping list** – Ingredients from all planned meals are merged by name, with duplicate quantities combined. Checkboxes let you tick items off, and a progress bar tracks completion. “Copy list” copies the list as plain text.
- **Responsive & accessible** – The layout adapts from mobile to desktop, with a collapsible navigation menu, visible focus states, and reduced-motion support.
---

**Optimization Tip:** You can replace the sample meals in the `MEALS` array inside the script with your own recipes. Each meal needs an `id`, `name`, `type`, `time`, `kcal`, `tags`, `icon`, `desc`, and an `ingredients` array of `{ n, q }` objects.
