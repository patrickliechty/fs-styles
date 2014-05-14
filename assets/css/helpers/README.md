Helpers
=========
Helpers are any utility tools or files that can be used across the site, such as colors, mixins, and functions.

# Rules
* Mixins which are triggered off of CSS properties should only be used to output vendor prefixes (such as `box-shadow` or `border-box`). This helps reduce any undesired effects when writing CSS.
* Functions should always be called using parentheses (such as `clearfix()`) and never look like a declaration. This helps developers know where the output is coming from.
* Variables should start with the most generic term and end with the most specific term (such as `$color-background-input`). Doing so will group common variables into categories which are easier to remember and search for.
* **Never** declare a variable that starts with `$brand-color`.
* **Never** use the a `$brand-color` variable in a CSS declaration. These variables are reserved and only used to create more functional color variables.
* When creating a new color variable to be used, create a new `$color` variable and set it to equal one of the `$brand-color`s. This will allow it to be more easily changed to a different color.
* Always use variables that start with `$color` for any CSS declarations. These variables are kept color agnostic so that they can be easily changed.