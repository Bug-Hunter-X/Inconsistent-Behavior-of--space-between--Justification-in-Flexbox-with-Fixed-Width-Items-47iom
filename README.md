# Inconsistent Behavior of `justify-content: space-between` in Flexbox

This repository demonstrates an uncommon issue related to the `justify-content: space-between` property in CSS flexbox.  When flex items have a fixed width and their total width exceeds the container's width, some browsers exhibit inconsistent behavior, leading to unexpected layouts.  The `bug.css` file showcases the problem, while `bugSolution.css` offers a potential solution.

## Problem Description

The provided CSS uses `justify-content: space-between` to space out flex items within a container. However, if the sum of the fixed widths of the items exceeds the container's width, the behavior varies across browsers.

## Solution

The solution involves setting a `min-width` on the container to ensure it's large enough to accommodate all items without wrapping, preventing the layout issues.

## Reproducing the Bug

1. Clone this repository.
2. Open `bug.html` in different browsers.
3. Observe the inconsistencies in how the red squares are positioned and spaced.