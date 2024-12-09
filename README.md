# Tailwind CSS Flexbox Layout Break on Overflow

This repository demonstrates a common issue with Tailwind CSS flexbox layouts where content overflow in one column can break the layout. The issue occurs because the default flexbox behavior allows columns to shrink and wrap when content exceeds their allocated space.

The solution involves using the `flex-shrink-0` utility class to prevent columns from shrinking and wrapping, ensuring a consistent layout regardless of content length.

## Bug

The `bug.html` file demonstrates the problem. The layout breaks when the content of the second column exceeds the available space.

## Solution

The `solution.html` file demonstrates the solution by adding `flex-shrink-0` to the column divs, preventing content overflow from breaking the layout.

## How to reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the broken layout in the second column.
4. Open `solution.html` in a web browser.
5. Observe the corrected layout with no overflow.