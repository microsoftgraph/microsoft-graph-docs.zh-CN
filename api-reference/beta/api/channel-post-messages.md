---
title: 在频道中创建 chatMessage
description: 在指定的频道中创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 59506023c280fbe8d5f18e9b9996815baad3c063
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288590"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="26b52-103">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="26b52-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="26b52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26b52-105">在指定的[频道](../resources/channel.md)中创建新的[了 chatmessage](../resources/chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="26b52-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="26b52-106">**注意**：我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="26b52-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="26b52-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="26b52-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="26b52-108">权限</span><span class="sxs-lookup"><span data-stu-id="26b52-108">Permissions</span></span>

<span data-ttu-id="26b52-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26b52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26b52-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="26b52-111">Permission type</span></span>                        | <span data-ttu-id="26b52-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26b52-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26b52-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26b52-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="26b52-114">ChannelMessage、Group、Group 写。 All</span><span class="sxs-lookup"><span data-stu-id="26b52-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="26b52-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26b52-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b52-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="26b52-116">Not supported.</span></span> |
| <span data-ttu-id="26b52-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="26b52-117">Application</span></span>                            | <span data-ttu-id="26b52-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b52-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26b52-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26b52-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="26b52-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="26b52-120">Request headers</span></span>

| <span data-ttu-id="26b52-121">名称</span><span class="sxs-lookup"><span data-stu-id="26b52-121">Name</span></span>          | <span data-ttu-id="26b52-122">说明</span><span class="sxs-lookup"><span data-stu-id="26b52-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26b52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26b52-123">Authorization</span></span> | <span data-ttu-id="26b52-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="26b52-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26b52-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="26b52-125">Request body</span></span>

<span data-ttu-id="26b52-126">在请求正文中，提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26b52-126">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="26b52-127">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="26b52-127">Only the body property is mandatory, other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="26b52-128">响应</span><span class="sxs-lookup"><span data-stu-id="26b52-128">Response</span></span>

<span data-ttu-id="26b52-129">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26b52-129">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26b52-130">示例</span><span class="sxs-lookup"><span data-stu-id="26b52-130">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="26b52-131">示例1： Hello World</span><span class="sxs-lookup"><span data-stu-id="26b52-131">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="26b52-132">请求</span><span class="sxs-lookup"><span data-stu-id="26b52-132">Request</span></span>
<span data-ttu-id="26b52-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b52-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26b52-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="26b52-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="26b52-135">C#</span><span class="sxs-lookup"><span data-stu-id="26b52-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26b52-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26b52-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26b52-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26b52-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="26b52-138">响应</span><span class="sxs-lookup"><span data-stu-id="26b52-138">Response</span></span>

<span data-ttu-id="26b52-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="26b52-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="26b52-140">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="26b52-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="26b52-141">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26b52-141">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-mentions"></a><span data-ttu-id="26b52-142">示例2： @mentions</span><span class="sxs-lookup"><span data-stu-id="26b52-142">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="26b52-143">请求</span><span class="sxs-lookup"><span data-stu-id="26b52-143">Request</span></span>
<span data-ttu-id="26b52-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b52-144">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="26b52-145">响应</span><span class="sxs-lookup"><span data-stu-id="26b52-145">Response</span></span>

<span data-ttu-id="26b52-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="26b52-146">The following is an example of the response.</span></span>
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

### <a name="example-3-cards"></a><span data-ttu-id="26b52-147">示例3：卡片</span><span class="sxs-lookup"><span data-stu-id="26b52-147">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="26b52-148">请求</span><span class="sxs-lookup"><span data-stu-id="26b52-148">Request</span></span>
<span data-ttu-id="26b52-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b52-149">The following is an example of the request.</span></span>

> <span data-ttu-id="26b52-150">注意：附件的 ID 必须是唯一的，并且可以是一个新的随机生成的 GUID。</span><span class="sxs-lookup"><span data-stu-id="26b52-150">Note: The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="26b52-151">但是，在_正文_和_附件_元素中，附件的 ID 必须相同。</span><span class="sxs-lookup"><span data-stu-id="26b52-151">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>

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

#### <a name="response"></a><span data-ttu-id="26b52-152">响应</span><span class="sxs-lookup"><span data-stu-id="26b52-152">Response</span></span>

<span data-ttu-id="26b52-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="26b52-153">The following is an example of the response.</span></span>
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

### <a name="example-4-file-attachments"></a><span data-ttu-id="26b52-154">示例4：文件附件</span><span class="sxs-lookup"><span data-stu-id="26b52-154">Example 4: File attachments</span></span>

#### <a name="request"></a><span data-ttu-id="26b52-155">请求</span><span class="sxs-lookup"><span data-stu-id="26b52-155">Request</span></span>
<span data-ttu-id="26b52-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26b52-156">The following is an example of the request.</span></span>

><span data-ttu-id="26b52-157">**注意：** 该文件必须已在 SharePoint 中。</span><span class="sxs-lookup"><span data-stu-id="26b52-157">**Note:** The file must already be in SharePoint.</span></span> <span data-ttu-id="26b52-158">若要查找文件属性，请获取文件的**driveItem** 。</span><span class="sxs-lookup"><span data-stu-id="26b52-158">To find the file properties, GET the **driveItem** for the file.</span></span> <span data-ttu-id="26b52-159">例如，/drives/{id}/items/{id}。</span><span class="sxs-lookup"><span data-stu-id="26b52-159">For example, /drives/{id}/items/{id}.</span></span> <span data-ttu-id="26b52-160">附件 ID 是**driveItem**的**ETAG**中的 GUID，附件**contentURL**是**driveItem**的文件夹的**webUrl**以及**driveItem**的名称，而附件名称是**driveItem**的名称。</span><span class="sxs-lookup"><span data-stu-id="26b52-160">Your attachment ID is the GUID in the **eTag** of the **driveItem**, your attachment **contentURL** is the **webUrl** of the **driveItem**'s folder plus the **driveItem**'s name, and your attachment name is the **driveItem**'s name.</span></span>

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
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "name": "Budget.docx"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="26b52-161">响应</span><span class="sxs-lookup"><span data-stu-id="26b52-161">Response</span></span>

<span data-ttu-id="26b52-162">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="26b52-162">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('13a99602-a5d3-4fed-99d2-7dc3ffe3730d')/channels('19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2')/messages/$entity",
    "id": "1589481435511",
    "replyToId": null,
    "etag": "1589481435511",
    "messageType": "message",
    "createdDateTime": "2020-05-14T18:37:15.511Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2/1589481435511?groupId=13a99602-a5d3-4fed-99d2-7dc3ffe3730d&tenantId=e5648b2b-1dea-445a-ab65-4f9326c2bd10&createdTime=1589481435511&parentMessageId=1589481435511",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "598efcd4-e549-402a-9602-0b50201faebe",
            "displayName": "MOD Administrator",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    "attachments": [
        {
            "id": "153fa47d-18c9-4179-be08-9879815a9f90",
            "contentType": "reference",
            "contentUrl": "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            "content": null,
            "name": "Budget.docx",
            "thumbnailUrl": null
        }
    ],
    "mentions": [],
    "reactions": []
}
```

## <a name="see-also"></a><span data-ttu-id="26b52-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="26b52-163">See also</span></span>

- [<span data-ttu-id="26b52-164">卡参考</span><span class="sxs-lookup"><span data-stu-id="26b52-164">Cards reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

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
