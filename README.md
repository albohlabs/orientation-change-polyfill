orientation-change-polyfill
===========================

orientation change polyfill module

## jQuery binding

Example:

    $(function($){  
      if (OrientationManager.supportsOrientationChange) {
        $(window).on('orientationchange', myCallback);
        return;
      }
 
      // use polyfill
      OrientationManager.bind(myCallback);
    });


Inspired by https://gist.github.com/JamesEggers1/1904283
