# Inconsistent Layout with calc() and inline-block in CSS

This repository demonstrates a common issue encountered when using the `calc()` function with `inline-block` elements in CSS.  The problem arises from inconsistent handling of whitespace and margin collapse across different browsers, leading to unexpected layout variations.

The `bug.css` file contains the problematic code.  The `bugSolution.css` file provides a solution to mitigate the issue.

## Bug Description

The core problem lies in the combination of `calc()` to determine the width and the `inline-block` display type.  Whitespace or margin collapse around the `inline-block` elements can cause the calculated width to be inaccurate or inconsistent, resulting in misaligned elements.

## Solution

The solution in `bugSolution.css` addresses this by using a more robust approach to layout.  This might involve using a different display type, like `block` or `flex`, or adding explicit spacing to ensure consistent rendering.