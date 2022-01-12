---
title: 使用 Microsoft Graph API 获取 Microsoft Teams 的系统消息
description: 了解 Microsoft Teams 如何使用 Microsoft Graph API 为事件生成系统消息。
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5c3aa7cb7d922805e94099db302de1f361783474
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860906"
---
# <a name="get-system-messages-for-microsoft-teams-using-microsoft-graph-apis"></a>使用 Microsoft Graph API 获取 Microsoft Teams 的系统消息

Microsoft Teams 为添加到聊天中的成员、已更新团队名称和已更新频道说明等事件生成系统消息。 通过系统消息，调用方可以深入了解团队、频道或聊天中发生的事件。


Microsoft Graph 将系统消息作为 [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-v1.0&preserve-view=true) GET 操作和 [聊天和频道消息的更改通知](teams-changenotifications-chatmessage.md)的一部分公开。


系统消息显示为 [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-v1.0&preserve-view=true) 对象。
在这种情况下，**messageType** 属性设置为 `systemEventMessage`，并且 **eventDetail** 属性提供事件详细信息。


## <a name="supported-get-operations"></a>支持的 GET 操作

以下 GET 操作支持系统消息：

- GET /teams/{team-id}/channel/{channel-id}/messages
- GET /teams/{team-td}/channel/{channel-id}/messages/{message-id}
- GET /chats/{chat-id}/messages
- GET /chats/{chat-id}/messages/{message-id}

有关详细信息，请参阅 [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-v1.0&preserve-view=true)。

## <a name="supported-change-notifications"></a>支持的更改通知

以下更改通知支持系统消息：

- 订阅频道中的消息 - /teams/{team-id}/channels/{channel-id}/messages
- 订阅聊天中的消息 - /chats/{chat-id}/messages

有关详细信息，请参阅 [更改消息的通知](teams-changenotifications-chatmessage.md)。


## <a name="supported-system-message-events"></a>支持的系统消息事件

