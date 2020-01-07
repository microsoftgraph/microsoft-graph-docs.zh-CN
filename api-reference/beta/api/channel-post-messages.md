---
title: 在频道中创建 chatMessage
description: 在指定的频道中创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 65ee5bcd763a065873fe795a1638c33b4610ded2
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951665"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="ccfdc-103">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="ccfdc-103">Create chatMessage in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccfdc-104">在指定的[频道](../resources/channel.md)中创建新的[了 chatmessage](../resources/chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-104">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="ccfdc-105">**注意**：我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="ccfdc-106">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccfdc-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ccfdc-107">Permissions</span></span>

<span data-ttu-id="ccfdc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccfdc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccfdc-110">Permission type</span></span>                        | <span data-ttu-id="ccfdc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccfdc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ccfdc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccfdc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccfdc-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccfdc-113">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ccfdc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccfdc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccfdc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-115">Not supported.</span></span> |
| <span data-ttu-id="ccfdc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccfdc-116">Application</span></span>                            | <span data-ttu-id="ccfdc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccfdc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccfdc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="ccfdc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccfdc-119">Request headers</span></span>

| <span data-ttu-id="ccfdc-120">名称</span><span class="sxs-lookup"><span data-stu-id="ccfdc-120">Name</span></span>          | <span data-ttu-id="ccfdc-121">说明</span><span class="sxs-lookup"><span data-stu-id="ccfdc-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ccfdc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccfdc-122">Authorization</span></span> | <span data-ttu-id="ccfdc-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ccfdc-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccfdc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccfdc-124">Request body</span></span>

<span data-ttu-id="ccfdc-125">在请求正文中，提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-125">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="ccfdc-126">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-126">Only the body property is mandatory, other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="ccfdc-127">响应</span><span class="sxs-lookup"><span data-stu-id="ccfdc-127">Response</span></span>

<span data-ttu-id="ccfdc-128">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-128">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccfdc-129">示例</span><span class="sxs-lookup"><span data-stu-id="ccfdc-129">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="ccfdc-130">示例1： Hello World</span><span class="sxs-lookup"><span data-stu-id="ccfdc-130">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="ccfdc-131">请求</span><span class="sxs-lookup"><span data-stu-id="ccfdc-131">Request</span></span>
<span data-ttu-id="ccfdc-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ccfdc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccfdc-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ccfdc-134">C#</span><span class="sxs-lookup"><span data-stu-id="ccfdc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ccfdc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccfdc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ccfdc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccfdc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccfdc-137">响应</span><span class="sxs-lookup"><span data-stu-id="ccfdc-137">Response</span></span>

<span data-ttu-id="ccfdc-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ccfdc-139">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ccfdc-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-140">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-mentions"></a><span data-ttu-id="ccfdc-141">示例2： @mentions</span><span class="sxs-lookup"><span data-stu-id="ccfdc-141">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="ccfdc-142">请求</span><span class="sxs-lookup"><span data-stu-id="ccfdc-142">Request</span></span>
<span data-ttu-id="ccfdc-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-143">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ccfdc-144">响应</span><span class="sxs-lookup"><span data-stu-id="ccfdc-144">Response</span></span>

<span data-ttu-id="ccfdc-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-145">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="ccfdc-146">示例3：卡片</span><span class="sxs-lookup"><span data-stu-id="ccfdc-146">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="ccfdc-147">请求</span><span class="sxs-lookup"><span data-stu-id="ccfdc-147">Request</span></span>
<span data-ttu-id="ccfdc-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-148">The following is an example of the request.</span></span>

> <span data-ttu-id="ccfdc-149">注意：附件的 ID 必须是唯一的，并且可以是一个新的随机生成的 GUID。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-149">Note: The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="ccfdc-150">但是，在_正文_和_附件_元素中，附件的 ID 必须相同。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-150">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>

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

#### <a name="response"></a><span data-ttu-id="ccfdc-151">响应</span><span class="sxs-lookup"><span data-stu-id="ccfdc-151">Response</span></span>

<span data-ttu-id="ccfdc-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ccfdc-152">The following is an example of the response.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ccfdc-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ccfdc-153">See also</span></span>

- [<span data-ttu-id="ccfdc-154">卡片参考</span><span class="sxs-lookup"><span data-stu-id="ccfdc-154">Cards Reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

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
  ]
}
-->
