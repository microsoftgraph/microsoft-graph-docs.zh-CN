---
title: 创建了 chatmessage
description: 使用此 API 创建新的了 chatmessage。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 66e73ac2c3523c7c374c78143a91fc7a5e846778
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438566"
---
# <a name="create-chatmessage"></a><span data-ttu-id="51e1e-103">创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="51e1e-103">Create chatMessage</span></span>

<span data-ttu-id="51e1e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="51e1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51e1e-105">在指定的[聊天](../resources/chat.md)中创建新[邮件](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="51e1e-105">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="51e1e-106">此 API 无法创建新聊天，在创建聊天消息之前，必须使用 "[列表聊天](chat-list.md)" 方法检索现有聊天的 Id。</span><span class="sxs-lookup"><span data-stu-id="51e1e-106">This API cannot create an new chat, you must use the [list chats](chat-list.md) method to retreive the Id of an existing chat before creating a chat message.</span></span>

## <a name="permissions"></a><span data-ttu-id="51e1e-107">权限</span><span class="sxs-lookup"><span data-stu-id="51e1e-107">Permissions</span></span>

<span data-ttu-id="51e1e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51e1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51e1e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51e1e-110">Permission type</span></span>                        | <span data-ttu-id="51e1e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51e1e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51e1e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51e1e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="51e1e-113">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e1e-113">Chat.ReadWrite</span></span> |
| <span data-ttu-id="51e1e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51e1e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51e1e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51e1e-115">Not supported.</span></span> |
| <span data-ttu-id="51e1e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="51e1e-116">Application</span></span>                            | <span data-ttu-id="51e1e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="51e1e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51e1e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51e1e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="51e1e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51e1e-119">Request headers</span></span>

| <span data-ttu-id="51e1e-120">名称</span><span class="sxs-lookup"><span data-stu-id="51e1e-120">Name</span></span>          | <span data-ttu-id="51e1e-121">说明</span><span class="sxs-lookup"><span data-stu-id="51e1e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="51e1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e1e-122">Authorization</span></span> | <span data-ttu-id="51e1e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="51e1e-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="51e1e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="51e1e-124">Request body</span></span>

<span data-ttu-id="51e1e-125">在请求正文中，提供[了 chatmessage](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51e1e-125">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="51e1e-126">响应</span><span class="sxs-lookup"><span data-stu-id="51e1e-126">Response</span></span>

<span data-ttu-id="51e1e-127">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="51e1e-127">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51e1e-128">示例</span><span class="sxs-lookup"><span data-stu-id="51e1e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51e1e-129">请求</span><span class="sxs-lookup"><span data-stu-id="51e1e-129">Request</span></span>

<span data-ttu-id="51e1e-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="51e1e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51e1e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="51e1e-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="51e1e-132">C#</span><span class="sxs-lookup"><span data-stu-id="51e1e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51e1e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51e1e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51e1e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51e1e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="51e1e-135">响应</span><span class="sxs-lookup"><span data-stu-id="51e1e-135">Response</span></span>

<span data-ttu-id="51e1e-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="51e1e-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="51e1e-137">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51e1e-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="51e1e-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="51e1e-138">All the properties will be returned from an actual call.</span></span>

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
