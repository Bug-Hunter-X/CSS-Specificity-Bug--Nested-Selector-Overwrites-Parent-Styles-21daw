# CSS Specificity Bug: Nested Selector Overwrites Parent Styles

This repository demonstrates a subtle bug related to CSS specificity.  The issue arises when trying to style a parent element and its nested children independently. Due to the way CSS specificity works, a more specific selector (in this case, `.container .inner`) might unintentionally override styles defined by a less specific selector (`.container`).

The `bug.css` file showcases the problematic code, while `bugSolution.css` provides a corrected version addressing the specificity issue.

## How to reproduce the bug
1. Open `bug.html` in a web browser.
2. Observe that the `.container` element's background color is unexpectedly overridden by the nested `.inner` element's style.