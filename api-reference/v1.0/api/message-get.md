---
title: 获取邮件
description: 检索邮件对象的属性和关系。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3dfb0f3d7f6d30bb04b635330a3ceca68b6df9f0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538831"
---
# <a name="get-message"></a>获取邮件

检索[邮件](../resources/message.md)对象的属性和关系。

可使用 `$value` 参数来[获取邮件的 MIME 内容](/graph/outlook-get-mime-message)。

在以下两种情况下，应用可以获取其他用户的邮件文件夹中的邮件：

* 如果该应用具有应用程序权限，或者
* 如果应用具有来自某个用户的相应委派[权限](#permissions)，而另一个用户与该用户共享了邮件文件夹，或者已为该用户授予委派的访问权限。 请参阅[详细信息和示例](/graph/outlook-share-messages-folders)。

由于**邮件**资源支持[扩展](/graph/extensibility-overview)，因此也可使用 `GET` 操作获取**邮件**实例中的自定义属性和扩展数据。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Mail.Read    |
|委派（个人 Microsoft 帐户） | Mail.Read    |
|应用程序 | Mail.Read |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Prefer: outlook.body-content-type | string | 要返回的 **body** 和 **uniqueBody** 属性的格式。 可取值为“text”或“html”。 如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。 如果未指定此头，采用 HTML 格式返回 **body** 和 **uniqueBody** 属性。 可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [message](../resources/message.md) 对象。


## <a name="examples"></a>示例
### <a name="example-1"></a>示例 1
#### <a name="request"></a>请求
下面是一个请求示例。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhMGAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhMGAAA=
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ\"",
    "id":"AAMkADhMGAAA=",
    "createdDateTime":"2018-09-09T03:15:05Z",
    "lastModifiedDateTime":"2018-09-09T03:15:08Z",
    "changeKey":"CQAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAnjjuZ",
    "categories":[

    ],
    "receivedDateTime":"2018-09-09T03:15:08Z",
    "sentDateTime":"2018-09-09T03:15:06Z",
    "hasAttachments":false,
    "internetMessageId":"<MWHPR6E1BE060@MWHPR1120.namprd22.prod.outlook.com>",
    "subject":"9/9/2018: concert",
    "bodyPreview":"The group represents Nevada.",
    "importance":"normal",
    "parentFolderId":"AAMkADcbAAAAAAEJAAA=",
    "conversationId":"AAQkADOUpag6yWs=",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":true,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADMGAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification":"focused",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nThe group represents Nevada.\r\n</body>\r\n</html>\r\n"
    },
    "sender":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "from":{
        "emailAddress":{
            "name":"Adele Vance",
            "address":"adelev@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients":[
        {
            "emailAddress":{
                "name":"Alex Wilber",
                "address":"AlexW@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients":[

    ],
    "bccRecipients":[

    ],
    "replyTo":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

### <a name="example-2"></a>示例 2
#### <a name="request"></a>请求
下一个示例使用 `$select` 查询参数获取邮件的 Internet 邮件标头。 

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADhAAAW-VPeAAA="],
  "name": "get_message_headers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADhAAAW-VPeAAA=/?$select=internetMessageHeaders
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
下面是一个响应示例。 注意：为简洁起见，将截断响应对象中的邮件标头集。 所有标头都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('7f180cbb-a5ae-457c-b7e8-6f5b42ba33e7')/messages(internetMessageHeaders)/$entity",
    "@odata.etag":"W/\"FwAAABYAAAC4ofQHEIqCSbQPot83AFcbAAAW/0tB\"",
    "id":"AAMkADhAAAW-VPeAAA=",
    "internetMessageHeaders":[
        {
            "name":"MIME-Version",
            "value":"1.0"
        },
        {
            "name":"Content-Type",
            "value":"multipart/report"
        },
        {
            "name":"x-custom-header-group-name",
            "value":"Washington"
        },
        {
            "name":"x-custom-header-group-id",
            "value":"WA001"
        }
    ]
}
```

### <a name="example-3"></a>示例 3
#### <a name="request"></a>请求

第三个示例介绍如何使用 `Prefer: outlook.body-content-type="text"` 标头获取采用文本格式的指定消息的 **body** 和 **uniqueBody**。


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面是一个响应示例。 注意：响应包含用于确认 `Prefer: outlook.body-content-type` 请求标头的 `Preference-Applied: outlook.body-content-type` 标头。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
    "body":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
    },
    "uniqueBody":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
    }
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
