## Accessibility Tools
These tools help test and improve accessibility:

Keyboard navigation: Can you tab through the page logically?

Screen readers: Tools like NVDA (Windows) or VoiceOver (Mac) read aloud content.

Browser extensions:

✅ WAVE (WebAIM)

✅ axe (Deque)

Lighthouse (built into Chrome DevTools): Audits accessibility performance

## ARIA Attribute Types
role
Describes what the element is (its function).
🔹 Example: role="button", role="navigation", role="dialog"

property
Describes characteristics of an element.
🔹 Example: aria-label="Close Menu" gives a screen reader-friendly name.

state
Describes a current condition that might change.
🔹 Example: aria-expanded="false" on a menu toggle

## Text Content & Readability
Accessible content means clear, meaningful text that:

Is visible to all users (not hidden in images or inaccessible widgets)

Uses semantic elements (<h1>–<h6>, <p>, <button>) for structure

Avoids vague links like "click here" — instead use “Learn more about accessibility”

## Best Practices
Use native HTML elements first (they're accessible by default)

Use ARIA only when necessary — and correctly

Always test with keyboard and screen reader

Label buttons and forms clearly