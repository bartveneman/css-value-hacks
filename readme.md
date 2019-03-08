# css-value-browser-h4cks-analyzer 
[![Build Status](https://travis-ci.org/bartveneman/css-value-browser-h4cks-analyzer.svg?branch=master)](https://travis-ci.org/bartveneman/css-value-browser-h4cks-analyzer) 
[![Known Vulnerabilities](https://snyk.io/test/github/bartveneman/css-value-browser-h4cks-analyzer/badge.svg)](https://snyk.io/test/github/bartveneman/css-value-browser-h4cks-analyzer) 
![Dependencies Status](https://img.shields.io/david/bartveneman/css-value-browser-h4cks-analyzer.svg) 
![Dependencies Status](https://img.shields.io/david/dev/bartveneman/css-value-browser-h4cks-analyzer.svg) 
[![XO code style](https://img.shields.io/badge/code_style-XO-5ed9c7.svg)](https://github.com/sindresorhus/xo)
[![Project: Wallace](https://img.shields.io/badge/Project-Wallace-29c87d.svg)](https://www.projectwallace.com/oss)

A list of tests to determine whether a value is a browser hack, derived from the
formidable [browserhacks.com](https://browserhacks.com)
([Repo](https://github.com/4ae9b8/browserhacks)).

## Installation

```bash
npm install css-value-browser-h4cks-analyzer

# or

yarn add css-value-browser-h4cks-analyzer
```

## Usage

```js
const isBrowserHack = require('css-value-browser-h4cks-analyzer')

// CSS declaration example => .selector { property: value !ie; }
console.log(isBrowserHack('value !ie'))
// => true

console.log(isBrowserHack('1px solid red'))
// => false
```

## Related projects

- [CSS Analyzer](https://github.com/projectwallace/css-analyzer) - CSS
  statistics module
- [Wallace CLI](https://github.com/bartveneman/wallace-cli) - CSS statistics in
  your CLI
- [CSS Analyzer Diff](https://github.com/bartveneman/css-analyzer-diff) -
  Calculates the diff between two sets of CSS analysis
- [Color Sorter](https://github.com/bartveneman/color-sorter) - Sort CSS colors
  by hue, saturation, lightness and opacity
- [Gromit CLI](https://github.com/bartveneman/gromit-cli) - A test framework to
  assert that CSS statistics don't exceed certain thresholds.

## License

MIT © Bart Veneman
