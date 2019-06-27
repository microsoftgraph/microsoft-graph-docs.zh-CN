---
title: 在频道中创建了 chatmessage
description: 在指定的频道中创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2b9398c91137119cecb174dc75bd465b550375f6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262053"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="49a50-103">在频道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="49a50-103">Create chatMessage in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49a50-104">在指定的[频道](../resources/channel.md)中创建新的[了 chatmessage](../resources/chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="49a50-104">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="49a50-105">**注意**: 我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="49a50-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="49a50-106">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="49a50-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="49a50-107">权限</span><span class="sxs-lookup"><span data-stu-id="49a50-107">Permissions</span></span>

<span data-ttu-id="49a50-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49a50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49a50-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="49a50-110">Permission type</span></span>                        | <span data-ttu-id="49a50-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49a50-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49a50-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49a50-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="49a50-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49a50-113">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="49a50-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49a50-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49a50-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="49a50-115">Not supported.</span></span> |
| <span data-ttu-id="49a50-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="49a50-116">Application</span></span>                            | <span data-ttu-id="49a50-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="49a50-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49a50-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49a50-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="49a50-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="49a50-119">Request headers</span></span>

| <span data-ttu-id="49a50-120">名称</span><span class="sxs-lookup"><span data-stu-id="49a50-120">Name</span></span>          | <span data-ttu-id="49a50-121">说明</span><span class="sxs-lookup"><span data-stu-id="49a50-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="49a50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49a50-122">Authorization</span></span> | <span data-ttu-id="49a50-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="49a50-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="49a50-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="49a50-124">Request body</span></span>

<span data-ttu-id="49a50-125">在请求正文中, 提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49a50-125">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="49a50-126">只有 body 属性是必需的, 其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="49a50-126">Only the body property is mandatory, other properties are optional.</span></span>

> <span data-ttu-id="49a50-127">注意: 不支持发送包含附件和图像的邮件。</span><span class="sxs-lookup"><span data-stu-id="49a50-127">Note: Sending messages with attachments and images is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="49a50-128">响应</span><span class="sxs-lookup"><span data-stu-id="49a50-128">Response</span></span>

<span data-ttu-id="49a50-129">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49a50-129">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49a50-130">示例</span><span class="sxs-lookup"><span data-stu-id="49a50-130">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="49a50-131">示例 1: Hello World</span><span class="sxs-lookup"><span data-stu-id="49a50-131">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="49a50-132">请求</span><span class="sxs-lookup"><span data-stu-id="49a50-132">Request</span></span>
<span data-ttu-id="49a50-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49a50-133">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="49a50-134">响应</span><span class="sxs-lookup"><span data-stu-id="49a50-134">Response</span></span>

<span data-ttu-id="49a50-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49a50-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="49a50-136">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49a50-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="49a50-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49a50-137">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="49a50-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="49a50-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="49a50-139">C#</span><span class="sxs-lookup"><span data-stu-id="49a50-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49a50-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="49a50-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="49a50-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="49a50-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_channel-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-mentions"></a><span data-ttu-id="49a50-142">示例 2: @mentions</span><span class="sxs-lookup"><span data-stu-id="49a50-142">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="49a50-143">请求</span><span class="sxs-lookup"><span data-stu-id="49a50-143">Request</span></span>
<span data-ttu-id="49a50-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49a50-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="49a50-145">响应</span><span class="sxs-lookup"><span data-stu-id="49a50-145">Response</span></span>

<span data-ttu-id="49a50-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49a50-146">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="49a50-147">示例 3: 卡片</span><span class="sxs-lookup"><span data-stu-id="49a50-147">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="49a50-148">请求</span><span class="sxs-lookup"><span data-stu-id="49a50-148">Request</span></span>
<span data-ttu-id="49a50-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49a50-149">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="49a50-150">响应</span><span class="sxs-lookup"><span data-stu-id="49a50-150">Response</span></span>

<span data-ttu-id="49a50-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49a50-151">The following is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="49a50-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="49a50-152">See also</span></span>

- [<span data-ttu-id="49a50-153">卡片参考</span><span class="sxs-lookup"><span data-stu-id="49a50-153">Cards Reference</span></span>](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards-reference)

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
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
