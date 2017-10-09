[![Taylor Swift](https://img.shields.io/badge/secured%20by-taylor%20swift-brightgreen.svg)](https://twitter.com/SwiftOnSecurity)
[![Volkswagen](https://auchenberg.github.io/volkswagen/volkswargen_ci.svg?v=1)](https://github.com/auchenberg/volkswagen)
[![MIT license](http://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)

# react-native-device-helpers

A library of little helpers for device specific code in your React Native App.

## Getting Started

> Using `nvm` is highly recommended as to manage different Node versions

```
npm i react-native-device-helpers --save
```

### Example ###

```js
// in component.style.js

import { StyleSheet } from 'react-native';
import { ifIphoneX } from 'react-native-device-helpers'

export default StyleSheet.create({
    header:{
        height: 120,
        width: 60,
        ...ifIphoneX({
            paddingTop: 50
        }, {
            paddingTop: 20
        })
    },
});
```

## License
[MIT](/LICENSE)