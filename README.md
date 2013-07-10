orientation-change-polyfill
===========================

orientation change polyfill module inspired by https://gist.github.com/JamesEggers1/1904283

### Requirements

* [jQuery](http://jquery.com/)
  - versions: 1.7.0 or later

### Example

    if (OrientationManager.supportsOrientationChange) {
      $(window).on('orientationchange', myCallback);
    } else {
      // use polyfill
      OrientationManager.bind(myCallback);
    }

### TODO

- set `window.orientation` (it should be a real polyfill)

## License
orientation-change-polyfill is free and open source software, released under the terms of the [GNU General Public License version 3](http://www.gnu.org/licenses/gpl.html)
