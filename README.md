# react-native-expo-svg

Convert .svg files to Expo-friendly Svg components.

## Installation

```bash
npm install -g react-native-expo-svg
```

## Usage:

### Output to an `*Icon.js` file

```bash
react-native-expo-svg test.svg
```

this will output a new file named `TestIcon.js`, containing:

```js
import React from "react";
import { Svg } from "expo";

function TestIcon() {
  return (
    <Svg width="41" height="32">
      <Svg.Path
        d="M34.212 12.79a6.11 6.11 0 0 1 .783-.05c3.317 0 6.005 2.665 6.005 5.955 0 3.289-2.688 5.955-6.005 5.955a6.01 6.01 0 0 1-4.051-1.56C27.991 28.38 23.288 32 17.234 32 6.49 32 .079 20.03 0 8.706c-.078-11.324 34.468-11.889 34.468 0 0 1.373-.087 2.74-.256 4.083zm.783 8.909c1.673 0 3.03-1.345 3.03-3.004 0-1.66-1.357-3.005-3.03-3.005-1.673 0-3.029 1.345-3.029 3.005 0 1.659 1.356 3.004 3.03 3.004z"
        fill="#000"
        fillRule="evenodd"
      />
    </Svg>
  );
}

export default TestIcon;
```

### Output result to the command line

If you only need the expo svg printed to the command line instead of a file with a component, run:

```bash
react-native-expo-svg test.svg output
```

Result (printed in the command line):

```bash
<Svg width="41" height="32" ><Svg.Path d="M34.212 12.79a6.11 6.11 0 0 1 .783-.05c3.317 0 6.005 2.665 6.005 5.955 0 3.289-2.688 5.955-6.005 5.955a6.01 6.01 0 0 1-4.051-1.56C27.991 28.38 23.288 32 17.234 32 6.49 32 .079 20.03 0 8.706c-.078-11.324 34.468-11.889 34.468 0 0 1.373-.087 2.74-.256 4.083zm.783 8.909c1.673 0 3.03-1.345 3.03-3.004 0-1.66-1.357-3.005-3.03-3.005-1.673 0-3.029 1.345-3.029 3.005 0 1.659 1.356 3.004 3.03 3.004z" fill="#000" fillRule="evenodd"/></Svg>
```
