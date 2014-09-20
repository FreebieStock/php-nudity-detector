PHP Nudity Detector
===================

At [FreebieVectors.com](http://www.freebievectors.com/) we are concerned to filter out inappropriate content (nudity in images). This algorithm tries to detect nudity in the image based on the amount os skin colors in it.

The algorithm is based on J. Marcial-Basilio et al. (2011) paper.

Example usage:

```php
$quant = new Image_FleshSkinQuantifier(__DIR__ . '/preview.jpg');
if($quant->isPorn())
    echo 'This image contains a lot of skin colors, thus might contain some adult content';
else
    echo 'This image does not contain many skin colors, thus is not likely to contain adult content';
```
