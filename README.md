# Demonstration in a Bug with Parcel Automatic Reloading

This repro demonstrates a bug with parcel2 automatic reloading.

## Repro Steps
1. Clone and install dependences by running `yarn`
2. Run `yarn start` (which runs `parcel index.html`)
3. Load the page in the browser
4. Make a change to `index.html` in your editor

Result: The page does not automatically reload

## Note
If you remove this line from `index.html`...
```
<script src="showAlert.js"></script>
```
...and repeat, the page will refresh as expected on changes to `index.html`.
