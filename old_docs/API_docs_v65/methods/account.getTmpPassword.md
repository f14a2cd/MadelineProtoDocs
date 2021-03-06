---
title: account.getTmpPassword
description: Get temporary payment password
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/account_getTmpPassword.html
---
# Method: account.getTmpPassword  
[Back to methods index](index.md)


Get temporary payment password

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|password\_hash|[bytes](../types/bytes.md) | The password hash | Yes|
|period|[int](../types/int.md) | Time during which the temporary password will be valid, in seconds; should be between 60 and 86400 | Yes|


### Return type: [account.TmpPassword](../types/account.TmpPassword.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$account.TmpPassword = $MadelineProto->account->getTmpPassword(['password_hash' => 'bytes', 'period' => int, ]);
```

Or, if you're into Lua:

```lua
account.TmpPassword = account.getTmpPassword({password_hash='bytes', period=int, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|PASSWORD_HASH_INVALID|The provided password hash is invalid|
|400|TMP_PASSWORD_DISABLED|The temporary password is disabled|


