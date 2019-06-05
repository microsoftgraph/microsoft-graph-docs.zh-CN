---
title: 创建了 chatmessage
description: 使用此 API 创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 22ee0d1e4b2822f26a4892fb354bdc8c90663d21
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720879"
---
# <a name="create-chatmessage"></a><span data-ttu-id="8e57e-103">创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="8e57e-103">Create chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e57e-104">在指定的[聊天](../resources/chat.md)中创建新[邮件](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="8e57e-104">Create a new [message](../resources/chatmessage.md) in the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e57e-105">权限</span><span class="sxs-lookup"><span data-stu-id="8e57e-105">Permissions</span></span>

<span data-ttu-id="8e57e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8e57e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e57e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e57e-108">Permission type</span></span>                        | <span data-ttu-id="8e57e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8e57e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e57e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e57e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e57e-111">聊天读</span><span class="sxs-lookup"><span data-stu-id="8e57e-111">Chat.ReadWrite</span></span> |
| <span data-ttu-id="8e57e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e57e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e57e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e57e-113">Not supported.</span></span> |
| <span data-ttu-id="8e57e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e57e-114">Application</span></span>                            | <span data-ttu-id="8e57e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e57e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e57e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e57e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="8e57e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e57e-117">Request headers</span></span>

| <span data-ttu-id="8e57e-118">名称</span><span class="sxs-lookup"><span data-stu-id="8e57e-118">Name</span></span>          | <span data-ttu-id="8e57e-119">说明</span><span class="sxs-lookup"><span data-stu-id="8e57e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e57e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e57e-120">Authorization</span></span> | <span data-ttu-id="8e57e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8e57e-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e57e-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e57e-122">Request body</span></span>

<span data-ttu-id="8e57e-123">在请求正文中, 提供[了 chatmessage](../resources/chatmessage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e57e-123">In the request body, supply a JSON representation of [chatMessage](../resources/chatmessage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8e57e-124">响应</span><span class="sxs-lookup"><span data-stu-id="8e57e-124">Response</span></span>

<span data-ttu-id="8e57e-125">如果成功, 此方法在响应`201 Created`正文中返回响应代码和新的[了 chatmessage](../resources/chatmessage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8e57e-125">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8e57e-126">示例</span><span class="sxs-lookup"><span data-stu-id="8e57e-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8e57e-127">请求</span><span class="sxs-lookup"><span data-stu-id="8e57e-127">Request</span></span>

<span data-ttu-id="8e57e-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8e57e-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e57e-129">响应</span><span class="sxs-lookup"><span data-stu-id="8e57e-129">Response</span></span>

<span data-ttu-id="8e57e-130">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8e57e-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="8e57e-131">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8e57e-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e57e-132">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8e57e-132">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->