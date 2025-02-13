# Uncommon HTML Error: Incorrect Event Listener Usage

This repository demonstrates a subtle error related to event listener attachment in HTML.  Older browsers used `attachEvent`, while modern browsers use `addEventListener`.  Mixing these approaches can lead to unexpected behavior or incompatibility.

## Bug Description
The primary issue lies in using `attachEvent` for adding an event listener.  This method, while functional in older Internet Explorer versions, is not consistent across browsers and can lead to failures in more modern environments.

## Solution
The solution is to standardize on the `addEventListener` method.  This ensures better cross-browser compatibility and avoids any potential inconsistencies related to event handling.