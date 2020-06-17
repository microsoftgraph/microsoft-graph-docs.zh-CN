---
title: 获取聊天
description: 检索一个聊天。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d444bb967aea89206c4c0a47d82cdcb6218c5e89
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287708"
---
# <a name="get-chat"></a><span data-ttu-id="0557f-103">获取聊天</span><span class="sxs-lookup"><span data-stu-id="0557f-103">Get chat</span></span>

<span data-ttu-id="0557f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0557f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0557f-105">检索一个[聊天](../resources/chat.md)（不含其消息）。</span><span class="sxs-lookup"><span data-stu-id="0557f-105">Retrieve a single [chat](../resources/chat.md) (without its messages).</span></span>

## <a name="permissions"></a><span data-ttu-id="0557f-106">权限</span><span class="sxs-lookup"><span data-stu-id="0557f-106">Permissions</span></span>

<span data-ttu-id="0557f-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0557f-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0557f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0557f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0557f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0557f-109">Permission type</span></span>      | <span data-ttu-id="0557f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0557f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0557f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0557f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0557f-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0557f-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="0557f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0557f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0557f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0557f-114">Not supported.</span></span>    |
|<span data-ttu-id="0557f-115">Application</span><span class="sxs-lookup"><span data-stu-id="0557f-115">Application</span></span> | <span data-ttu-id="0557f-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0557f-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="0557f-117">借助应用程序权限，支持获取一次聊天，但不支持[获取聊天列表](chat-list.md)。</span><span class="sxs-lookup"><span data-stu-id="0557f-117">With application permissions, getting a single chat is supported, but [getting a list of chats](chat-list.md) is not.</span></span>

> [!NOTE]
> <span data-ttu-id="0557f-118">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="0557f-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="0557f-119">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="0557f-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="0557f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0557f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats/{id}
GET /users/{id}/chats/{id}
GET /chats/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0557f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0557f-121">Optional query parameters</span></span>

<span data-ttu-id="0557f-122">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0557f-122">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0557f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0557f-123">Request headers</span></span>

| <span data-ttu-id="0557f-124">标头</span><span class="sxs-lookup"><span data-stu-id="0557f-124">Header</span></span>       | <span data-ttu-id="0557f-125">值</span><span class="sxs-lookup"><span data-stu-id="0557f-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0557f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0557f-126">Authorization</span></span>  | <span data-ttu-id="0557f-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0557f-127">Bearer {token}.</span></span> <span data-ttu-id="0557f-128">Required.</span><span class="sxs-lookup"><span data-stu-id="0557f-128">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0557f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0557f-129">Request body</span></span>

<span data-ttu-id="0557f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0557f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0557f-131">响应</span><span class="sxs-lookup"><span data-stu-id="0557f-131">Response</span></span>

<span data-ttu-id="0557f-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0557f-132">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0557f-133">示例</span><span class="sxs-lookup"><span data-stu-id="0557f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0557f-134">请求</span><span class="sxs-lookup"><span data-stu-id="0557f-134">Request</span></span>
<span data-ttu-id="0557f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0557f-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0557f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0557f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats/{id}
```
# <a name="c"></a>[<span data-ttu-id="0557f-137">C#</span><span class="sxs-lookup"><span data-stu-id="0557f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0557f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0557f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0557f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0557f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0557f-140">响应</span><span class="sxs-lookup"><span data-stu-id="0557f-140">Response</span></span>
<span data-ttu-id="0557f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0557f-141">Here is an example of the response.</span></span> 

><span data-ttu-id="0557f-142">**注意：** 为提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0557f-142">**Note:** The response object shown here is shortened for readability.</span></span> <span data-ttu-id="0557f-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0557f-143">All the properties will be returned from an actual call.</span></span>
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
