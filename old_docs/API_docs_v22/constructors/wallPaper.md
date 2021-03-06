---
title: wallPaper
description: Wallpaper settings.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: wallPaper  
[Back to constructors index](index.md)



Wallpaper settings.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[int](../types/int.md) | Yes|
|title|[string](../types/string.md) | Yes|
|sizes|Array of [PhotoSize](../types/PhotoSize.md) | Yes|
|color|[int](../types/int.md) | Yes|



### Type: [WallPaper](../types/WallPaper.md)


### Example:

```php
$wallPaper = ['_' => 'wallPaper', 'id' => int, 'title' => 'string', 'sizes' => [PhotoSize, PhotoSize], 'color' => int];
```  


Or, if you're into Lua:

```lua
wallPaper={_='wallPaper', id=int, title='string', sizes={PhotoSize}, color=int}

```


