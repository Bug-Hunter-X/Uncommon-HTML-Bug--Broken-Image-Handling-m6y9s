# Uncommon HTML Bug: Broken Image Handling

This repository demonstrates an uncommon bug in HTML related to how browsers handle broken images. The bug doesn't produce a syntax error, but instead leads to unexpected behavior, potentially impacting the layout or user experience.

## Bug Description

The bug lies in the way the code attempts to set the innerHTML of a div element with an image that doesn't exist. The browser will try to load `invalid-image.jpg`, but fail. This can lead to problems such as a blank space where the image should be, or even console errors depending on browser settings.

## Solution

The solution involves implementing more robust error handling. By using the `onerror` event on the image element, you can prevent unexpected behaviour.  An alternative image or placeholder can be shown, or other actions taken, making the overall experience more user-friendly.