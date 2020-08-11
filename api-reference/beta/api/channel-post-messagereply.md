---
title: 答复频道中的邮件
description: 在渠道中回复现有消息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 135815f373799fa0f75e104894b61d54115a476c
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630261"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="1a0ea-103">答复频道中的邮件</span><span class="sxs-lookup"><span data-stu-id="1a0ea-103">Reply to a message in a channel</span></span>

<span data-ttu-id="1a0ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a0ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a0ea-105">在指定[频道](../resources/channel.md)中创建对[了 chatmessage](../resources/chatmessage.md)的新答复。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="1a0ea-106">**注意**：我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="1a0ea-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="1a0ea-108">**注意**：违反使用 Microsoft 团队作为日志文件的[使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use)。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-108">**Note**: It is a violation of the [terms of use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="1a0ea-109">仅发送人员将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a0ea-110">权限</span><span class="sxs-lookup"><span data-stu-id="1a0ea-110">Permissions</span></span>
<span data-ttu-id="1a0ea-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a0ea-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a0ea-113">Permission type</span></span>      | <span data-ttu-id="1a0ea-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a0ea-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a0ea-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a0ea-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1a0ea-116">ChannelMessage、Group、Group 写。 All</span><span class="sxs-lookup"><span data-stu-id="1a0ea-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="1a0ea-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a0ea-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a0ea-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-118">Not supported.</span></span>    |
|<span data-ttu-id="1a0ea-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a0ea-119">Application</span></span> | <span data-ttu-id="1a0ea-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a0ea-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a0ea-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="1a0ea-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a0ea-122">Request headers</span></span>
| <span data-ttu-id="1a0ea-123">名称</span><span class="sxs-lookup"><span data-stu-id="1a0ea-123">Name</span></span>       | <span data-ttu-id="1a0ea-124">类型</span><span class="sxs-lookup"><span data-stu-id="1a0ea-124">Type</span></span> | <span data-ttu-id="1a0ea-125">说明</span><span class="sxs-lookup"><span data-stu-id="1a0ea-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1a0ea-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a0ea-126">Authorization</span></span>  | <span data-ttu-id="1a0ea-127">string</span><span class="sxs-lookup"><span data-stu-id="1a0ea-127">string</span></span>  | <span data-ttu-id="1a0ea-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a0ea-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a0ea-130">Request body</span></span>
<span data-ttu-id="1a0ea-131">在请求正文中，提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="1a0ea-132">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="1a0ea-133">响应</span><span class="sxs-lookup"><span data-stu-id="1a0ea-133">Response</span></span>

<span data-ttu-id="1a0ea-134">如果成功，此方法 `201 Created` 将在已创建的[邮件](../resources/chatmessage.md)中返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="1a0ea-135">示例</span><span class="sxs-lookup"><span data-stu-id="1a0ea-135">Example</span></span>

<span data-ttu-id="1a0ea-136">有关示例的更完整列表，请参阅[Create 了 chatmessage in a 信道 or chat](chatmessage-post.md)。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-136">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="1a0ea-137">请求</span><span class="sxs-lookup"><span data-stu-id="1a0ea-137">Request</span></span>
<span data-ttu-id="1a0ea-138">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a0ea-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a0ea-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="1a0ea-140">C#</span><span class="sxs-lookup"><span data-stu-id="1a0ea-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a0ea-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a0ea-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a0ea-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a0ea-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a0ea-143">响应</span><span class="sxs-lookup"><span data-stu-id="1a0ea-143">Response</span></span>

<span data-ttu-id="1a0ea-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1a0ea-144">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
