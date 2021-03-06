---
title: updateUserStatus
description: User went online/offline
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateUserStatus  
[Back to constructors index](index.md)



User went online/offline

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|user\_id|[int](../types/int.md) | Yes|User identifier|
|status|[UserStatus](../types/UserStatus.md) | Optional|New user status|



### Type: [Update](../types/Update.md)


### Example:

```php
$updateUserStatus = ['_' => 'updateUserStatus', 'user_id' => int, 'status' => UserStatus];
```  


Or, if you're into Lua:

```lua
updateUserStatus={_='updateUserStatus', user_id=int, status=UserStatus}

```


