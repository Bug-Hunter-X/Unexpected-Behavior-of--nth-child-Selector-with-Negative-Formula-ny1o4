# Unexpected Behavior of :nth-child Selector with Negative Formula

This repository demonstrates an uncommon error related to the CSS `:nth-child` pseudo-class selector when using a formula that results in a negative value. The selector `:nth-child(-n+3)` is intended to style the first three list items, but its behavior varies between browsers and often produces unexpected results.

The primary issue is the use of a negative value (`-n`) within the `an+b` formula of the `:nth-child` selector. While some contexts allow for negative indexes, `:nth-child` requires a non-negative value for reliable selection.

The `bug.css` file shows the erroneous CSS code, and `bugSolution.css` provides the corrected version.  The solution addresses the problem by using a different, valid formula to target the first three list elements.

This example highlights a potential pitfall when working with `:nth-child` and complex formulas.  It's crucial to test thoroughly and avoid negative values in the formula to ensure cross-browser compatibility and expected styling results.