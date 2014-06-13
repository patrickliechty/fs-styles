Modules
=========
Modules are resuable groups of elements, such as forms, popups, and navigation. They are location agnostic, flexible, and should be made with reuse in mind.

# Rules
* Use only class selectors to style a module.
* Preface all class names with `fs-` and use BEM syntax.
* **Never** use tag selectors to style a module.
* **Never** use a parent selector to style a module differently based on it's location on the page. Instead, sub-class the module by creating a new class name which declares the changes needed. For example, if a module needs to look differently in the sidebar, never use the sidebar to style the element and instead create a new class (such as `module--sidebar`) and append this class to the module (such as `<div class="module module--sidebar"></div>`).
* **Never** include declarations for colors, font, font-size, line-height, shadows, or width when styling modules. These styles will be applied by the current theme file. For example, when styling a border, use the declaration `border: $border-size $border-type` and never include the `border-color` value.
