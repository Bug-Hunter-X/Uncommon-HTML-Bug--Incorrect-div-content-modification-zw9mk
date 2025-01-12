# Uncommon HTML Bug: Incorrect div content modification

This repository demonstrates an uncommon bug related to modifying the content of a div element in HTML using innerHTML and outerHTML.  The issue is that the browser's automatic correction might prevent the changes from being rendered, leading to unexpected behavior.

## Bug Description
The provided HTML code attempts to change the content of a div with the id "myDiv." However, due to the way innerHTML and outerHTML are used, the changes are not reflected in the rendered output.  This can be confusing because it might appear as though the code is correct, but the browser silently prevents the invalid operations.

## Solution
The solution involves using a more robust approach for updating the div's content and to prevent this situation to happen. This includes correctly appending or replacing the content within the div instead of modifying its complete structure. 

## How to reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that the new text is not displayed, despite seemingly valid JavaScript code. Open `bugSolution.html` to see the solution