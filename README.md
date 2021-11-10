# worldfiles-js

### *!! This package is not yet published !!*

## Usage
### Import
```js
const wf = require('../worldfiles.js');
```

### Create wf object
##### With JSON-object 
```js
w1 = new wf.worldFile({
    A: 1.266085014, 
    D: -0.09964305157,
    B: -0.09964305157,
    E: -1.266085014,
    C: 563252.8774,
    F: 6504846.927,
};
```
##### From file
```js
w1 = new wf.worldFile(wf.readFile("./image.pgw"));
```

### Coordinates to Pixel
```js
w1.coordToPx(565355, 6503003); // x, y // longitude, latitude
```
Returns the pixel x and y value as an JSON-object.
```js
{ x: 1764.0277970702975, y: 1317.568622011786 }
```
