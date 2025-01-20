# Firebase Cloud Messaging Payload

#### Android Chat Notification Payload
```json
{
    "message": {
        "token": "<FCM_TOKEN>",
        "data": {
            "type": "chat",
            "group_name": "Room Name",
            "group_id": "group_identifier",
            "sender_id": "sender_identifier",
            "sender_name": "Sender Name",
            "message": "Message content",
            "icon": "notification_icon",
            "avatar": "avatar_url"
        }
    }
}
```

#### iOS Chat Notification Payload
```json
{
    "message": {
        "token": "<FCM_TOKEN>",
        "apns": {
            "payload": {
                "aps": {
                    "alert": {
                        "title": "Sender Name",
                        "body": "Message Content"
                    },
                    "mutable-content": 1,
                    "content-available": 1,
                    "sound": "default"
                }
            }
        },
        "data": {
            "type": "chat",
            "group_name": "Room Name",
            "group_id": "group_identifier",
            "group_avatar": "group_avatar_url",
            "sender_id": "sender_identifier",
            "sender_name": "Sender Name",
            "message": "Message content",
            "avatar": "sender_avatar_url"
        }
    }
}
```

#### Standard Notification Payload
```json
{
    "message": {
        "token": "<FCM_TOKEN>",
        "notifications": {
            "title": "Notification Title",
            "body": "Notification Content"
        }
    }
}
```
