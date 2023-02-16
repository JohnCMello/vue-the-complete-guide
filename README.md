## Module Summary

- Component Registration & styles

  - Components can be registered globally or locally. Prefer local registers.
  - Styles can be global or scoped to a component.Prefer scoped for most components

- Slots

  - Slots can be used to add a "placeholder" for dynamic HTML.
  - Multiple, named slots are possible, default fallbacks can be provided. Scoped slots allow advanced use-cases.

- Dynamic Components

  - Components can be swapped dynamically via de built-it <component> component.
  - Component caching can be added via de <keep-alive> component.

- Teleport & styles.
  - Dom structure can be manipulated via <teleport> - it keeps the component hierarchy.
  - Consider following the official style guide do keep code clean and understandable.
