# thumbnail

Usage
------

```php
{var $image='images/image.jpg'}

<img src="{$image|thumbnail: 150, 150}" />

```

config.neon

```yaml


extensions:
	thumbnail: Kollarovic\Thumbnail\DI\Extension
```
Configuration
-------------

config.neon

```yaml

thumbnail:
	thumbPathMask: 'images/thumbs/{filename}-{width}x{height}.{extension}'
	placeholder: 'http://dummyimage.com/{width}x{height}/efefef/f00&text=Image+not+found'
    
```

```yaml

thumbPathMask: 'images/thumbs/{md5}/{width}x{height}-{crop}.{extension}'

```

it gets stored in `images/thumbs/e/7/2/e728fdeab7e2edda33f36fbf7a2b7c82/{width}x{height}-{crop}.jpg`

