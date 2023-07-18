# Profanity Filter
![version](https://img.shields.io/npm/v/custom-profanity-filter.svg)
![downloads](https://img.shields.io/npm/dm/custom-profanity-filter.svg)

In the era of social media, trolls and negativity can often overshadow the benefits of open communication. Harsh words or profanity can turn any constructive conversation into a hostile environment. This is where our profanity filter Node.js module comes in handy. Designed to sanitize user-generated content, it helps to maintain the quality and decency of discussions by filtering out offensive words.

Built for flexibility, this module allows you to use a default list of profane words or define a custom list based on your needs. Regardless of where the offending words appear, whether standalone or within other words, our filter can identify and replace them, ensuring a safer and more respectful social platform.

Easy to integrate and use, this module is a valuable addition to any project that values positive and respectful communication. Remember, the pen is mightier than the sword, and with our profanity filter, we can ensure it's also more polite."

Remember, the exact wording can be adjusted based on your understanding of the module's functionality and your project's tone and style.

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
