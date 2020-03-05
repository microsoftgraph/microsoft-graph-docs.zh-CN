---
title: 在频道中创建 chatMessage 回复
description: 在答复现有的了 chatmessage 对象中创建新的了 chatmessage 对象。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 00d1f9d6d2197f1e265c59a795ef66941c0a5c60
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438300"
---
# <a name="create-chatmessage-reply-in-a-channel"></a><span data-ttu-id="db58f-103">在频道中创建 chatMessage 回复</span><span class="sxs-lookup"><span data-stu-id="db58f-103">Create chatMessage reply in a channel</span></span>

<span data-ttu-id="db58f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="db58f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db58f-105">在答复现有的[了 chatmessage](../resources/chatmessage.md)对象中创建新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="db58f-105">Creates a new [chatMessage](../resources/chatmessage.md) object in reply to an existing [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db58f-106">权限</span><span class="sxs-lookup"><span data-stu-id="db58f-106">Permissions</span></span>

<span data-ttu-id="db58f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db58f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db58f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db58f-109">Permission type</span></span>                        | <span data-ttu-id="db58f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db58f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db58f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db58f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db58f-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db58f-112">Chat.ReadWrite</span></span> |
| <span data-ttu-id="db58f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db58f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db58f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db58f-114">Not supported.</span></span> |
| <span data-ttu-id="db58f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db58f-115">Application</span></span>                            | <span data-ttu-id="db58f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db58f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db58f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db58f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="db58f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db58f-118">Request headers</span></span>

| <span data-ttu-id="db58f-119">名称</span><span class="sxs-lookup"><span data-stu-id="db58f-119">Name</span></span>          | <span data-ttu-id="db58f-120">说明</span><span class="sxs-lookup"><span data-stu-id="db58f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db58f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db58f-121">Authorization</span></span> | <span data-ttu-id="db58f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="db58f-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="db58f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="db58f-123">Request body</span></span>

<span data-ttu-id="db58f-124">在请求正文中，提供[了 chatmessage](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db58f-124">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="db58f-125">响应</span><span class="sxs-lookup"><span data-stu-id="db58f-125">Response</span></span>

<span data-ttu-id="db58f-126">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="db58f-126">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db58f-127">示例</span><span class="sxs-lookup"><span data-stu-id="db58f-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db58f-128">请求</span><span class="sxs-lookup"><span data-stu-id="db58f-128">Request</span></span>

<span data-ttu-id="db58f-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db58f-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db58f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="db58f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chatmessage"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="db58f-131">C#</span><span class="sxs-lookup"><span data-stu-id="db58f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chatmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db58f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db58f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chatmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db58f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db58f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chatmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db58f-134">响应</span><span class="sxs-lookup"><span data-stu-id="db58f-134">Response</span></span>

<span data-ttu-id="db58f-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="db58f-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="db58f-136">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="db58f-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="db58f-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="db58f-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
