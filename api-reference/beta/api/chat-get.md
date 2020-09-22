---
title: 获取聊天
description: 检索一个聊天。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ecfc4a6e1f000755bda95a4014ccf5efa1c8fc7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982715"
---
# <a name="get-chat"></a><span data-ttu-id="23f15-103">获取聊天</span><span class="sxs-lookup"><span data-stu-id="23f15-103">Get chat</span></span>

<span data-ttu-id="23f15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f15-105">检索一个[聊天](../resources/chat.md)（不含其消息）。</span><span class="sxs-lookup"><span data-stu-id="23f15-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="23f15-106">权限</span><span class="sxs-lookup"><span data-stu-id="23f15-106">Permissions</span></span>

<span data-ttu-id="23f15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="23f15-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="23f15-109">Permission type</span></span>      | <span data-ttu-id="23f15-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23f15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f15-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23f15-111">Delegated (work or school account)</span></span> | <span data-ttu-id="23f15-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23f15-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="23f15-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23f15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f15-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="23f15-114">Not supported.</span></span>    |
|<span data-ttu-id="23f15-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="23f15-115">Application</span></span> | <span data-ttu-id="23f15-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="23f15-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="23f15-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23f15-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23f15-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23f15-118">Optional query parameters</span></span>

<span data-ttu-id="23f15-119">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23f15-119">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23f15-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="23f15-120">Request headers</span></span>

| <span data-ttu-id="23f15-121">标头</span><span class="sxs-lookup"><span data-stu-id="23f15-121">Header</span></span>       | <span data-ttu-id="23f15-122">值</span><span class="sxs-lookup"><span data-stu-id="23f15-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23f15-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23f15-123">Authorization</span></span>  | <span data-ttu-id="23f15-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23f15-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23f15-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="23f15-126">Request body</span></span>

<span data-ttu-id="23f15-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23f15-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23f15-128">响应</span><span class="sxs-lookup"><span data-stu-id="23f15-128">Response</span></span>

<span data-ttu-id="23f15-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="23f15-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23f15-130">示例</span><span class="sxs-lookup"><span data-stu-id="23f15-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23f15-131">请求</span><span class="sxs-lookup"><span data-stu-id="23f15-131">Request</span></span>
<span data-ttu-id="23f15-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23f15-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23f15-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="23f15-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```
# <a name="c"></a>[<span data-ttu-id="23f15-134">C#</span><span class="sxs-lookup"><span data-stu-id="23f15-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23f15-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23f15-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23f15-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23f15-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23f15-137">响应</span><span class="sxs-lookup"><span data-stu-id="23f15-137">Response</span></span>
<span data-ttu-id="23f15-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="23f15-138">Here is an example of the response.</span></span> 

><span data-ttu-id="23f15-139">**注意：** 为提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="23f15-139">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="23f15-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="23f15-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
    "topic": null,
    "createdDateTime": "2019-04-18T23:51:42.099Z",
    "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


