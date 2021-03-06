---
title: channels.checkUsername
description: Check if a username is free and can be assigned to a channel/supergroup
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/channels_checkUsername.html
---
# Method: channels.checkUsername  
[Back to methods index](index.md)


Check if a username is free and can be assigned to a channel/supergroup

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|channel|[Username, chat ID, Update, Message or InputChannel](../types/InputChannel.md) | The [channel/supergroup](https://core.telegram.org/api/channel) that will assigned the specified username | Optional|
|username|[string](../types/string.md) | The username to check | Yes|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->channels->checkUsername(['channel' => InputChannel, 'username' => 'string', ]);
```

Or, if you're into Lua:

```lua
Bool = channels.checkUsername({channel=InputChannel, username='string', })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|CHANNEL_INVALID|The provided channel is invalid|
|400|CHAT_ID_INVALID|The provided chat id is invalid|
|400|USERNAME_INVALID|The provided username is not valid|


