---
title: 答复频道中的邮件
description: 在渠道中回复现有消息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1ee31b18c17da5ea038115adb17fd362363030c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364325"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="33888-103">答复频道中的邮件</span><span class="sxs-lookup"><span data-stu-id="33888-103">Reply to a message in a channel</span></span>

<span data-ttu-id="33888-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33888-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33888-105">在指定的[频道](../resources/channel.md)中创建对[邮件](../resources/chatmessage.md)的新答复。</span><span class="sxs-lookup"><span data-stu-id="33888-105">Create a new reply to a [message](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="33888-106">**注意**：我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="33888-106">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="33888-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="33888-107">It does not have the throughput necessary for a typical migration.</span></span>

## <a name="permissions"></a><span data-ttu-id="33888-108">权限</span><span class="sxs-lookup"><span data-stu-id="33888-108">Permissions</span></span>

<span data-ttu-id="33888-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33888-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33888-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="33888-111">Permission type</span></span>      | <span data-ttu-id="33888-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33888-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33888-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33888-113">Delegated (work or school account)</span></span> | <span data-ttu-id="33888-114">ChannelMessage、Group、Group 写。 All</span><span class="sxs-lookup"><span data-stu-id="33888-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="33888-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33888-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33888-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="33888-116">Not supported.</span></span>    |
| <span data-ttu-id="33888-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="33888-117">Application</span></span>                           | <span data-ttu-id="33888-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="33888-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="33888-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33888-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="33888-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="33888-120">Request headers</span></span>

| <span data-ttu-id="33888-121">名称</span><span class="sxs-lookup"><span data-stu-id="33888-121">Name</span></span>       | <span data-ttu-id="33888-122">类型</span><span class="sxs-lookup"><span data-stu-id="33888-122">Type</span></span> | <span data-ttu-id="33888-123">说明</span><span class="sxs-lookup"><span data-stu-id="33888-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33888-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33888-124">Authorization</span></span>  | <span data-ttu-id="33888-125">string</span><span class="sxs-lookup"><span data-stu-id="33888-125">string</span></span>  | <span data-ttu-id="33888-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33888-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33888-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="33888-128">Request body</span></span>

<span data-ttu-id="33888-129">在请求正文中，提供 [message](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33888-129">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="33888-130">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="33888-130">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="33888-131">响应</span><span class="sxs-lookup"><span data-stu-id="33888-131">Response</span></span>

<span data-ttu-id="33888-132">如果成功，此方法 `201 Created` 将在已创建的 [邮件](../resources/chatmessage.md) 中返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="33888-132">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example"></a><span data-ttu-id="33888-133">示例</span><span class="sxs-lookup"><span data-stu-id="33888-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="33888-134">请求</span><span class="sxs-lookup"><span data-stu-id="33888-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="33888-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="33888-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="33888-136">C#</span><span class="sxs-lookup"><span data-stu-id="33888-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33888-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33888-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33888-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33888-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33888-139">Java</span><span class="sxs-lookup"><span data-stu-id="33888-139">Java</span></span>](#tab/java) 
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="33888-140">响应</span><span class="sxs-lookup"><span data-stu-id="33888-140">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
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
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
