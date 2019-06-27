---
title: 列出聊天
description: 检索用户的聊天列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 180cfad72a8a8df60a58be5cedfab07fad40a5b7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261416"
---
# <a name="list-chats"></a><span data-ttu-id="4f6d5-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="4f6d5-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f6d5-104">检索用户所属的[聊天](../resources/chat.md)列表。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-104">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f6d5-105">权限</span><span class="sxs-lookup"><span data-stu-id="4f6d5-105">Permissions</span></span>

<span data-ttu-id="4f6d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f6d5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f6d5-108">Permission type</span></span>      | <span data-ttu-id="4f6d5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f6d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f6d5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f6d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4f6d5-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="4f6d5-111">Chat.Read</span></span>   |
|<span data-ttu-id="4f6d5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f6d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f6d5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-113">Not supported.</span></span>    |
|<span data-ttu-id="4f6d5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f6d5-114">Application</span></span> | <span data-ttu-id="4f6d5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="4f6d5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f6d5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f6d5-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4f6d5-117">Optional query parameters</span></span>

<span data-ttu-id="4f6d5-118">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f6d5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f6d5-119">Request headers</span></span>

| <span data-ttu-id="4f6d5-120">标头</span><span class="sxs-lookup"><span data-stu-id="4f6d5-120">Header</span></span>       | <span data-ttu-id="4f6d5-121">值</span><span class="sxs-lookup"><span data-stu-id="4f6d5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f6d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f6d5-122">Authorization</span></span>  | <span data-ttu-id="4f6d5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f6d5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f6d5-125">Request body</span></span>

<span data-ttu-id="4f6d5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f6d5-127">响应</span><span class="sxs-lookup"><span data-stu-id="4f6d5-127">Response</span></span>

<span data-ttu-id="4f6d5-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f6d5-129">示例</span><span class="sxs-lookup"><span data-stu-id="4f6d5-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4f6d5-130">请求</span><span class="sxs-lookup"><span data-stu-id="4f6d5-130">Request</span></span>

<span data-ttu-id="4f6d5-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```

##### <a name="response"></a><span data-ttu-id="4f6d5-132">响应</span><span class="sxs-lookup"><span data-stu-id="4f6d5-132">Response</span></span>

<span data-ttu-id="4f6d5-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-133">Here is an example of the response.</span></span> 

><span data-ttu-id="4f6d5-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f6d5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4f6d5-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4f6d5-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4f6d5-137">C#</span><span class="sxs-lookup"><span data-stu-id="4f6d5-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chats-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f6d5-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f6d5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chats-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4f6d5-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="4f6d5-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chats-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/chat-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chat-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chat-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
