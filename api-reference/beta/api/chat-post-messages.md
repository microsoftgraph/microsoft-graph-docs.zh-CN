---
title: 创建了 chatmessage
description: 使用此 API 创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cb9f939e6c58ce83ad1386e9303d95978e0a6d58
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261450"
---
# <a name="create-chatmessage"></a><span data-ttu-id="8b8ff-103">创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8b8ff-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b8ff-104">在指定的[聊天](../resources/chat.md)中创建新[邮件](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b8ff-105">权限</span><span class="sxs-lookup"><span data-stu-id="8b8ff-105">Permissions</span></span>

<span data-ttu-id="8b8ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b8ff-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b8ff-108">Permission type</span></span>                        | <span data-ttu-id="8b8ff-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b8ff-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b8ff-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b8ff-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b8ff-111">聊天读</span><span class="sxs-lookup"><span data-stu-id="8b8ff-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="8b8ff-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b8ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b8ff-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-113">Not supported.</span></span> |
| <span data-ttu-id="8b8ff-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b8ff-114">Application</span></span>                            | <span data-ttu-id="8b8ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b8ff-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b8ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="8b8ff-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b8ff-117">Request headers</span></span>

| <span data-ttu-id="8b8ff-118">名称</span><span class="sxs-lookup"><span data-stu-id="8b8ff-118">Name</span></span>          | <span data-ttu-id="8b8ff-119">说明</span><span class="sxs-lookup"><span data-stu-id="8b8ff-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8b8ff-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b8ff-120">Authorization</span></span> | <span data-ttu-id="8b8ff-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8b8ff-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b8ff-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b8ff-122">Request body</span></span>

<span data-ttu-id="8b8ff-123">在请求正文中, 提供[了 chatmessage](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8b8ff-124">响应</span><span class="sxs-lookup"><span data-stu-id="8b8ff-124">Response</span></span>

<span data-ttu-id="8b8ff-125">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b8ff-126">示例</span><span class="sxs-lookup"><span data-stu-id="8b8ff-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b8ff-127">请求</span><span class="sxs-lookup"><span data-stu-id="8b8ff-127">Request</span></span>

<span data-ttu-id="8b8ff-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8b8ff-129">响应</span><span class="sxs-lookup"><span data-stu-id="8b8ff-129">Response</span></span>

<span data-ttu-id="8b8ff-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="8b8ff-131">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8b8ff-132">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8b8ff-132">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8b8ff-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8b8ff-133">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="8b8ff-134">C#</span><span class="sxs-lookup"><span data-stu-id="8b8ff-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b8ff-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="8b8ff-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8b8ff-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="8b8ff-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
