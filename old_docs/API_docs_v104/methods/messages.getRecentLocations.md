---
title: messages.getRecentLocations
description: Get live location history of a certain user
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_getRecentLocations.html
---
# Method: messages.getRecentLocations  
[Back to methods index](index.md)


Get live location history of a certain user

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | User | Optional|
|limit|[int](../types/int.md) | Maximum number of results to return, [see pagination](https://core.telegram.org/api/offsets) | Yes|
|hash|Array of [int](../types/int.md) | IDs of locations you already fetched | Optional|


### Return type: [messages.Messages](../types/messages.Messages.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages.Messages = $MadelineProto->messages->getRecentLocations(['peer' => InputPeer, 'limit' => int, 'hash' => [int, int], ]);
```

Or, if you're into Lua:

```lua
messages.Messages = messages.getRecentLocations({peer=InputPeer, limit=int, hash={int}, })
```

