---
title: 在渠道中回复消息
description: 在渠道中回复现有消息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 040f439fcdcb8caa6c0b1a08594b60626bfe4665
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864422"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="96c9b-103">在渠道中回复消息</span><span class="sxs-lookup"><span data-stu-id="96c9b-103">Reply to a message in a channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96c9b-104">在指定的[频道](../resources/channel.md)中创建对[邮件](../resources/chatmessage.md)的新答复。</span><span class="sxs-lookup"><span data-stu-id="96c9b-104">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="96c9b-105">**注意**: 我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="96c9b-105">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="96c9b-106">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="96c9b-106">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="96c9b-107">权限</span><span class="sxs-lookup"><span data-stu-id="96c9b-107">Permissions</span></span>
<span data-ttu-id="96c9b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96c9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96c9b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96c9b-110">Permission type</span></span>      | <span data-ttu-id="96c9b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96c9b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96c9b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96c9b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96c9b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96c9b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96c9b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96c9b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96c9b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96c9b-115">Not supported.</span></span>    |
|<span data-ttu-id="96c9b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="96c9b-116">Application</span></span> | <span data-ttu-id="96c9b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="96c9b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96c9b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96c9b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```
## <a name="request-headers"></a><span data-ttu-id="96c9b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96c9b-119">Request headers</span></span>
| <span data-ttu-id="96c9b-120">名称</span><span class="sxs-lookup"><span data-stu-id="96c9b-120">Name</span></span>       | <span data-ttu-id="96c9b-121">类型</span><span class="sxs-lookup"><span data-stu-id="96c9b-121">Type</span></span> | <span data-ttu-id="96c9b-122">说明</span><span class="sxs-lookup"><span data-stu-id="96c9b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96c9b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96c9b-123">Authorization</span></span>  | <span data-ttu-id="96c9b-124">string</span><span class="sxs-lookup"><span data-stu-id="96c9b-124">string</span></span>  | <span data-ttu-id="96c9b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96c9b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96c9b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="96c9b-127">Request body</span></span>
<span data-ttu-id="96c9b-128">在请求正文中, 提供[message](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96c9b-128">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="96c9b-129">只有 body 属性是必需的, 其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="96c9b-129">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="96c9b-130">响应</span><span class="sxs-lookup"><span data-stu-id="96c9b-130">Response</span></span>

<span data-ttu-id="96c9b-131">如果成功, 此方法将`201 Created`在已创建的[邮件](../resources/chatmessage.md)中返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="96c9b-131">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="96c9b-132">示例</span><span class="sxs-lookup"><span data-stu-id="96c9b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96c9b-133">请求</span><span class="sxs-lookup"><span data-stu-id="96c9b-133">Request</span></span>
<span data-ttu-id="96c9b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96c9b-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96c9b-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="96c9b-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="96c9b-136">C#</span><span class="sxs-lookup"><span data-stu-id="96c9b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96c9b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="96c9b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96c9b-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="96c9b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96c9b-139">Java</span><span class="sxs-lookup"><span data-stu-id="96c9b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96c9b-140">响应</span><span class="sxs-lookup"><span data-stu-id="96c9b-140">Response</span></span>

<span data-ttu-id="96c9b-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="96c9b-141">Here is an example of the response.</span></span>
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
