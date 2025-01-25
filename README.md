# Uncommon HTML Bug: Unexpected innerHTML Behavior

This repository demonstrates an uncommon bug related to the use of `innerHTML` in HTML.  The issue arises when attempting to append content to an existing element using `innerHTML` in a way that inadvertently overwrites the original content.

## Bug Description
The original content of the div is replaced instead of being appended to, due to the way innerHTML operates. This can be very subtle and hard to track down if you're not expecting it. 

## How to Reproduce
1. Open `bug.html` in a web browser.
2. Observe the unexpected behavior. The intended behavior was to append to the existing text in the div; however, only the newly added content from the script is shown.

## Solution
The solution involves using `textContent` or `appendChild` to correctly append content without replacing the initial content of the div element. This avoids unexpected behavior and ensures that both the original and new content are displayed. 
