# domain-regex.js
JavaScript Domain Regex

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Installation
```html
<script src="domain-regex.js"></script>
```
or
```
npm install --save domain-regex.js
```
```javascript
require('domain-regex.js');
```

## Usage
```javascript
// false
domainRegex.test('htt://githubcom');
domainRegex.test('http://githubcom');
domainRegex.test('http//githubcom');
domainRegex.test('http:/githubcom');
domainRegex.test('http:/github.com123');
domainRegex.test('22http://github.com');

// true
domainRegex.test('github.com');
domainRegex.test('http://github.com');
domainRegex.test('http://www.github.com');
domainRegex.test('https://github.com');
domainRegex.test('https://www.github.com');

// Unicode Domains
domainRegex.test('짧.한국');
domainRegex.test('http://짧.한국');
domainRegex.test('https://www.facebook.com/소행성-소녀-387632298355712');
```

## License
[MIT](LICENSE)

## Author
[Young Jae Sim](https://github.com/Hanul)