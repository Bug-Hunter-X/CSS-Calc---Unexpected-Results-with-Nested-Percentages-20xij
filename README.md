# CSS Calc() Unexpected Results with Nested Percentages

This repository demonstrates a common issue encountered when using the CSS `calc()` function with nested percentage calculations.  The problem arises when percentages within the `calc()` expression refer to different parent elements, leading to unexpected and incorrect sizing or positioning.

The `bug.css` file contains the erroneous CSS, and `bugSolution.css` provides the corrected version.

## Bug Description

When using percentages within `calc()` that relate to different containing blocks, the calculation might not produce the expected outcome. This is because the percentage is resolved relative to the containing block at the time of evaluation.

## Solution

The solution often involves restructuring the CSS or using absolute values instead of relying on percentages nested within `calc()` in such cases.  In some instances, using Javascript to make calculations beforehand and set these values into the CSS as variables may be a more reliable solution.