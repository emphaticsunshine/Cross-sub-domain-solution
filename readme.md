# Overview
A solution for cross sub domain request from a browser



## Problem:
Cross sub domain request is not possible using ajax because of browser securities. 

## Use Case:
* Trying to get content from second app to the first app to avoid rewriting the code.
* Get content from existing app.

## Proposed Solution:
Use a hidden iframe in a running app.
The trick behind iframe to get sub domain content is to initialize "document.domain" using javascript to the same domains on both side.
Get content into iframe and replace those contents to running target location.
Created a very easy to use function to perform this operation. Developer has to write a single line in code to initialize the plugin
