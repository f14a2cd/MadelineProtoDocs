---
title: updateChatParticipantAdd
description: New group member.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateChatParticipantAdd  
[Back to constructors index](index.md)



New group member.

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|chat\_id|[int](../types/int.md) | Yes|Group ID|
|user\_id|[int](../types/int.md) | Yes|ID of the new member|
|inviter\_id|[int](../types/int.md) | Yes|ID of the user, who added member to the group|
|version|[int](../types/int.md) | Yes|Chat version number|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateChatParticipantAdd = ['_' => 'updateChatParticipantAdd', 'chat_id' => int, 'user_id' => int, 'inviter_id' => int, 'version' => int];
```  


Or, if you're into Lua:

```lua
updateChatParticipantAdd={_='updateChatParticipantAdd', chat_id=int, user_id=int, inviter_id=int, version=int}

```


