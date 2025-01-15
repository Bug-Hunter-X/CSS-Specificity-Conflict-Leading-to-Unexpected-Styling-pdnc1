# CSS Specificity Conflict

This repository demonstrates a common CSS issue where specificity conflicts lead to unexpected styling outcomes. The problem lies in the way CSS determines which styles are applied when multiple rules match the same element. Rules with higher specificity win.

## Problem

The `bug.css` file shows a scenario with several conflicting styles. Despite having a rule that specifically targets `#container .box`, a more specific rule (`#container .box.special`) overrides it.

## Solution

The `bugSolution.css` file provides a potential solution involving either adjusting the specificity of the existing rules or utilizing the `!important` flag (though using this is generally discouraged unless absolutely necessary).