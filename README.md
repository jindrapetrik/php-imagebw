# php-imagebw
PHP Functions for converting image to greyscale and to black and white.

## Usage
Simply include `imagebw.php` in your project and start using
`imagegreyscale` and `imagebw` functions - see docs below.

## Function docs
```php
/**
 * Converts image to greyscale
 * @param resource|GdImage $img
 */
function imagegreyscale($img): void;

/**
 * Converts image to black and white image
 * @param resource|GdImage $img
 * @param int $type See BW_ constants
 */
function imagebw($img, int $type): void;
```

## Methods of black and white conversion - `BW_` constants
For second parameter of `imagebw` a `$type` of conversion is needed.

You can use following constants:
```php
/**
 * Nearest color
 */
define("BW_NORMAL", 0);
/**
 * Floyd/Steinenberg
 */
define("BW_FLOID", 1);
/**
 * Stucki
 */
define("BW_STUCKI", 2);
/**
 * Burkes
 */
define("BW_BURKES", 3);
/**
 * Bayer
 */
define("BW_BAYER", 4);
```

## License
The library is licensed under GNU/LGPL v2.1, see [LICENSE](LICENSE)
for details.

## Author
Jindra Petřík aka JPEXS

## Changelog
Changes in versions are logged in the file [CHANGELOG.md](CHANGELOG.md)
