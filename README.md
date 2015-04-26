# pixi-tiled

Import [Tiled](http://www.mapeditor.org/) maps into pixi v3.

## installation

```sh
npm install pixi-tiled
```

## usage

```js
var PIXI = require('pixi.js');
var pixiTiled = require('pixi-tiled');

/**
 * simply load a Tiled map in json format
 * the plugin has automatically registered itself to handle the file
 * the map will be loaded, parsed and made available on res.tiledMap
 */
PIXI.loader.add('map.json', function(res) {

    var map = res.tiledMap;
    
    /**
     * the resulting pixiTiled.Map object is an extension of PIXI.Container
     * and so is fully renderable
     */
    // renderer.render(res.tiledMap);
    
});

PIXI.loader.load();
```
