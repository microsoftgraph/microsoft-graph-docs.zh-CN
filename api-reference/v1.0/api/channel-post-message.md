---
title: 在频道中创建 chatMessage
description: 在指定的频道中创建新的 chatMessage。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a40f4f34b8eda962a9ce7b80fefa6b4c5b372d26
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202773"
---
# <a name="create-chatmessage-in-a-channel"></a><span data-ttu-id="86b1f-103">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="86b1f-103">Create chatMessage in a channel</span></span>

<span data-ttu-id="86b1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86b1f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86b1f-105">在指定的[频道中创建新的 chatMessage。](../resources/chatmessage.md) [](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="86b1f-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="86b1f-106">**注意**：不建议使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="86b1f-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="86b1f-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="86b1f-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="86b1f-108">权限</span><span class="sxs-lookup"><span data-stu-id="86b1f-108">Permissions</span></span>

<span data-ttu-id="86b1f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86b1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86b1f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="86b1f-111">Permission type</span></span>                        | <span data-ttu-id="86b1f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86b1f-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86b1f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86b1f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="86b1f-114">ChannelMessage.Send、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86b1f-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="86b1f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86b1f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86b1f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86b1f-116">Not supported.</span></span> |
| <span data-ttu-id="86b1f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86b1f-117">Application</span></span>                            | <span data-ttu-id="86b1f-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="86b1f-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="86b1f-119">**注意**：仅迁移 *支持应用程序*[权限](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="86b1f-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="86b1f-120">将来，Microsoft 可能要求你或你的客户根据导入的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="86b1f-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="86b1f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86b1f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="86b1f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="86b1f-122">Request headers</span></span>

| <span data-ttu-id="86b1f-123">名称</span><span class="sxs-lookup"><span data-stu-id="86b1f-123">Name</span></span>          | <span data-ttu-id="86b1f-124">说明</span><span class="sxs-lookup"><span data-stu-id="86b1f-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="86b1f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="86b1f-125">Authorization</span></span> | <span data-ttu-id="86b1f-126">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="86b1f-126">Bearer {code}.</span></span> <span data-ttu-id="86b1f-127">必需。</span><span class="sxs-lookup"><span data-stu-id="86b1f-127">Required.</span></span> |
| <span data-ttu-id="86b1f-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="86b1f-128">Content-type</span></span> | <span data-ttu-id="86b1f-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="86b1f-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86b1f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="86b1f-131">Request body</span></span>

<span data-ttu-id="86b1f-132">在请求正文中，提供 [chatMessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86b1f-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="86b1f-133">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="86b1f-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="86b1f-134">响应</span><span class="sxs-lookup"><span data-stu-id="86b1f-134">Response</span></span>

<span data-ttu-id="86b1f-135">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [chatMessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86b1f-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86b1f-136">示例</span><span class="sxs-lookup"><span data-stu-id="86b1f-136">Examples</span></span>

### <a name="example-1-hello-world"></a><span data-ttu-id="86b1f-137">示例 1：Hello World</span><span class="sxs-lookup"><span data-stu-id="86b1f-137">Example 1: Hello World</span></span>

#### <a name="request"></a><span data-ttu-id="86b1f-138">请求</span><span class="sxs-lookup"><span data-stu-id="86b1f-138">Request</span></span>

<span data-ttu-id="86b1f-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86b1f-139">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```


#### <a name="response"></a><span data-ttu-id="86b1f-140">响应</span><span class="sxs-lookup"><span data-stu-id="86b1f-140">Response</span></span>

<span data-ttu-id="86b1f-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86b1f-141">The following is an example of the response.</span></span>

> <span data-ttu-id="86b1f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86b1f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-2-mentions"></a><span data-ttu-id="86b1f-144">示例 2：@mentions</span><span class="sxs-lookup"><span data-stu-id="86b1f-144">Example 2: @mentions</span></span>

#### <a name="request"></a><span data-ttu-id="86b1f-145">请求</span><span class="sxs-lookup"><span data-stu-id="86b1f-145">Request</span></span>
<span data-ttu-id="86b1f-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86b1f-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86b1f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="86b1f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
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
# <a name="c"></a>[<span data-ttu-id="86b1f-148">C#</span><span class="sxs-lookup"><span data-stu-id="86b1f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86b1f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86b1f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86b1f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86b1f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="86b1f-151">响应</span><span class="sxs-lookup"><span data-stu-id="86b1f-151">Response</span></span>

<span data-ttu-id="86b1f-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86b1f-152">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-3-cards"></a><span data-ttu-id="86b1f-153">示例 3：卡片</span><span class="sxs-lookup"><span data-stu-id="86b1f-153">Example 3: Cards</span></span>

#### <a name="request"></a><span data-ttu-id="86b1f-154">请求</span><span class="sxs-lookup"><span data-stu-id="86b1f-154">Request</span></span>
<span data-ttu-id="86b1f-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86b1f-155">The following is an example of the request.</span></span>

><span data-ttu-id="86b1f-156">**注意：** 附件的 ID 必须是唯一的，并且可以是随机生成的新 GUID。</span><span class="sxs-lookup"><span data-stu-id="86b1f-156">**Note:** The attachment's ID must be unique and can be a new randomly generated GUID.</span></span> <span data-ttu-id="86b1f-157">但是，附件的 ID 在 _body_ 和 attachments 元素中 _必须_ 相同。</span><span class="sxs-lookup"><span data-stu-id="86b1f-157">However, the attachment's ID must be the same in the _body_ and _attachments_ elements.</span></span>


# <a name="http"></a>[<span data-ttu-id="86b1f-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="86b1f-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
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
# <a name="c"></a>[<span data-ttu-id="86b1f-159">C#</span><span class="sxs-lookup"><span data-stu-id="86b1f-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86b1f-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86b1f-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86b1f-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86b1f-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86b1f-162">Java</span><span class="sxs-lookup"><span data-stu-id="86b1f-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="86b1f-163">响应</span><span class="sxs-lookup"><span data-stu-id="86b1f-163">Response</span></span>

<span data-ttu-id="86b1f-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86b1f-164">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-4-file-attachments"></a><span data-ttu-id="86b1f-165">示例 4：文件附件</span><span class="sxs-lookup"><span data-stu-id="86b1f-165">Example 4: File attachments</span></span>

#### <a name="request"></a><span data-ttu-id="86b1f-166">请求</span><span class="sxs-lookup"><span data-stu-id="86b1f-166">Request</span></span>
<span data-ttu-id="86b1f-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86b1f-167">The following is an example of the request.</span></span>

><span data-ttu-id="86b1f-168">**注意：** 文件必须已经在 SharePoint 中。</span><span class="sxs-lookup"><span data-stu-id="86b1f-168">**Note:** The file must already be in SharePoint.</span></span> <span data-ttu-id="86b1f-169">若要查找文件属性，请获取 **文件的 driveItem。**</span><span class="sxs-lookup"><span data-stu-id="86b1f-169">To find the file properties, GET the **driveItem** for the file.</span></span> <span data-ttu-id="86b1f-170">例如，/drives/{id}/items/{id}。</span><span class="sxs-lookup"><span data-stu-id="86b1f-170">For example, /drives/{id}/items/{id}.</span></span> <span data-ttu-id="86b1f-171">附件 ID 是 **driveItem** 的 **eTag** 中的 GUID，附件 contentURL 是 **driveItem** 文件夹的 **webUrl** 加上 **driveItem** 的名称，附件名称是 **driveItem** 的名称。 </span><span class="sxs-lookup"><span data-stu-id="86b1f-171">Your attachment ID is the GUID in the **eTag** of the **driveItem**, your attachment **contentURL** is the **webUrl** of the **driveItem**'s folder plus the **driveItem**'s name, and your attachment name is the **driveItem**'s name.</span></span>


# <a name="http"></a>[<span data-ttu-id="86b1f-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="86b1f-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
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
# <a name="c"></a>[<span data-ttu-id="86b1f-173">C#</span><span class="sxs-lookup"><span data-stu-id="86b1f-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86b1f-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86b1f-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86b1f-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86b1f-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86b1f-176">Java</span><span class="sxs-lookup"><span data-stu-id="86b1f-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="86b1f-177">响应</span><span class="sxs-lookup"><span data-stu-id="86b1f-177">Response</span></span>

<span data-ttu-id="86b1f-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86b1f-178">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-5-import-messages"></a><span data-ttu-id="86b1f-179">示例 5：导入邮件</span><span class="sxs-lookup"><span data-stu-id="86b1f-179">Example 5: Import messages</span></span>

> <span data-ttu-id="86b1f-180">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="86b1f-180">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="86b1f-181">请求</span><span class="sxs-lookup"><span data-stu-id="86b1f-181">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="86b1f-182">以下示例显示如何使用 请求正文中的 和 键导入 `createDateTime` `from` 实时邮件。</span><span class="sxs-lookup"><span data-stu-id="86b1f-182">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "deleted":false,
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
}
```

#### <a name="response"></a><span data-ttu-id="86b1f-183">响应</span><span class="sxs-lookup"><span data-stu-id="86b1f-183">Response</span></span>

<span data-ttu-id="86b1f-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86b1f-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
   "id":"id-value",
   "replyToId":null,
   "etag":"id-value",
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

### <a name="example-6-import-messages-with-inline-images"></a><span data-ttu-id="86b1f-185">示例 6：导入包含内嵌图像的邮件</span><span class="sxs-lookup"><span data-stu-id="86b1f-185">Example 6: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="86b1f-186">目前，内联图像是导入邮件 API 架构支持的唯一媒体类型。</span><span class="sxs-lookup"><span data-stu-id="86b1f-186">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="86b1f-187">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="86b1f-187">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="86b1f-188">请求</span><span class="sxs-lookup"><span data-stu-id="86b1f-188">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="86b1f-189">以下示例演示如何使用 请求正文中的 和 键导入包含内嵌图像的 `createDateTime` `from` 返回时间邮件。</span><span class="sxs-lookup"><span data-stu-id="86b1f-189">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
{
   "body":{
      "contentType":"html",
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"../hostedContents/1/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "hostedContents":[
      {
         "@microsoft.graph.temporaryId":"1",
         "contentBytes":"iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>",
         "contentType":"image/png"
      }
   ]
}
```

#### <a name="response"></a><span data-ttu-id="86b1f-190">响应</span><span class="sxs-lookup"><span data-stu-id="86b1f-190">Response</span></span>

<span data-ttu-id="86b1f-191">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86b1f-191">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
   "id":"id-value",
   "replyToId":null,
   "etag":"id-value",
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"https://graph.microsoft.com/teams/teamId/channels/channelId/messages/id-value/hostedContents/hostedContentId/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}

```

## <a name="see-also"></a><span data-ttu-id="86b1f-192">另请参阅</span><span class="sxs-lookup"><span data-stu-id="86b1f-192">See also</span></span>

* [<span data-ttu-id="86b1f-193">卡参考</span><span class="sxs-lookup"><span data-stu-id="86b1f-193">Cards reference</span></span>](/microsoftteams/platform/concepts/cards/cards-reference)
* [<span data-ttu-id="86b1f-194">使用 Microsoft Graph 将第三方平台消息导入 Teams</span><span class="sxs-lookup"><span data-stu-id="86b1f-194">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="86b1f-195">创建频道</span><span class="sxs-lookup"><span data-stu-id="86b1f-195">Create channel</span></span>](channel-post.md)

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

