# CSS Specificity Bug

This repository demonstrates a common yet often overlooked CSS specificity issue. The bug arises from insufficient specificity in a CSS rule, leading to unintended styling consequences.

## Bug Description

A lack of specificity in the CSS rule `.container p { color: blue; }` results in the style being applied to more elements than intended. If a similar structure exists elsewhere in the document, the rule will also apply there, leading to unforeseen styling changes.

## Solution

The solution involves increasing the specificity of the CSS selector to precisely target only the intended elements. This is achieved by using more specific selectors or by employing the `!important` flag (though this is generally discouraged for maintainability).

## How to reproduce

1. Clone this repository
2. Open `bug.html` in your web browser
3. Observe that the unexpected element is also styled in blue
4. Open `solution.html` and observe that only the intended element is styled.