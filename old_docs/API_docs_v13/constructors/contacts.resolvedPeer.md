---
title: contacts.resolvedPeer
description: Resolved peer
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/contacts_resolvedPeer.html
---
# Constructor: contacts.resolvedPeer  
[Back to constructors index](index.md)



Resolved peer

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|peer|[Peer](../types/Peer.md) | Yes|The peer|
|chats|Array of [Chat](../types/Chat.md) | Yes|Chats|
|users|Array of [User](../types/User.md) | Yes|Users|



### Type: [contacts.ResolvedPeer](../types/contacts.ResolvedPeer.md)


### Example:

```php
$contacts.resolvedPeer = ['_' => 'contacts.resolvedPeer', 'peer' => Peer, 'chats' => [Chat, Chat], 'users' => [User, User]];
```  


Or, if you're into Lua:

```lua
contacts.resolvedPeer={_='contacts.resolvedPeer', peer=Peer, chats={Chat}, users={User}}

```


