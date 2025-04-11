---
date: 2025-04-06
tags:
  - css
  - frontend
cssclasses: []
---
![](https://youtu.be/j425CIWRfZ8?si=iTZGpQEM9b6b5hAG)

- In CSS, **`::before`** creates a [pseudo-element](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements) that is the first child of the selected element. It is often used to add cosmetic content to an element with the [`content`](https://developer.mozilla.org/en-US/docs/Web/CSS/content) property. It is inline by default. [::](https://developer.mozilla.org/en-US/docs/Web/CSS/::before)
- transition property is awesome for styling
- absolute anchors to first parent with position relative or root
- The functional **`:has()`** CSS [pseudo-class](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes) represents an element if any of the [relative selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_selectors/Selector_structure#relative_selector) that are passed as an argument match at least one element when anchored against this element. This pseudo-class presents a way of selecting a parent element or a previous sibling element with respect to a reference element by taking a [relative selector list](https://developer.mozilla.org/en-US/docs/Web/CSS/Selector_list#relative_selector_list) as an argument.

```css
li:has(a:active)::before,
.logo:active,
body:has(.logo:active) li::before { ... }

body:has(.logo:active) a:link,
body:has(.logo:active) a:visited { ... }
```