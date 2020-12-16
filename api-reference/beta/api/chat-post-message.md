---
title: 在聊天中发送 chatMessage
description: 在聊天中发送新的 chatMessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7f0e18946903c2926b8c26241b7dbdd7fdbf5851
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689757"
---
# <a name="send-chatmessage-in-a-chat"></a><span data-ttu-id="05d91-103">在聊天中发送 chatMessage</span><span class="sxs-lookup"><span data-stu-id="05d91-103">Send chatMessage in a chat</span></span>

<span data-ttu-id="05d91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05d91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05d91-105">在指定的[聊天中创建新的 chatMessage](../resources/chatmessage.md) [。](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="05d91-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="05d91-106">此 API 无法创建新聊天;在创建聊天 [消息之前](chat-list.md) ，必须使用列表聊天方法检索现有聊天的 ID。</span><span class="sxs-lookup"><span data-stu-id="05d91-106">This API cannot create a new chat; you must use the [list chats](chat-list.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="05d91-107">**注意**：不建议使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="05d91-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="05d91-108">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="05d91-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="05d91-109">**注意**：使用 Microsoft Teams [](/legal/microsoft-apis/terms-of-use)作为 microsoft Teams 日志文件。</span><span class="sxs-lookup"><span data-stu-id="05d91-109">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="05d91-110">仅发送用户将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="05d91-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="05d91-111">权限</span><span class="sxs-lookup"><span data-stu-id="05d91-111">Permissions</span></span>

<span data-ttu-id="05d91-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05d91-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05d91-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="05d91-114">Permission type</span></span>                        | <span data-ttu-id="05d91-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05d91-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05d91-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05d91-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="05d91-117">ChatMessage.Send、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="05d91-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="05d91-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05d91-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05d91-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="05d91-119">Not supported.</span></span> |
| <span data-ttu-id="05d91-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="05d91-120">Application</span></span>                            | <span data-ttu-id="05d91-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="05d91-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="05d91-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05d91-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="05d91-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="05d91-123">Request headers</span></span>

| <span data-ttu-id="05d91-124">名称</span><span class="sxs-lookup"><span data-stu-id="05d91-124">Name</span></span>          | <span data-ttu-id="05d91-125">说明</span><span class="sxs-lookup"><span data-stu-id="05d91-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="05d91-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="05d91-126">Authorization</span></span> | <span data-ttu-id="05d91-127">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="05d91-127">Bearer {code}.</span></span> <span data-ttu-id="05d91-128">必需。</span><span class="sxs-lookup"><span data-stu-id="05d91-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05d91-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="05d91-129">Request body</span></span>

<span data-ttu-id="05d91-130">在请求正文中，提供 [chatMessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05d91-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="05d91-131">响应</span><span class="sxs-lookup"><span data-stu-id="05d91-131">Response</span></span>

<span data-ttu-id="05d91-132">如果成功，此方法在响应正文中返回响应代码和 `201 Created` 新的 [chatMessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05d91-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05d91-133">示例</span><span class="sxs-lookup"><span data-stu-id="05d91-133">Examples</span></span>

<span data-ttu-id="05d91-134">有关示例的更全面的列表，请参阅在频道[或聊天中创建 chatMessage。](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="05d91-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="05d91-135">请求</span><span class="sxs-lookup"><span data-stu-id="05d91-135">Request</span></span>

<span data-ttu-id="05d91-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="05d91-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05d91-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="05d91-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/{id}/messages
Content-type: application/json

{
  "body": {
     "content": "Hello world"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="05d91-138">C#</span><span class="sxs-lookup"><span data-stu-id="05d91-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05d91-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05d91-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05d91-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05d91-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05d91-141">Java</span><span class="sxs-lookup"><span data-stu-id="05d91-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05d91-142">响应</span><span class="sxs-lookup"><span data-stu-id="05d91-142">Response</span></span>

<span data-ttu-id="05d91-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="05d91-143">The following is an example of the response.</span></span>

> <span data-ttu-id="05d91-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="05d91-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
