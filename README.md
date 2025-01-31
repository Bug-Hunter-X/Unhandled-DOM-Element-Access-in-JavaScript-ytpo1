# Unhandled DOM Element Access in JavaScript

This repository demonstrates a common yet often overlooked error in HTML/JavaScript: attempting to manipulate a DOM element without first verifying its existence.  This can lead to silent failures or unexpected behavior.  The bug and solution show how to robustly handle such scenarios.

## Bug

The `bug.html` file contains a simple HTML page with a button. When you click the button, the JavaScript code attempts to hide a div element. The problem is that if the div element is not found, the code will throw an error silently. 

## Solution

The `solution.html` file demonstrates the correct way to handle this scenario. Before attempting to manipulate the div element, the code first checks if it exists using `getElementById`. If the element exists, then its display is set to "none"; otherwise, a fallback is executed or appropriate message is shown to the user.  This prevents unexpected errors and makes the code more robust.