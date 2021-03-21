---
title: 在频道中创建 chatMessage
description: 在指定的频道中创建新的 chatMessage。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6301daf2c51818c5f967bd163939beffbd9a7a6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964273"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="ba22f-103">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="ba22f-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="ba22f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba22f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba22f-105">在指定的[频道中创建新的 chatMessage。](../resources/chatmessage.md) [](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="ba22f-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="ba22f-106">**注意**：不建议使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="ba22f-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="ba22f-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="ba22f-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba22f-108">权限</span><span class="sxs-lookup"><span data-stu-id="ba22f-108">Permissions</span></span>

<span data-ttu-id="ba22f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba22f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba22f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba22f-111">Permission type</span></span>                        | <span data-ttu-id="ba22f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba22f-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba22f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba22f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba22f-114">ChannelMessage.Send、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba22f-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ba22f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba22f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba22f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba22f-116">Not supported.</span></span> |
| <span data-ttu-id="ba22f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba22f-117">Application</span></span>                            | <span data-ttu-id="ba22f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba22f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba22f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba22f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="ba22f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba22f-120">Request headers</span></span>

| <span data-ttu-id="ba22f-121">名称</span><span class="sxs-lookup"><span data-stu-id="ba22f-121">Name</span></span>          | <span data-ttu-id="ba22f-122">说明</span><span class="sxs-lookup"><span data-stu-id="ba22f-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ba22f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba22f-123">Authorization</span></span> | <span data-ttu-id="ba22f-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="ba22f-124">Bearer {code}.</span></span> <span data-ttu-id="ba22f-125">必需。</span><span class="sxs-lookup"><span data-stu-id="ba22f-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba22f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba22f-126">Request body</span></span>

<span data-ttu-id="ba22f-127">在请求正文中，提供 message 对象的 JSON [表示](../resources/chatmessage.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="ba22f-127">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="ba22f-128">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="ba22f-128">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="ba22f-129">响应</span><span class="sxs-lookup"><span data-stu-id="ba22f-129">Response</span></span>

<span data-ttu-id="ba22f-130">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [chatMessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba22f-130">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba22f-131">示例</span><span class="sxs-lookup"><span data-stu-id="ba22f-131">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="ba22f-132">示例 1：Hello World</span><span class="sxs-lookup"><span data-stu-id="ba22f-132">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="ba22f-133">请求</span><span class="sxs-lookup"><span data-stu-id="ba22f-133">Request</span></span>

<span data-ttu-id="ba22f-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba22f-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba22f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba22f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="ba22f-136">C#</span><span class="sxs-lookup"><span data-stu-id="ba22f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba22f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba22f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba22f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba22f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba22f-139">Java</span><span class="sxs-lookup"><span data-stu-id="ba22f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ba22f-140">响应</span><span class="sxs-lookup"><span data-stu-id="ba22f-140">Response</span></span>

<span data-ttu-id="ba22f-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba22f-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ba22f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba22f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

### <a name="example-2-mentions"></a><span data-ttu-id="ba22f-144">示例 2：@mentions</span><span class="sxs-lookup"><span data-stu-id="ba22f-144">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="ba22f-145">请求</span><span class="sxs-lookup"><span data-stu-id="ba22f-145">Request</span></span>
<span data-ttu-id="ba22f-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba22f-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ba22f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba22f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
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
# <a name="c"></a>[<span data-ttu-id="ba22f-148">C#</span><span class="sxs-lookup"><span data-stu-id="ba22f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba22f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba22f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba22f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba22f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ba22f-151">响应</span><span class="sxs-lookup"><span data-stu-id="ba22f-151">Response</span></span>

<span data-ttu-id="ba22f-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba22f-152">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

### <a name="example-3-cards"></a><span data-ttu-id="ba22f-153">示例 3：卡片</span><span class="sxs-lookup"><span data-stu-id="ba22f-153">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="ba22f-154">请求</span><span class="sxs-lookup"><span data-stu-id="ba22f-154">Request</span></span>
<span data-ttu-id="ba22f-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba22f-155">The following is an example of the request.</span></span>

><span data-ttu-id="ba22f-156">**注意：** 附件的 ID 必须是唯一的，并且可以是随机生成的新 GUID。</span><span class="sxs-lookup"><span data-stu-id="ba22f-156">**Note:** The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="ba22f-157">但是，附件的 ID 在 _body_ 和 attachments 元素中 _必须_ 相同。</span><span class="sxs-lookup"><span data-stu-id="ba22f-157">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba22f-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba22f-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
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
# <a name="c"></a>[<span data-ttu-id="ba22f-159">C#</span><span class="sxs-lookup"><span data-stu-id="ba22f-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba22f-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba22f-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba22f-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba22f-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba22f-162">Java</span><span class="sxs-lookup"><span data-stu-id="ba22f-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ba22f-163">响应</span><span class="sxs-lookup"><span data-stu-id="ba22f-163">Response</span></span>

<span data-ttu-id="ba22f-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba22f-164">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('bdb7bcda-9c3b-4341-b9a9-f52bf9a23407')/channels('19%3A786524f437c042b68bac5c0511ad6be2%40thread.skype')/messages/$entity",
    "id": "1554837297516",
    "replyToId": null,
    "etag": "1554837297516",
    "messageType": "message",
    "createdDateTime": "2019-04-09T19:14:57.516Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

### <a name="example-4-file-attachments"></a><span data-ttu-id="ba22f-165">示例 4：文件附件</span><span class="sxs-lookup"><span data-stu-id="ba22f-165">Example 4: File attachments</span></span>

#### <a name="request"></a><span data-ttu-id="ba22f-166">请求</span><span class="sxs-lookup"><span data-stu-id="ba22f-166">Request</span></span>
<span data-ttu-id="ba22f-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba22f-167">The following is an example of the request.</span></span>

><span data-ttu-id="ba22f-168">**注意：** 文件必须已经在 SharePoint 中。</span><span class="sxs-lookup"><span data-stu-id="ba22f-168">**Note:** The file must already be in SharePoint.</span></span> <span data-ttu-id="ba22f-169">若要查找文件属性，请获取 **文件的 driveItem。**</span><span class="sxs-lookup"><span data-stu-id="ba22f-169">To find the file properties, GET the **driveItem** for the file.</span></span> <span data-ttu-id="ba22f-170">例如，/drives/{id}/items/{id}。</span><span class="sxs-lookup"><span data-stu-id="ba22f-170">For example, /drives/{id}/items/{id}.</span></span> <span data-ttu-id="ba22f-171">附件 ID 是 **driveItem** 的 **eTag** 中的 GUID，附件 contentURL 是 **driveItem** 文件夹的 **webUrl** 加上 **driveItem** 的名称，附件名称是 **driveItem** 的名称。 </span><span class="sxs-lookup"><span data-stu-id="ba22f-171">Your attachment ID is the GUID in the **eTag** of the **driveItem**, your attachment **contentURL** is the **webUrl** of the **driveItem**'s folder plus the **driveItem**'s name, and your attachment name is the **driveItem**'s name.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba22f-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba22f-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages
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
# <a name="c"></a>[<span data-ttu-id="ba22f-173">C#</span><span class="sxs-lookup"><span data-stu-id="ba22f-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba22f-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba22f-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba22f-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba22f-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba22f-176">Java</span><span class="sxs-lookup"><span data-stu-id="ba22f-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ba22f-177">响应</span><span class="sxs-lookup"><span data-stu-id="ba22f-177">Response</span></span>

<span data-ttu-id="ba22f-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba22f-178">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('13a99602-a5d3-4fed-99d2-7dc3ffe3730d')/channels('19%3A8af03d1e70f5455fbb74d36acbe2957f%40thread.tacv2')/messages/$entity",
    "id": "1589481435511",
    "replyToId": null,
    "etag": "1589481435511",
    "messageType": "message",
    "createdDateTime": "2020-05-14T18:37:15.511Z",
    "lastModifiedDateTime":"2020-07-04T19:58:15.511Z",
    "lastEditedDateTime": null,
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

## <a name="see-also"></a><span data-ttu-id="ba22f-179">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ba22f-179">See also</span></span>

- [<span data-ttu-id="ba22f-180">卡参考</span><span class="sxs-lookup"><span data-stu-id="ba22f-180">Cards reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)

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

