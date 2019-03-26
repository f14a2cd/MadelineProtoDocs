---
title: channels.createChannel
description: Create channel/supergroup
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: channels.createChannel  
[Back to methods index](index.md)


Create channel/supergroup

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|broadcast|[Bool](../types/Bool.md) | Set this to true to create a channel | Optional|
|megagroup|[Bool](../types/Bool.md) | Set this to true to create a supergroup | Optional|
|title|[string](../types/string.md) | Supergroup/channel title | Yes|
|about|[string](../types/string.md) | About text | Yes|


### Return type: [Updates](../types/Updates.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
define('MADELINE_BRANCH', '');
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Updates = $MadelineProto->channels->createChannel(['broadcast' => Bool, 'megagroup' => Bool, 'title' => 'string', 'about' => 'string', ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/channels.createChannel`

Parameters:

broadcast - Json encoded Bool

megagroup - Json encoded Bool

title - Json encoded string

about - Json encoded string




Or, if you're into Lua:

```lua
Updates = channels.createChannel({broadcast=Bool, megagroup=Bool, title='string', about='string', })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|CHAT_TITLE_EMPTY|No chat title provided|
|USER_RESTRICTED|You're spamreported, you can't create channels or chats.|

