### Question 1: Box-Sizing, Width Properties, and Selectors
- **CSS Question:** What does the `box-sizing` property do? What's the difference between `width: auto` and `width: 100%`?
- **CSS Question:** How do you use various CSS selectors, such as adjacent sibling selectors and class selectors?

**Details:**
- **Box-Sizing Property:** The `box-sizing` property allows you to define how the width and height of an element are calculated. The `border-box` value includes padding and border in the element's total width and height.
- **Width Properties:** `width: auto` sets the width of an element based on its content, while `width: 100%` makes the element take up the full width of its container.
- **CSS Selectors:** CSS selectors are used to select and style specific elements. Examples include class selectors (`.class`), ID selectors (`#id`), and sibling selectors (`+`, `~`).


**Links**
https://htmlbook.ru/css/selector/sibling

**Key words**
width, cascade, selectors

**Instructions**:

- Ensure the paragraph immediately following the ul with id="menu" has a red color.
- Add another paragraph with class highlight that should only be blue.

- *Change the width of the box to 100% and apply box-sizing: border-box.

what will happen?

- add to .box
margin-left: 50px;
box-sizing: border-box;


Explanations:


https://stackoverflow.com/questions/17468733/difference-between-width-auto-and-width-100-percent#:~:text=width%3A%20auto%3B%20will%20try%20as,without%20regards%20to%20the%20parent.


As long as the value of width is auto, the element can have horizontal margin, padding and border without becoming wider than its container (unless of course the sum of margin-left + border-left-width + padding-left + padding-right + border-right-width + margin-right is larger than the container). The width of its content box will be whatever is left when the margin, padding and border have been subtracted from the container’s width.

On the other hand, if you specify width:100%, the element’s total width will be 100% of its containing block plus any horizontal margin, padding and border (unless you’ve used box-sizing:border-box, in which case only margins are added to the 100% to change how its total width is calculated). This may be what you want, but most likely it isn’t.

width:auto;
width will never exceed the total width of parent element. Maximum width is it's parent width. Even if we add border, padding and margin, content of element itself will become smaller in order to give space for border, padding and margin. In case if space required for border + padding + margin is greater than total width of parent element then width of content will become zero.

When we say

width:100%;
width of content of element will become 100% of parent element and from now if we add border, padding or margin then it will cause child element to exceed parent element's width and it will starts overflowing out of parent element.