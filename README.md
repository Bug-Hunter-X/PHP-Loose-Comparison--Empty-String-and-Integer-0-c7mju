# PHP Loose Comparison Bug

This repository demonstrates a subtle bug in PHP related to loose comparisons between empty strings and the integer 0.  Loose comparison (==) can lead to unexpected results. The `bug.php` file showcases the problem, while `bugSolution.php` provides the correct solution using strict comparison (===).

## Problem

In PHP, the loose comparison operator (==) does not always produce the expected results when comparing an empty string ('') to the integer 0 (0).  This can lead to unexpected behavior in your code, potentially causing bugs that are hard to track down.

## Solution

The solution is to use the strict comparison operator (===).  Strict comparison checks for both value and type equality. This ensures that the comparison is accurate and predictable. Refer to `bugSolution.php` for an example of how to fix the bug using strict comparison.

## How to reproduce the bug

1. Clone this repository.
2. Run the `bug.php` script using PHP (e.g., `php bug.php`). Observe the output.
3. Run the `bugSolution.php` script using PHP. Observe the difference in the output.
