# CSS `calc()` Function Error: Missing Space

This repository demonstrates a subtle but potentially problematic error in using the CSS `calc()` function. The error involves omitting a space between the operator and the numeric value within the `calc()` expression.

## Problem

The following CSS code snippet demonstrates the problem:

```css
.element {
  width: calc(100%-10px); /* Incorrect: Missing space */
}
```

This code will likely not render as expected.  The absence of the space between `-` and `10px` can cause the calculation to fail or produce unexpected results across different browsers.

## Solution

The correct syntax requires a space between the operator and the value:

```css
.element {
  width: calc(100% - 10px); /* Correct: Space added */
}
```

This seemingly small detail can lead to significant layout issues, especially when dealing with complex calculations within the `calc()` function.  Always double-check your spacing within `calc()` expressions.