---
title: 列出聊天
description: 检索用户的聊天列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ec54f01cc6ad4e025fac0d7297d94dba9a65317
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982671"
---
# <a name="list-chats"></a><span data-ttu-id="007ef-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="007ef-103">List chats</span></span>

<span data-ttu-id="007ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="007ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="007ef-105">检索用户所属的 [聊天](../resources/chat.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="007ef-105">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="007ef-106">权限</span><span class="sxs-lookup"><span data-stu-id="007ef-106">Permissions</span></span>

<span data-ttu-id="007ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="007ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="007ef-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="007ef-109">Permission type</span></span>      | <span data-ttu-id="007ef-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="007ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="007ef-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="007ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="007ef-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="007ef-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="007ef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="007ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="007ef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="007ef-114">Not supported.</span></span>    |
|<span data-ttu-id="007ef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="007ef-115">Application</span></span> | <span data-ttu-id="007ef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="007ef-116">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="007ef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="007ef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="007ef-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="007ef-118">Optional query parameters</span></span>

<span data-ttu-id="007ef-119">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="007ef-119">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="007ef-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="007ef-120">Request headers</span></span>

| <span data-ttu-id="007ef-121">标头</span><span class="sxs-lookup"><span data-stu-id="007ef-121">Header</span></span>       | <span data-ttu-id="007ef-122">值</span><span class="sxs-lookup"><span data-stu-id="007ef-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="007ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="007ef-123">Authorization</span></span>  | <span data-ttu-id="007ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="007ef-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="007ef-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="007ef-126">Request body</span></span>

<span data-ttu-id="007ef-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="007ef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="007ef-128">响应</span><span class="sxs-lookup"><span data-stu-id="007ef-128">Response</span></span>

<span data-ttu-id="007ef-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="007ef-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="007ef-130">示例</span><span class="sxs-lookup"><span data-stu-id="007ef-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="007ef-131">请求</span><span class="sxs-lookup"><span data-stu-id="007ef-131">Request</span></span>

<span data-ttu-id="007ef-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="007ef-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="007ef-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="007ef-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="007ef-134">C#</span><span class="sxs-lookup"><span data-stu-id="007ef-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="007ef-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="007ef-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="007ef-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="007ef-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="007ef-137">响应</span><span class="sxs-lookup"><span data-stu-id="007ef-137">Response</span></span>

<span data-ttu-id="007ef-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="007ef-138">Here is an example of the response.</span></span> 

><span data-ttu-id="007ef-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="007ef-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


