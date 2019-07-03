---
title: 列出聊天
description: 检索用户的聊天列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a220806659ec72632a8f8e4c485cb7f4c818244f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437822"
---
# <a name="list-chats"></a><span data-ttu-id="f4336-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="f4336-103">List chats</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4336-104">检索用户所属的[聊天](../resources/chat.md)列表。</span><span class="sxs-lookup"><span data-stu-id="f4336-104">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4336-105">权限</span><span class="sxs-lookup"><span data-stu-id="f4336-105">Permissions</span></span>

<span data-ttu-id="f4336-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4336-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4336-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4336-108">Permission type</span></span>      | <span data-ttu-id="f4336-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4336-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4336-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4336-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f4336-111">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="f4336-111">Chat.Read</span></span>   |
|<span data-ttu-id="f4336-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4336-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4336-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4336-113">Not supported.</span></span>    |
|<span data-ttu-id="f4336-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4336-114">Application</span></span> | <span data-ttu-id="f4336-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4336-115">Not supported.</span></span>   |

## <a name="http-request"></a><span data-ttu-id="f4336-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4336-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4336-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4336-117">Optional query parameters</span></span>

<span data-ttu-id="f4336-118">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4336-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4336-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4336-119">Request headers</span></span>

| <span data-ttu-id="f4336-120">标头</span><span class="sxs-lookup"><span data-stu-id="f4336-120">Header</span></span>       | <span data-ttu-id="f4336-121">值</span><span class="sxs-lookup"><span data-stu-id="f4336-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f4336-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4336-122">Authorization</span></span>  | <span data-ttu-id="f4336-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4336-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f4336-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4336-125">Request body</span></span>

<span data-ttu-id="f4336-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4336-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4336-127">响应</span><span class="sxs-lookup"><span data-stu-id="f4336-127">Response</span></span>

<span data-ttu-id="f4336-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4336-128">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4336-129">示例</span><span class="sxs-lookup"><span data-stu-id="f4336-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f4336-130">请求</span><span class="sxs-lookup"><span data-stu-id="f4336-130">Request</span></span>

<span data-ttu-id="f4336-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4336-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f4336-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f4336-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f4336-133">C#</span><span class="sxs-lookup"><span data-stu-id="f4336-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4336-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4336-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f4336-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="f4336-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f4336-136">响应</span><span class="sxs-lookup"><span data-stu-id="f4336-136">Response</span></span>

<span data-ttu-id="f4336-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4336-137">Here is an example of the response.</span></span> 

><span data-ttu-id="f4336-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f4336-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
