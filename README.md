# Tailwind CSS @apply Directive Bug with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive does not correctly handle pseudo-selectors like `:hover`, `:focus`, and `:active`.  When using `@apply` with these pseudo-selectors, the styles are not applied as expected.

## Bug Description
The `@apply` directive is designed to apply pre-defined Tailwind CSS utility classes to an element. However, when a utility class includes a pseudo-selector (e.g., `hover:bg-blue-500`), the `@apply` directive fails to correctly apply the styles when the pseudo-selector condition is met.

## Workaround
Instead of using `@apply` with pseudo-selectors, apply the styles directly in the HTML. This ensures the styles are correctly applied to the element in the appropriate state.

## Example
See the `bug.html` file for an example of the bug, and `bugSolution.html` for a working solution.