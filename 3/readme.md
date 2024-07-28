### Question 2: Sticky Header, Fixed Positioning, and Visibility Management

**Details:**
- **Display vs. Visibility:** `display: none` removes an element from the document flow, while `visibility: hidden` hides the element but keeps its space in the layout.
- **z-index:** The `z-index` property controls the stack order of positioned elements. Higher values are on top of lower values.
- **Sticky Header:** `position: sticky` makes the header stick to the top of the viewport when scrolling. It has a `top` value of `0` to keep it always at the top.
- **Fixed Footer:** `position: fixed` keeps the footer at the bottom of the viewport, regardless of scrolling. It has a lower `z-index` compared to the header.
- **Sticky Section:** The `.sticky-section` should stick to the top of the viewport below the header, with a `top` value of `100px` to avoid overlap.
- **Visibility Management:** The button toggles the visibility of the `#toggleElement` div between `display: none` and `display: block`. The second hidden element remains in the layout but is not visible.
- **Box-Sizing:** Applied globally to ensure consistent box-sizing across all elements.

**Instructions:**
1. Create a sticky header that remains at the top of the viewport when scrolling.
2. Implement a fixed footer that stays at the bottom of the viewport regardless of scrolling.
3. Add a section that sticks below the header while scrolling.
4. Create two hidden elements and use JavaScript to toggle the visibility of one element between `display: none` and `display: block`. The other element should be hidden using `visibility: hidden`.