| 事件   |  系统消息类型   | 适用于 |
|:--------|:--------------|:--------------|
| 已结束通话 | [callEndedEventMessageDetail](#call-ended) | 聊天，频道 |
| 通话记录 | [callRecordingEventMessageDetail](#call-recording) | 聊天，频道 |
| 已开始通话 | [callStartedEventMessageDetail](#call-started) | 聊天，频道 |
| 通话脚本 | [callTranscriptEventMessageDetail](#call-transcript) | 聊天，频道 |
| 已添加频道 | [channelAddedEventMessageDetail](#channel-added) | 团队 |
| 已删除频道 | [channelDeletedEventMessageDetail](#channel-deleted) | 团队 |
| 已更新频道说明 | [channelDescriptionUpdatedEventMessageDetail](#channel-description-updated) | 频道 |
| 已重命名频道 | [channelRenamedEventMessageDetail](#channel-renamed) | 频道 |
| 已将频道设置为书签 | [channelSetAsFavoriteByDefaultEventMessageDetail](#channel-set-as-favorite-by-default) | 频道 |
| 已取消将频道设置为书签 | [channelUnsetAsFavoriteByDefaultEventMessageDetail](#channel-unset-as-favorite-by-default) | 频道 |
| 已重命名聊天 | [chatRenamedEventMessageDetail](#chat-renamed) | 聊天 |
| 已更新对话成员角色 | [conversationMemberRoleUpdatedEventMessageDetail](#conversation-member-role-updated) | 频道，团队 |
| 已更新会议策略 | [meetingPolicyUpdatedEventMessageDetail](#meeting-policy-updated) | 聊天 |
| 已添加成员。 | [membersAddedEventMessageDetail](#members-added) | 聊天，频道，团队 |
| 已删除成员 | [membersDeletedEventMessageDetail](#members-deleted) | 聊天，频道，团队 |
| 已加入成员 | [membersJoinedEventMessageDetail](#members-joined) | 聊天 |
| 剩余成员 | [membersLeftEventMessageDetail](#members-left) | 聊天 |
| 已更新选项卡 | [tabUpdatedEventMessageDetail](#tab-updated) | 聊天，频道 |
| 已存档团队 | [teamArchivedEventMessageDetail](#team-archived) | 团队 |
| 已创建团队 | [teamCreatedEventMessageDetail](#team-created) | 团队 |
| 已更新说明 | [teamDescriptionUpdatedEventMessageDetail](#team-description-updated) | 团队 |
| 已禁用团队加入 | [teamJoiningDisabledEventMessageDetail](#team-joining-disabled) | 团队 |
| 已启用团队加入 | [teamJoiningEnabledEventMessageDetail](#team-joining-enabled) | 团队 |
| 已重命名团队 | [teamRenamedEventMessageDetail](#team-renamed) | 团队 |
| 已安装 Teams 应用 | [teamsAppInstalledEventMessageDetail](#teams-app-installed) | 聊天，频道，团队 |
| 已删除 Teams 应用 | [teamsAppRemovedEventMessageDetail](#teams-app-removed) | 聊天，频道，团队 |
| 已升级 Teams 应用 | [teamsAppUpgradedEventMessageDetail](#teams-app-upgraded) | 聊天，频道，团队 |
| 未存档团队 | [teamUnarchivedEventMessageDetail](#team-unarchived) | 团队 |


> **注意：** 适用于团队的系统消息在主频道中发布。


## <a name="json-response-examples"></a>JSON 响应示例

以下 JSON 示例显示每个受支持事件类型的响应。

### <a name="call-ended"></a>已结束通话

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callEndedEventMessageDetail",
    "callId": "9c848c0e-f906-4dfc-b22e-c68a785a587c",
    "callDuration": "PT59S",
    "callEventType": "meeting",
    "callParticipants": [{
      "participant": {
        "application": null,
        "device": null,
        "user": {
          "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
          "displayName": "Adele Vance ",
          "userIdentityType": "aadUser"
        }
      }
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-recording"></a>通话记录

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callRecordingEventMessageDetail",
    "callId": "c86c6052-410b-4e7c-b843-9a09f576e4d5",
    "callRecordingDisplayName": "Meeting Recording.mp4",
    "callRecordingUrl": "https://testtenant.sharepoint.com/sites/TestTeam/Shared%20Documents/General/Recordings/Meeting%20Recording.mp4?web=1",
    "callRecordingDuration": "PT40M19.26S",
    "callRecordingStatus": "success",
    "meetingOrganizer": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    },
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-started"></a>已开始通话

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callStartedEventMessageDetail",
    "callId": "9c848c0e-f906-4dfc-b22e-c68a785a587c",
    "callEventType": "call",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-transcript"></a>通话脚本

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callTranscriptEventMessageDetail",
    "callId": "5b927778-760b-429e-8c4e-65b1802dd6c9",
    "callTranscriptICalUid": "040000008200E00074C5B7101A82E00800000000002C743F89CDD601000000000000000010000000CA87F90D9372ED45A399B5D75E854EE9 ",
    "meetingOrganizer": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-added"></a>已添加频道

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelAddedEventMessageDetail",
    "channelId": "19:e84f079882f44fa8bebb7343b9e8921a@thread.tacv2",
    "channelDisplayName": "Standard channel",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-deleted"></a>已删除频道

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelDeletedEventMessageDetail",
    "channelId": "19:914b8c83915548c0bff588e510a6cf01@thread.tacv2",
    "channelDisplayName": "Standard channel",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-description-updated"></a>已更新频道说明

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "channelDescription": "Channel description updated",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-renamed"></a>已重命名频道

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "channelDisplayName": "Standard channel rename",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-set-as-favorite-by-default"></a>频道默认设置为收藏夹

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-unset-as-favorite-by-default"></a>频道默认取消设置为收藏夹

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="chat-renamed"></a>已重命名聊天

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.chatRenamedEventMessageDetail",
    "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
    "chatDisplayName": "Microsoft Teams Members",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="conversation-member-role-updated"></a>已更新对话成员角色

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
    "conversationMemberRoles": [
      "Owner"
    ],
    "conversationMemberUser": {
      "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
      "displayName": null,
      "userIdentityType": "aadUser"
    },
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="meeting-policy-updated"></a>已更新会议策略

```json
{
  "id": "1620732126822",
  "replyToId": null,
  "etag": "1620732126822",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-11T11:22:06.822Z",
  "lastModifiedDateTime": "2021-05-11T11:22:06.822Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
    "meetingChatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
    "meetingChatEnabled": true,
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-added"></a>已添加成员。

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersAddedEventMessageDetail",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
    "members": [{
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      },
      {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    ],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-deleted"></a>已删除成员

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersDeletedEventMessageDetail",
    "members": [{
      "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
      "displayName": null,
      "userIdentityType": "aadUser"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-joined"></a>已加入成员

```json
{
  "id": "1620050140712",
  "replyToId": null,
  "etag": "1620050140712",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T13:55:40.712Z",
  "lastModifiedDateTime": "2021-05-03T13:55:40.712Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersJoinedEventMessageDetail",
    "members": [{
      "id": "2c3f5f34-ac9f-42e7-8b35-442ccac166cb",
      "displayName": "Alex (Guest)",
      "userIdentityType": "aadUser"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-left"></a>剩余成员

```json
{
  "id": "1620049976741",
  "replyToId": null,
  "etag": "1620049976741",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T13:52:56.741Z",
  "lastModifiedDateTime": "2021-05-03T13:52:56.741Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "onBehalfOf": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersLeftEventMessageDetail",
    "members": [{
      "id": "ee8af8acd3184068a935a1f207865620",
      "displayName": "Alex (Guest)",
      "userIdentityType": "anonymousGuest"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="tab-updated"></a>已更新选项卡

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.tabUpdatedEventMessageDetail",
    "tabId": "tab::e82fa916-3c9a-407e-806b-0b9d8d7492c0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-archived"></a>已存档团队

```json
{
  "id": "1623677858199",
  "replyToId": null,
  "etag": "1623677858199",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:37:38.199Z",
  "lastModifiedDateTime": "2021-06-14T13:37:38.199Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623677858199?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623677858199&parentMessageId=1623677858199",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamArchivedEventMessageDetail",
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-created"></a>已创建团队

```json
{
  "id": "1623677858199",
  "replyToId": null,
  "etag": "1623677858199",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:37:38.199Z",
  "lastModifiedDateTime": "2021-06-14T13:37:38.199Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623677858199?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623677858199&parentMessageId=1623677858199",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamCreatedEventMessageDetail",
    "teamId": "19:715b7c2ea0894fe3a503f8958df1ef06@thread.tacv2",
    "teamDisplayName": "Test Team",
    "teamDescription": "This is a test team.",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-description-updated"></a>已更新说明

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "teamDescription": "Team description updated",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-joining-disabled"></a>已禁用团队加入

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamJoiningDisabledEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-joining-enabled"></a>已启用团队加入

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamJoiningEnabledEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-renamed"></a>已重命名团队

```json
{
  "id": "1618821548765",
  "replyToId": null,
  "etag": "1618821548765",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-19T08:39:08.765Z",
  "lastModifiedDateTime": "2021-04-19T08:39:08.765Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618821548765?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618821548765&parentMessageId=1618821548765",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamRenamedEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "teamDisplayName": "Team rename",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-installed"></a>已安装 Teams 应用

```json
{
  "id": "1620046494994",
  "replyToId": null,
  "etag": "1620046494994",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:54:54.994Z",
  "lastModifiedDateTime": "2021-05-03T12:54:54.994Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046494994?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046494994&parentMessageId=1620046494994",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppInstalledEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-removed"></a>已删除 Teams 应用

```json
{
  "id": "1620046597520",
  "replyToId": null,
  "etag": "1620046597520",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:56:37.52Z",
  "lastModifiedDateTime": "2021-05-03T12:56:37.52Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046597520?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046597520&parentMessageId=1620046597520",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppRemovedEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-upgraded"></a>已升级 Teams 应用

```json
{
  "id": "1620046597520",
  "replyToId": null,
  "etag": "1620046597520",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:56:37.52Z",
  "lastModifiedDateTime": "2021-05-03T12:56:37.52Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046597520?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046597520&parentMessageId=1620046597520",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppUpgradedEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-unarchived"></a>未存档团队

```json
{
  "id": "1623678060910",
  "replyToId": null,
  "etag": "1623678060910",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:41:00.91Z",
  "lastModifiedDateTime": "2021-06-14T13:41:00.91Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623678060910?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623678060910&parentMessageId=1623678060910",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "onBehalfOf": null,
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamUnarchivedEventMessageDetail",
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```
