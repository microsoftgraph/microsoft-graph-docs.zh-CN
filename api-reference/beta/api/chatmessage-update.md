---
title: 更新 chatMessage
description: 更新 chatMessage 对象的属性。
author: RamjotSingh
doc_type: apiPageType
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: 0033ad1375cfb5120f88041531a8237c14c760fb
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768264"
---
# <a name="update-chatmessage"></a>更新 chatMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


更新 [chatMessage](../resources/chatMessage.md) 对象。 除了 **policyViolation** 属性外， **聊天Message** 的所有属性都可以在委派权限方案中更新。
在应用程序权限方案中，只能更新 **chatMessage** 的 **policyViolation** 属性。

[!INCLUDE [teams-model-A-only-disclaimer](../../includes/teams-model-A-only-disclaimer.md)]

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Chat.ReadWrite |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 聊天消息的 Chat.UpdatePolicyViolation.All。</br>频道消息的 ChannelMessage.UpdatePolicyViolation.All。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/messages/{message-id}
PATCH /teams/(team-id)/channels/{channel-id}/messages/{message-id}/replies/{reply-id}
PATCH /chats/{chatThread-id}/messages/{message-id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

可以使用 `model` 查询参数，该参数仅支持该值 `A`，如以下示例所示。

```http
PATCH /teams/(team-id)/channels/{channel-id}/messages/{message-id}?model=A
PATCH /teams/(team-id)/channels/{channel-id}/messages/{message-id}/replies/{reply-id}?model=A
PATCH /chats/{chatThread-id}/messages/{message-id}?model=A
```
如果未指定 `model`，将使用 [评估模式](/graph/teams-licenses#evaluation-mode-default-requirements)。 

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Content-Type | application/json. Required. |

## <a name="request-body"></a>请求正文
对于使用委派权限的应用程序：在请求正文中，提供 [chatMessage 对象的](../resources/chatMessage.md) JSON 表示形式，指定需要更改的属性。

对于使用应用程序权限的应用程序：在请求正文中，提供 [chatMessage](../resources/chatMessage.md) 对象的 JSON 表示形式，仅指定 **policyViolation** 属性。

## <a name="response-body"></a>响应正文
对于使用委派权限的应用程序：如果成功，此方法将返回 `204 NoContent` 响应。

对于使用应用程序权限的应用程序：如果成功，此方法将返回 `200 OK` 响应。

## <a name="example-for-updating-policyviolation-by-using-application-permissions"></a>使用应用程序权限更新 policyViolation 的示例

#### <a name="request"></a>请求

下面是请求使用应用程序权限更新 Microsoft Teams 通道消息上的 **policyViolation** 属性的示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chatMessage.PatchPolicyViolation.All"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json

{
  "policyViolation": {
    "policyTip": {
      "generalText" : "This item has been blocked by the administrator.",
      "complianceUrl" : "https://contoso.com/dlp-policy-page",
      "matchedConditionDescriptions" : ["Credit Card Number"]
    },
    "verdictDetails" : "AllowOverrideWithoutJustification,AllowFalsePositiveOverride",
    "dlpAction" : "BlockAccess"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chatmessagepatchpolicyviolationall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chatmessagepatchpolicyviolationall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chatmessagepatchpolicyviolationall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chatmessagepatchpolicyviolationall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chatmessagepatchpolicyviolationall-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/chatmessagepatchpolicyviolationall-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessage.UpdatePolicyViolation.All",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


## <a name="example-for-updating-any-property-of-a-message-by-using-delegated-permissions"></a>使用委派权限更新消息的任何属性的示例

#### <a name="request"></a>请求

下面是请求使用委派权限更新 Microsoft Teams 频道消息上的属性的示例。

<!-- {
  "blockType": "request",
  "name": "patch_chatMessage_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json

{
  "messageType": "message",
  "subject": null,
  "summary": null,
  "importance": "normal",
  "locale": "en-us",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "3b102402-813e-4e17-a6b2-f841aef1fdfc",
      "displayName": "Sumit Gupta",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "Edit text only"
  },
  "attachments": [],
  "mentions": [],
  "reactions": []
}
```

#### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 204 NoContent
```

### <a name="request-to-update-the-mentions-of-a-message-by-using-delegated-permissions"></a>请求使用委派权限更新对消息的提及

下面是请求使用委派权限更新 Microsoft Teams 频道消息上的提及的示例。

<!-- {
  "blockType": "request",
  "name": "patch_chatMessage_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json

{
  "messageType": "message",
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "importance": "normal",
  "locale": "en-us",
  "from": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "6b3f3c54-d09c-4fdd-b146-9b514a8a4f40",
      "displayName": "Sumit Gupta",
      "userIdentityType": "aadUser"
    }
  },
  "body": {
    "contentType": "html",
    "content": "<div><div>\n<div>\n<div>\n<div>\n<div><at id=\"0\">Raghav</at><at id=\"1\">TestGlobalBot</at> YEAH"
  },
  "attachments": [],
  "mentions": [
    {
      "id": 0,
      "mentionText": "Raghav",
      "mentioned": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "f1b66449-b46d-49b0-9c3c-53c10234c818e",
          "displayName": "Raghav Mankad",
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "id": 1,
      "mentionText": "TestGlobalBot",
      "mentioned": {
        "application": {
          "id": "03a02232-d8f5-4970-a77e-6e8c76ce7a4e",
          "displayName": "TestGlobalBot",
          "applicationIdentityType": "bot"
        },
        "device": null,
        "conversation": null,
        "user": null
      }
    }
  ],
  "reactions": []
}
```

#### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 204 NoContent
```

### <a name="request-to-update-the-content-with-attachments-of-a-message-by-using-delegated-permissions"></a>使用委派权限使用邮件附件更新内容的请求

下面是请求使用委派权限更新 Microsoft Teams 频道消息上的附件的示例。

<!-- {
  "blockType": "request",
  "name": "patch_chatMessage_3"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json

{
  "messageType": "message",
  "subject": null,
  "summary": null,
  "importance": "normal",
  "locale": "en-us",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "3b102402-813e-4e17-a6b2-f841aef1fdfc",
      "displayName": "Sumit Gupta",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "html",
    "content": "<p><em>text</em></p><attachment id=\"e8f78756199240b88448ae0fc6db112d\"></attachment><attachment id=\"638464e32834471ea202007da60a5ae6\"></attachment>"
  },
  "attachments": [
    {
      "id": "e8f78756199240b88448ae0fc6db112d",
      "contentType": "application/vnd.microsoft.card.hero",
      "contentUrl": null,
      "content": "{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you're cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"image\": \"https://urlp.asm.skype.com/v1/url/content?url=https%3a%2f%2fcdn2.iconfinder.com%2fdata%2ficons%2fsocial-icons-33%2f128%2fTrello-128.png\",\r\n      \"title\": \"😃😃 click me 😃😃\",\r\n      \"value\": \"http://microsoft.com\"\r\n    },\r\n    {\r\n      \"type\": \"imback\",\r\n      \"title\": \"&i am back& <>= \\\"\",\r\n      \"value\": \"&i am back& <>= \\\"\"\r\n    },\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"title\": \"Open URL\",\r\n      \"value\": \"http://google.com\"\r\n    }\r\n  ]\r\n}",
      "name": null,
      "thumbnailUrl": null
    },
    {
      "id": "638464e32834471ea202007da60a5ae6",
      "contentType": "application/vnd.microsoft.card.hero",
      "contentUrl": null,
      "content": "{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you're cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"&message back& <>= \\\"\",\r\n      \"text\": \"text = &message back& <>= \\\"\",\r\n      \"displayText\": \"displayText = &message back& <>= \\\"\",\r\n      \"value\": {\r\n        \"text\": \"some text 2\"\r\n      }\r\n    }\r\n  ]\r\n}",
      "name": null,
      "thumbnailUrl": null
    }
  ],
  "mentions": [],
  "reactions": []
}
```

#### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 204 NoContent
```

### <a name="request-to-update-the-reactions-in-a-message-by-using-delegated-permissions"></a>请求使用委派权限更新消息中的反应

下面是请求使用委派权限更新 Microsoft Teams 通道消息上响应属性的示例。


<!-- {
  "blockType": "request",
  "name": "patch_chatMessage_4"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json

{
  "messageType": "message",
  "subject": null,
  "summary": null,
  "importance": "normal",
  "locale": "en-us",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "3b102402-813e-4e17-a6b2-f841aef1fdfc",
      "displayName": "Sumit Gupta",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "html",
    "content": "<p><em>text</em></p><attachment id=\"e8f78756199240b88448ae0fc6db112d\"></attachment><attachment id=\"638464e32834471ea202007da60a5ae6\"></attachment>"
  },
  "attachments": [
    {
      "id": "e8f78756199240b88448ae0fc6db112d",
      "contentType": "application/vnd.microsoft.card.hero",
      "contentUrl": null,
      "content": "{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you're cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"image\": \"https://urlp.asm.skype.com/v1/url/content?url=https%3a%2f%2fcdn2.iconfinder.com%2fdata%2ficons%2fsocial-icons-33%2f128%2fTrello-128.png\",\r\n      \"title\": \"😃😃 click me 😃😃\",\r\n      \"value\": \"http://microsoft.com\"\r\n    },\r\n    {\r\n      \"type\": \"imback\",\r\n      \"title\": \"&i am back& <>= \\\"\",\r\n      \"value\": \"&i am back& <>= \\\"\"\r\n    },\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"title\": \"Open URL\",\r\n      \"value\": \"http://google.com\"\r\n    }\r\n  ]\r\n}",
      "name": null,
      "thumbnailUrl": null
    },
    {
      "id": "638464e32834471ea202007da60a5ae6",
      "contentType": "application/vnd.microsoft.card.hero",
      "contentUrl": null,
      "content": "{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you're cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"&message back& <>= \\\"\",\r\n      \"text\": \"text = &message back& <>= \\\"\",\r\n      \"displayText\": \"displayText = &message back& <>= \\\"\",\r\n      \"value\": {\r\n        \"text\": \"some text 2\"\r\n      }\r\n    }\r\n  ]\r\n}",
      "name": null,
      "thumbnailUrl": null
    }
  ],
  "mentions": [],
  "reactions": [
    {
      "reactionType": "angry",
      "createdDateTime": "2018-10-21T08:10:30.489Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "f1b66449-b46d-49b0-9c3c-53c10a5c818e",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "reactionType": "laugh",
      "createdDateTime": "2018-10-21T08:10:32.489Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "03a02232-d8f5-4970-a77e-6e8c76ce7a4e",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "reactionType": "like",
      "createdDateTime": "2018-10-21T02:17:14.67Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "f1b66449-b46d-49b0-9c3c-53c10a5c818e",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "reactionType": "like",
      "createdDateTime": "2018-10-21T02:34:40.3Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "4c9041b7-449a-40f7-8855-56da239b9fd1",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "reactionType": "like",
      "createdDateTime": "2018-10-21T08:10:25.489Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "03a02232-d8f5-4970-a77e-6e8c76ce7a4e",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "reactionType": "heart",
      "createdDateTime": "2018-10-21T08:10:31.489Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "03a02232-d8f5-4970-a77e-6e8c76ce7a4e",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "reactionType": "sad",
      "createdDateTime": "2018-10-21T08:10:33.489Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "03a02232-d8f5-4970-a77e-6e8c76ce7a4e",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    },
    {
      "reactionType": "surprised",
      "createdDateTime": "2018-10-21T08:10:34.489Z",
      "user": {
        "application": null,
        "device": null,
        "user": {
          "id": "03a02232-d8f5-4970-a77e-6e8c76ce7a4e",
          "displayName": null,
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

#### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 204 NoContent
```
