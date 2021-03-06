---
title: chatFull
description: Detailed chat info
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: chatFull  
[Back to constructors index](index.md)



Detailed chat info

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|[int](../types/int.md) | Yes|ID of the chat|
|participants|[ChatParticipants](../types/ChatParticipants.md) | Yes|Participant list|
|chat\_photo|[Photo](../types/Photo.md) | Optional|Chat photo|
|notify\_settings|[PeerNotifySettings](../types/PeerNotifySettings.md) | Yes|Notification settings|
|exported\_invite|[ExportedChatInvite](../types/ExportedChatInvite.md) | Yes|Chat invite|
|bot\_info|Array of [BotInfo](../types/BotInfo.md) | Yes|Info about bots that are in this chat|



### Type: [ChatFull](../types/ChatFull.md)


### Example:

```php
$chatFull = ['_' => 'chatFull', 'id' => int, 'participants' => ChatParticipants, 'chat_photo' => Photo, 'notify_settings' => PeerNotifySettings, 'exported_invite' => ExportedChatInvite, 'bot_info' => [BotInfo, BotInfo]];
```  


Or, if you're into Lua:

```lua
chatFull={_='chatFull', id=int, participants=ChatParticipants, chat_photo=Photo, notify_settings=PeerNotifySettings, exported_invite=ExportedChatInvite, bot_info={BotInfo}}

```


