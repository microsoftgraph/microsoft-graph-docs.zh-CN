---
title: 创建了 chatmessage
description: 使用此 API 创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 784c275f3006af144b56c7de17758492f13e8db1
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418164"
---
# <a name="create-chatmessage"></a><span data-ttu-id="01614-103">创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="01614-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01614-104">在指定的[聊天](../resources/chat.md)中创建新[邮件](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="01614-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01614-105">权限</span><span class="sxs-lookup"><span data-stu-id="01614-105">Permissions</span></span>

<span data-ttu-id="01614-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01614-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="01614-108">Permission type</span></span>                        | <span data-ttu-id="01614-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01614-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="01614-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01614-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="01614-111">聊天读</span><span class="sxs-lookup"><span data-stu-id="01614-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="01614-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01614-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01614-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="01614-113">Not supported.</span></span> |
| <span data-ttu-id="01614-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="01614-114">Application</span></span>                            | <span data-ttu-id="01614-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01614-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01614-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01614-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="01614-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="01614-117">Request headers</span></span>

| <span data-ttu-id="01614-118">名称</span><span class="sxs-lookup"><span data-stu-id="01614-118">Name</span></span>          | <span data-ttu-id="01614-119">说明</span><span class="sxs-lookup"><span data-stu-id="01614-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="01614-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="01614-120">Authorization</span></span> | <span data-ttu-id="01614-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="01614-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="01614-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="01614-122">Request body</span></span>

<span data-ttu-id="01614-123">在请求正文中, 提供[了 chatmessage](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01614-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="01614-124">响应</span><span class="sxs-lookup"><span data-stu-id="01614-124">Response</span></span>

<span data-ttu-id="01614-125">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01614-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01614-126">示例</span><span class="sxs-lookup"><span data-stu-id="01614-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01614-127">请求</span><span class="sxs-lookup"><span data-stu-id="01614-127">Request</span></span>

<span data-ttu-id="01614-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01614-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01614-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="01614-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01614-130">C#</span><span class="sxs-lookup"><span data-stu-id="01614-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01614-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01614-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01614-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="01614-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01614-133">响应</span><span class="sxs-lookup"><span data-stu-id="01614-133">Response</span></span>

<span data-ttu-id="01614-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="01614-134">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="01614-135">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="01614-135">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="01614-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01614-136">All the properties will be returned from an actual call.</span></span>

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
