<a href="https://unly.org"><img src="https://storage.googleapis.com/unly/images/ICON_UNLY.png" align="right" height="20" alt="Unly logo" title="Unly logo" /></a>
# iso3166-1 [![Build Status][travis-image]][travis-url]
[![Version][npm-version-image]][npm-version-url] [![License][npm-license-image]][npm-license-url] [![Downloads][npm-downloads-image]][npm-downloads-url] [![Deps][npm-deps-image]][npm-deps-url] [![DevDeps][npm-devdeps-image]][npm-devdeps-url]
[![Known Vulnerabilities](https://snyk.io/test/github/UnlyEd/iso3166-1/badge.svg?targetFile=package.json)](https://snyk.io/test/github/UnlyEd/iso3166-1?targetFile=package.json)

The smallest, fastest, node module for ISO 3166-1 alpha 2/3 helper lookup/parser. Browserify/Webpack friendly.

## Install

```bash
npm install --save iso3166-1
```

## Usage

```
var iso31661 = require('iso3166-1')
iso31661.from('USA').to3()         // USA
iso31661.from('USA').to2()         // US
iso31661.from('US').to3()          // USA
iso31661.from('US').to2()          // US
iso31661.fromLocale('en-US').to3() // USA
iso31661.fromLocale('en-US').to2() // US
```

```
var iso31661 = require('iso3166-1')
iso31661.to2('USA') // US
iso31661.to3('US')  // USA
```

```
var iso31661 = require('iso3166-1')
var locale2 = require('locale2')
iso31661.fromLocale(locale2).to3() // USA
iso31661.fromLocale(locale2).to2() // US
```

```
import iso31661 from 'iso3166-1';
iso31661.is2('US')  // true
iso31661.is3('USA') // true
iso31661.is2('XX')  // false
iso31661.is3('XXX') // false
```

## License

MIT

# Vulnerability disclosure

[See our policy](https://github.com/UnlyEd/Unly).

---

# Contributors and maintainers

This project is being maintained by:
- [Unly] Ambroise Dhenain ([Vadorequest](https://github.com/vadorequest)) **(active)**

---

# **[ABOUT UNLY]** <a href="https://unly.org"><img src="https://storage.googleapis.com/unly/images/ICON_UNLY.png" height="40" align="right" alt="Unly logo" title="Unly logo" /></a>

> [Unly](https://unly.org) is a socially responsible company, fighting inequality and facilitating access to higher education. 
> Unly is committed to making education more inclusive, through responsible funding for students. 
We provide technological solutions to help students find the necessary funding for their studies. 

We proudly participate in many TechForGood initiatives. To support and learn more about our actions to make education accessible, visit : 
- https://twitter.com/UnlyEd
- https://www.facebook.com/UnlyEd/
- https://www.linkedin.com/company/unly
- [Interested to work with us?](https://jobs.zenploy.io/unly/about)

Tech tips and tricks from our CTO on our [Medium page](https://medium.com/unly-org/tech/home)!

#TECHFORGOOD #EDUCATIONFORALL


[npm-version-url]: https://www.npmjs.com/package/iso3166-1
[npm-version-image]: https://img.shields.io/npm/v/iso3166-1.svg
[npm-license-url]: https://github.com/moimikey/iso3166-1/blob/master/LICENSE
[npm-license-image]: https://img.shields.io/npm/l/iso3166-1.svg
[npm-downloads-url]: https://www.npmjs.com/package/iso3166-1
[npm-downloads-image]: https://img.shields.io/npm/dm/iso3166-1.svg
[npm-deps-url]: https://david-dm.org/moimikey/iso3166-1
[npm-deps-image]: https://img.shields.io/david/moimikey/iso3166-1.svg
[npm-devdeps-url]: https://david-dm.org/moimikey/iso3166-1
[npm-devdeps-image]: https://img.shields.io/david/dev/moimikey/iso3166-1.svg
[travis-url]: https://travis-ci.org/moimikey/iso3166-1
[travis-image]: https://travis-ci.org/moimikey/iso3166-1.svg?branch=master
