Elements
=========
Elements are HTML tags such as buttons, labels, and form inputs. They constitute the base styles for the entire site.

# Rules
* Use only tag selectors to style an element. You may only use pseudo selectors (such as :before, :hover) and attribute selectors when used in conjunction with a tag selector (i.e. use `input[type=text]` instead of just `[type=text]`).
* **Never** use a class selector to style an element.
* **Never** include declarations for colors, font, font-size, line-height, shadows, or width when styling elements. These styles will be applied by the current theme file. For example, when styling a border, use the declaration `border: $border-size $border-type` and never include the `border-color` value.