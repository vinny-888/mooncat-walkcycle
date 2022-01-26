# mooncat-walkcycle

## Demo

Up, Down, Left, Right Arrow Keys to Walk
Space Bar to Jump
Change the MoonCat # to see a different MoonCat

[Live Demo](https://vinny-888.github.io/mooncat-walkcycle/index.html)

## Import Module

```javascript
import {MoonCatWalk} from './mooncatWalk.js';
```

## Usage

```javascript
let size = 1;
let tokenId = 0;

// Generate the Sprite Sheet for the specific MoonCat
let spriteSheet = MoonCatWalk.generateMoonCatSpriteSheet(tokenId, size);

let mooncat = document.getElementById('mooncat');

// TODO updte these as the cat moves 
let frame = 0;
let direction = 0;

let x = frame * 32;
/*
  0 = frame 1
  ...
  7 = frame 8
*/
let y = direction * 32;
/*
  0 = right
  1 = up
  2 = down
  3 = left
  4 = idle right
  5 = idle up
  6 = idle down
  7 = idle left
*/

// Set the Sprite Sheet offset for each of the walk cycles
mooncat.style.backgroundPosition = `-${x}px -${y}px`;

// Set the background image to the base64 image data sprite sheet generated above
mooncat.style.backgroundImage = "url('"+spriteSheet+"')";
```

## Sprite Sheet for MoonCat TokenId=0

[OpenSea MoonCat 0](https://opensea.io/assets/0xc3f733ca98e0dad0386979eb96fb1722a1a05e69/0)

![0.png](/images/0.png?raw=true "0.png")
