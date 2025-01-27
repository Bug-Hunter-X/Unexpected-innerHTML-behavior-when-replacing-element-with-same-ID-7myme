# Uncommon HTML Bug: Unexpected innerHTML Behavior

This repository demonstrates an uncommon bug related to the use of `innerHTML` in HTML.  Specifically, it highlights the issue of replacing an element with another element having the same ID using `innerHTML`. This can lead to unexpected behavior, including the loss of event listeners and associated data.

## Bug Description
The bug occurs when using `innerHTML` to replace an element with a new element having the same ID. This action removes the original element from the DOM, including any attached event listeners or data. The behavior is different than simply changing the contents of the element. 

## Solution
The solution involves using DOM manipulation methods such as `replaceChild` to correctly replace elements without unexpected consequences.