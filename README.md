# lunr-unicode-normalizer

An extension to [lunr.js](http://lunrjs.com/) to normalize unicode characters
by removing all diacritical marks.

For example, searching for "facade" will return results for "façade" and
searching for for "façade" will return results for "facade."


## Usage

Just drop in the `lunr.unicodeNormalizer.js` script after `lunr.js` has been
loaded. `lunr.tokenizer` will then be monkeypatched to use
`lunr.unicodeNormalizer`, and you're good to go.
