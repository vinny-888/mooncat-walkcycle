# mooncat-walkcycle

## Demo

Up, Down, Left, Right Arrow Keys to Walk
Space Bar to Jump
Change the MoonCat # to see a different MoonCat

[Live Demo](https://vinny-888.github.io/mooncat-walkcycle/index.html)

## Import Module

```
import {MoonCatWalk} from './mooncatWalk.js';
```

## Usage

```
let size = 1;
let tokenId = 0;
let spriteSheet = MoonCatWalk.generateMoonCatSpriteSheet(tokenId, size);
document.getElementById('sprite_sheet').src = spriteSheet;
```

## Sprite Sheet for MoonCat TokenId=0

[OpenSea MoonCat 0](https://opensea.io/assets/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/0)

![0.png](/images/0.png?raw=true "0.png")
