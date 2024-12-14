# Uncommon HTML innerHTML Bug

This repository demonstrates a subtle bug related to setting the `innerHTML` property of an HTML element to `null`.  While one might expect this to completely remove the element's content, it actually results in an empty string being assigned.

The `bug.html` file shows the problematic code.  The `bugSolution.html` file provides a corrected version.

This is a helpful example illustrating that directly setting `innerHTML` to `null` is not the standard or effective way to clear content.  The best practice is to use either `innerHTML = ''` or other appropriate methods like `removeChild()` for more controlled removal.