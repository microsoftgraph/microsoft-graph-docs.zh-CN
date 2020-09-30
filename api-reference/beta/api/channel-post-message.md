---
title: 在频道中创建 chatMessage
description: 在指定的频道中创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6d8ca916ec8e9c358eba1ff0809de41b5a6343e6
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313046"
---
# <a name="create-chatmessage-in-channel"></a><span data-ttu-id="5aeb5-103">在信道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="5aeb5-103">Create chatMessage in channel</span></span>

<span data-ttu-id="5aeb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aeb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aeb5-105">在指定的[频道](../resources/channel.md)中创建新的[了 chatmessage](../resources/chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="5aeb5-106">**注意**：我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="5aeb5-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="5aeb5-108">**注意**：违反使用 Microsoft 团队作为日志文件的 [使用条款](/legal/microsoft-apis/terms-of-use) 。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-108">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="5aeb5-109">仅发送人员将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aeb5-110">权限</span><span class="sxs-lookup"><span data-stu-id="5aeb5-110">Permissions</span></span>

<span data-ttu-id="5aeb5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5aeb5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="5aeb5-113">Permission type</span></span>                        | <span data-ttu-id="5aeb5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5aeb5-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5aeb5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5aeb5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5aeb5-116">ChannelMessage、Group、Group 写。 All</span><span class="sxs-lookup"><span data-stu-id="5aeb5-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="5aeb5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5aeb5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aeb5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-118">Not supported.</span></span> |
| <span data-ttu-id="5aeb5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="5aeb5-119">Application</span></span>                            | <span data-ttu-id="5aeb5-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5aeb5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5aeb5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="5aeb5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5aeb5-122">Request headers</span></span>

| <span data-ttu-id="5aeb5-123">名称</span><span class="sxs-lookup"><span data-stu-id="5aeb5-123">Name</span></span>          | <span data-ttu-id="5aeb5-124">说明</span><span class="sxs-lookup"><span data-stu-id="5aeb5-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5aeb5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aeb5-125">Authorization</span></span> | <span data-ttu-id="5aeb5-126">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-126">Bearer {code}.</span></span> <span data-ttu-id="5aeb5-127">必需。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-127">Required.</span></span> |
| <span data-ttu-id="5aeb5-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="5aeb5-128">Content-type</span></span> | <span data-ttu-id="5aeb5-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5aeb5-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5aeb5-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5aeb5-131">Request body</span></span>

<span data-ttu-id="5aeb5-132">在请求正文中，提供 [了 chatmessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="5aeb5-133">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-133">Only the body property is mandatory, other properties are optional.</span></span>


## <a name="response"></a><span data-ttu-id="5aeb5-134">响应</span><span class="sxs-lookup"><span data-stu-id="5aeb5-134">Response</span></span>

<span data-ttu-id="5aeb5-135">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [了 chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5aeb5-136">示例</span><span class="sxs-lookup"><span data-stu-id="5aeb5-136">Examples</span></span>

<span data-ttu-id="5aeb5-137">有关示例的更完整列表，请参阅 [Create 了 chatmessage in a 信道 or chat](chatmessage-post.md)。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-137">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="5aeb5-138">请求</span><span class="sxs-lookup"><span data-stu-id="5aeb5-138">Request</span></span>
<span data-ttu-id="5aeb5-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5aeb5-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aeb5-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5aeb5-141">C#</span><span class="sxs-lookup"><span data-stu-id="5aeb5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aeb5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aeb5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aeb5-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aeb5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5aeb5-144">响应</span><span class="sxs-lookup"><span data-stu-id="5aeb5-144">Response</span></span>

<span data-ttu-id="5aeb5-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-145">The following is an example of the response.</span></span>

> <span data-ttu-id="5aeb5-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5aeb5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

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