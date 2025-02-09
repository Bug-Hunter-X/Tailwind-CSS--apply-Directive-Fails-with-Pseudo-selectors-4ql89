# Tailwind CSS @apply Directive Issue with Pseudo-selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly apply styles when used with pseudo-selectors such as `&:hover` within a custom class.  The expected hover effect is not applied. This issue is observed in [version of Tailwind CSS].

## Reproduction Steps

1. Clone this repository.
2. Install the necessary dependencies (if any).
3. Run the application (if applicable).
4. Observe that the hover styles are not applied to the element using the custom class with `@apply`.

## Solution

The issue is resolved by applying the styles directly to the pseudo-selector within the component's styles or by restructuring the custom class to avoid using `@apply` for pseudo-selectors.  See `bugSolution.css` for a working solution.