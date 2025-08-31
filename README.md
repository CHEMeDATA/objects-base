# objects-base

This repository contains the javaScript base class of all [CHEMeDATA](https://github.com/orgs/CHEMeDATA) derived ["objects"](https://github.com/orgs/CHEMeDATA/repositories?q=objects). Data classes include chemical information (nmr spectra, physical properties of molecules, etc.) their names end with `-object`. 


# Role

This javaScript base class features:
- Offer methods enabling derived-class developers to concentrate on their main objectives.
- Manage binary encoded data (experimental!).
- Versioning of object data.
- Homogeity of methods and data structure.

# Setup and Usage

In principle this is automatically loaded with the derived classes you use. If not, get this file into your ./src folder with:

```zsh 
mkdir -p "src"
wget -O src/objectBase.js https://raw.githubusercontent.com/chemedata/objects-base/main/src/objectBase.js
```

Place this import statement at the very beginning of your JavaScript viwer class, right above your class definition.

```js 
include... 

import { ObjectBase } from 'objectBase.js';

export class MyObject extends ObjectBase {
	constructor() {
    console.log();
  }
}
```
