---
title: 列出聊天
description: 检索用户的聊天列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bc8f92eec06167d79db5e9849d5984dae1bc0278
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863093"
---
# <a name="list-chats"></a><span data-ttu-id="d3487-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="d3487-103">List chats</span></span>

<span data-ttu-id="d3487-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3487-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3487-105">检索用户所属的[聊天](../resources/chat.md)列表。</span><span class="sxs-lookup"><span data-stu-id="d3487-105">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3487-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3487-106">Permissions</span></span>

<span data-ttu-id="d3487-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d3487-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d3487-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3487-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3487-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3487-109">Permission type</span></span>      | <span data-ttu-id="d3487-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3487-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3487-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3487-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3487-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3487-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="d3487-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3487-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3487-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3487-114">Not supported.</span></span>    |
|<span data-ttu-id="d3487-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3487-115">Application</span></span> | <span data-ttu-id="d3487-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3487-116">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="d3487-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3487-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3487-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3487-118">Optional query parameters</span></span>

<span data-ttu-id="d3487-119">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3487-119">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3487-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3487-120">Request headers</span></span>

| <span data-ttu-id="d3487-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3487-121">Header</span></span>       | <span data-ttu-id="d3487-122">值</span><span class="sxs-lookup"><span data-stu-id="d3487-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3487-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3487-123">Authorization</span></span>  | <span data-ttu-id="d3487-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d3487-124">Bearer {token}.</span></span> <span data-ttu-id="d3487-125">Required.</span><span class="sxs-lookup"><span data-stu-id="d3487-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3487-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3487-126">Request body</span></span>

<span data-ttu-id="d3487-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3487-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3487-128">响应</span><span class="sxs-lookup"><span data-stu-id="d3487-128">Response</span></span>

<span data-ttu-id="d3487-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d3487-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3487-130">示例</span><span class="sxs-lookup"><span data-stu-id="d3487-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d3487-131">请求</span><span class="sxs-lookup"><span data-stu-id="d3487-131">Request</span></span>

<span data-ttu-id="d3487-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3487-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3487-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3487-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="d3487-134">C#</span><span class="sxs-lookup"><span data-stu-id="d3487-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3487-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3487-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3487-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3487-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3487-137">响应</span><span class="sxs-lookup"><span data-stu-id="d3487-137">Response</span></span>

<span data-ttu-id="d3487-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d3487-138">Here is an example of the response.</span></span> 

><span data-ttu-id="d3487-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="d3487-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d3487-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d3487-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats",
    "value": [
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_877192bd-9183-47d3-a74c-8aa0426716cf@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:51:42.099Z",
            "lastUpdatedDateTime": "2019-04-18T23:51:43.255Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_0c5cfdbb-596f-4d39-b557-5d9516c94107@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-04-18T23:19:23.76Z",
            "lastUpdatedDateTime": "2019-04-18T23:19:21.994Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_3ee373aa-62fa-4fc6-b11f-9627d5b4a73d@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-03-21T22:30:14.867Z",
            "lastUpdatedDateTime": "2019-03-21T22:30:15.507Z"
        },
        {
            "id": "19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_90a27c51-5c74-453b-944a-134ba86da790@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2019-02-06T03:38:58.062Z",
            "lastUpdatedDateTime": "2019-02-06T03:38:58.063Z"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
