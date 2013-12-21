# embed-youtube

Embed youtube videos.

## Installation

Install with [component(1)](http://component.io):

```
$ component install fredsterss/embed-youtube
```

## Example

Embed-youtube currently depends on ``swfobject.js``. 
@TODO - componentize this.

```
<script src="//ajax.googleapis.com/ajax/libs/swfobject/2.2/swfobject.js"></script>
```


```
var y = require('embed-youtube');
var youtube = y(el, videoId, width, height);
y.play();
```

To use it, pass in the Youtube video ``id``, ``width`` and ``height``.

## API

### Youtube(el, videoId, width, height)

Insert a new Youtube embed instance into ``el`` with the given ``videoId``, ``width`` and ``height``.

### #play(fn)

Play whatever video is loaded, emitting ``play``, optionally calling ``fn``.

### #pause(fn)

Pause whatever video is loaded, emitting ``pause``, optionally calling ``fn``.

## License

MIT
