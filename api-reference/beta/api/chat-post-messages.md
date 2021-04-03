---
title: 在聊天中发送消息
description: 在聊天中发送新消息。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f84bc4bcbcdadd050e6e300aabc89578b5e96e2
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51583023"
---
# <a name="send-message-in-a-chat"></a><span data-ttu-id="a2587-103">在聊天中发送消息</span><span class="sxs-lookup"><span data-stu-id="a2587-103">Send message in a chat</span></span>

<span data-ttu-id="a2587-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2587-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2587-105">在指定的聊天 中发送新的[chatMessage](../resources/chatmessage.md) [。](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="a2587-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="a2587-106">此 API 无法创建新聊天;在创建聊天消息之前，必须使用 [列表聊天](chat-list.md) 方法检索现有聊天的 ID。</span><span class="sxs-lookup"><span data-stu-id="a2587-106">This API cannot create a new chat; you must use the [list chats](chat-list.md) method to retrieve the ID of an existing chat before creating a chat message.</span></span>

> <span data-ttu-id="a2587-107">**注意**：不建议使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="a2587-107">**Note**: We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="a2587-108">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="a2587-108">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="a2587-109">**注意**：使用 Microsoft Teams [](/legal/microsoft-apis/terms-of-use)作为 microsoft Teams 日志文件。</span><span class="sxs-lookup"><span data-stu-id="a2587-109">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="a2587-110">仅发送用户将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="a2587-110">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2587-111">权限</span><span class="sxs-lookup"><span data-stu-id="a2587-111">Permissions</span></span>

<span data-ttu-id="a2587-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2587-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2587-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2587-114">Permission type</span></span>                        | <span data-ttu-id="a2587-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2587-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a2587-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2587-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2587-117">ChatMessage.Send、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2587-117">ChatMessage.Send, Chat.ReadWrite</span></span> |
| <span data-ttu-id="a2587-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2587-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2587-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2587-119">Not supported.</span></span> |
| <span data-ttu-id="a2587-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2587-120">Application</span></span>                            | <span data-ttu-id="a2587-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2587-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2587-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2587-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="a2587-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2587-123">Request headers</span></span>

| <span data-ttu-id="a2587-124">名称</span><span class="sxs-lookup"><span data-stu-id="a2587-124">Name</span></span>          | <span data-ttu-id="a2587-125">说明</span><span class="sxs-lookup"><span data-stu-id="a2587-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a2587-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2587-126">Authorization</span></span> | <span data-ttu-id="a2587-127">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="a2587-127">Bearer {code}.</span></span> <span data-ttu-id="a2587-128">必需。</span><span class="sxs-lookup"><span data-stu-id="a2587-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2587-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2587-129">Request body</span></span>

<span data-ttu-id="a2587-130">在请求正文中，提供 [chatMessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2587-130">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a2587-131">响应</span><span class="sxs-lookup"><span data-stu-id="a2587-131">Response</span></span>

<span data-ttu-id="a2587-132">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [chatMessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2587-132">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2587-133">示例</span><span class="sxs-lookup"><span data-stu-id="a2587-133">Examples</span></span>

<span data-ttu-id="a2587-134">有关示例的更全面的列表，请参阅在频道或[聊天中创建 chatMessage。](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="a2587-134">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="a2587-135">请求</span><span class="sxs-lookup"><span data-stu-id="a2587-135">Request</span></span>

<span data-ttu-id="a2587-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2587-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_chatmessages_1"
}-->
```http
POST https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages
Content-type: application/json

{
  "body": {
     "content": "Hello world"
  }
}
```

### <a name="response"></a><span data-ttu-id="a2587-137">响应</span><span class="sxs-lookup"><span data-stu-id="a2587-137">Response</span></span>

<span data-ttu-id="a2587-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2587-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A2da4c29f6d7041eca70b638b43d45437%40thread.v2')/messages/$entity",
    "id": "1616991463150",
    "replyToId": null,
    "etag": "1616991463150",
    "messageType": "message",
    "createdDateTime": "2021-03-29T04:17:43.15Z",
    "lastModifiedDateTime": "2021-03-29T04:17:43.15Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
    "importance": "normal",
    "locale": "en-us",
    "webUrl": null,
    "channelIdentity": null,
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Robin Kline",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "text",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
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
