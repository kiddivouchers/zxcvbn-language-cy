# zxcvbn-language-cy
Welsh language pack for [zxcvbn-ts](https://github.com/zxcvbn-ts/zxcvbn).

## Installation
Install via NPM:

```shell
$ npm install --save @widerplan/zxcvbn-language-cy
```

## Usage

1. Follow [zxcvbn-ts installation documentation](https://zxcvbn-ts.github.io/zxcvbn/guide/getting-started/#installation)
2. Install this package also
3. Import the dictionary and translations:

```js
import { zxcvbn, zxcvbnOptions } from '@zxcvbn-ts/core'
import zxcvbnCommonPackage from '@zxcvbn-ts/language-common'
import zxcvbnCyPackage from '@widerplan/zxcvbn-language-cy'

const options = {
  translations: zxcvbnCyPackage.translations,
  graphs: zxcvbnCommonPackage.adjacencyGraphs,
  dictionary: {
    ...zxcvbnCommonPackage.dictionary,
    ...zxcvbnCyPackage.dictionary,
  },
}

zxcvbnOptions.setOptions(options)

zxcvbn(password)
```