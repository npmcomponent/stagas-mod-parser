*This repository is a mirror of the [component](http://component.io) module [stagas/mod-parser](http://github.com/stagas/mod-parser). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/stagas-mod-parser`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# mod-parser

module (.mod) parser in javascript

## Example

```js
function play(buffer){
  if (playing) playing.disconnect();
  var mod = new ModParser(buffer);
  var player = new ModPlayer(mod, rate, size);
  var node = playing = process(audio, size, player.process);
  node.connect(audio.destination);
}
```

## Credits

* [gasman](https://github.com/gasman) [original](https://github.com/gasman/jsmodplayer)
* [BillyWM](https://github.com/BillyWM) [improvements (fork based upon)](https://github.com/BillyWM/jsmodplayer)

## License

MIT
