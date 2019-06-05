---
title: 在频道中创建了 chatmessage
description: 在指定的频道中创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0681ded7bb45eea328f9ce6a61f65683aa4d8cf9
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720882"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="c2c17-103">在频道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="c2c17-103">Create chatMessage in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2c17-104">在指定的[频道](../resources/channel.md)中创建新的[了 chatmessage](../resources/chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="c2c17-104">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2c17-105">权限</span><span class="sxs-lookup"><span data-stu-id="c2c17-105">Permissions</span></span>

<span data-ttu-id="c2c17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2c17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2c17-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2c17-108">Permission type</span></span>                        | <span data-ttu-id="c2c17-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2c17-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2c17-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2c17-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2c17-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2c17-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c2c17-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2c17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2c17-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2c17-113">Not supported.</span></span> |
| <span data-ttu-id="c2c17-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2c17-114">Application</span></span>                            | <span data-ttu-id="c2c17-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2c17-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2c17-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2c17-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="c2c17-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2c17-117">Request headers</span></span>

| <span data-ttu-id="c2c17-118">名称</span><span class="sxs-lookup"><span data-stu-id="c2c17-118">Name</span></span>          | <span data-ttu-id="c2c17-119">说明</span><span class="sxs-lookup"><span data-stu-id="c2c17-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c2c17-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2c17-120">Authorization</span></span> | <span data-ttu-id="c2c17-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c2c17-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2c17-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2c17-122">Request body</span></span>

<span data-ttu-id="c2c17-123">在请求正文中, 提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2c17-123">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="c2c17-124">只有 body 属性是必需的, 其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="c2c17-124">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="c2c17-125">注意: 不支持发送包含附件和图像的邮件。</span><span class="sxs-lookup"><span data-stu-id="c2c17-125">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="c2c17-126">响应</span><span class="sxs-lookup"><span data-stu-id="c2c17-126">Response</span></span>

<span data-ttu-id="c2c17-127">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2c17-127">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2c17-128">示例</span><span class="sxs-lookup"><span data-stu-id="c2c17-128">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="c2c17-129">示例 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="c2c17-129">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="c2c17-130">请求</span><span class="sxs-lookup"><span data-stu-id="c2c17-130">Request</span></span>
<span data-ttu-id="c2c17-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2c17-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="c2c17-132">响应</span><span class="sxs-lookup"><span data-stu-id="c2c17-132">Response</span></span>

<span data-ttu-id="c2c17-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2c17-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c2c17-134">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c2c17-134">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c2c17-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c2c17-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2c17-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c2c17-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2c17-137">C#</span><span class="sxs-lookup"><span data-stu-id="c2c17-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2c17-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2c17-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-mentions"></a><span data-ttu-id="c2c17-139">示例 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="c2c17-139">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="c2c17-140">请求</span><span class="sxs-lookup"><span data-stu-id="c2c17-140">Request</span></span>
<span data-ttu-id="c2c17-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2c17-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World <at id=\"0\">Jane Smith</at>"
  },
  "mentions": [
    {
      "id": 0,
      "mentionText": "Jane Smith",
      "mentioned": {
        "user": {
          "displayName": "Jane Smith",
          "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
          "userIdentityType": "aadUser"
        }
      }
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="c2c17-142">响应</span><span class="sxs-lookup"><span data-stu-id="c2c17-142">Response</span></span>

<span data-ttu-id="c2c17-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2c17-143">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World <at id=\"0\">Jane Smith</at>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Jane Smith",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                    "displayName": "Jane Smith",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```

### <a name="example-3-cards"></a><span data-ttu-id="c2c17-144">示例 3: 卡片</span><span class="sxs-lookup"><span data-stu-id="c2c17-144">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="c2c17-145">请求</span><span class="sxs-lookup"><span data-stu-id="c2c17-145">Request</span></span>
<span data-ttu-id="c2c17-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2c17-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
    "subject": null,
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="c2c17-147">响应</span><span class="sxs-lookup"><span data-stu-id="c2c17-147">Response</span></span>

<span data-ttu-id="c2c17-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2c17-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('bdb7bcda-9c3b-4341-b9a9-f52bf9a23407')/channels('19%3A786524f437c042b68bac5c0511ad6be2%40thread.skype')/messages/$entity",
    "id": "1554837297516",
    "replyToId": null,
    "etag": "1554837297516",
    "messageType": "message",
    "createdDateTime": "2019-04-09T19:14:57.516Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.thumbnail",
            "contentUrl": null,
            "content": "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\n\\r\\n\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\n\\r\\n\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="c2c17-149">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c2c17-149">See also</span></span>

- [<span data-ttu-id="c2c17-150">卡片参考</span><span class="sxs-lookup"><span data-stu-id="c2c17-150">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
