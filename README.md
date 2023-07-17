# Profanity Filter

![version](https://img.shields.io/badge/version-1.0.0-blue)
![downloads](https://img.shields.io/badge/downloads-100%2Fweek-green)

[NPM package available here.](https://www.npmjs.com/package/custom-profanity-filter)
## Installation
npm install custom-profanity-filter

## Usage

You will have to provide the custom list of bad words for the filter. Ensure that the custom list of bad words you want to filter is in an array format.
customBadWords = ["custom", "list", "here"];

The filter is case insensitive and will pick up words part of a larger string.

```javascript
const profanityFilter = require('custom-profanity-filter');

let customBadWords = ["custom1", "custom2", "custom3"];
let textToFilter = "This is some text with custom1 and CUSTOM2 and another custom1word without space.";

let filteredText = profanityFilter(textToFilter, customBadWords);
console.log(filteredText);  // Outputs the filtered text