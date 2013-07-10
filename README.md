orientation-change-polyfill
===========================

orientation change polyfill module Inspired by https://gist.github.com/JamesEggers1/1904283

## Example

    $(function($){  
      if (OrientationManager.supportsOrientationChange) {
        $(window).on('orientationchange', myCallback);
        return;
      }
 
      // use polyfill
      OrientationManager.bind(myCallback);
    });

## License
Copyright (c) 2013 Daniel Gräber  
Licensed under the MIT license.
