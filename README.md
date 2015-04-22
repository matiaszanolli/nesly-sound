nesly-sound
===========

[![Build Status](https://travis-ci.org/emkay/nesly-sound.svg?branch=master)](https://travis-ci.org/emkay/nesly-sound)

Create beautiful music on your NES

## Special Thanks

Thomas Hjelm wrote the sound engine code in 6052 asm that this project uses. If you want to learn how sound (or anything else) on the NES works check out the [Nintendo Age Forums](http://nintendoage.com/forum/messageview.cfm?catid=22&threadid=7155). Without those this wouldn't even be possible.

## Install

`npm install nesly-sound`

## Example

```javascript
var song = require('nesly-sound')();

song.square1(['C5', 'E5', 'G5', 'C6'])
    .timing(1/8)
    .loop(4);

song.loop()
    .done();

song.write();
```
