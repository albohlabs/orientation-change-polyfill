orientation-change-polyfill
===========================

orientation change polyfill module inspired by https://gist.github.com/JamesEggers1/1904283

### Requirements

* [jQuery](http://jquery.com/)
  - versions: 1.7.0 or later

### Example

    $(function($){  
      if (OrientationManager.supportsOrientationChange) {
        $(window).on('orientationchange', myCallback);
        return;
      }
 
      // use polyfill
      OrientationManager.bind(myCallback);
    });

### TODO

- set `window.orientation` (it should be a real polyfill)

## License
Copyright (c) 2013 Daniel Gräber  
Licensed under the MIT license.
