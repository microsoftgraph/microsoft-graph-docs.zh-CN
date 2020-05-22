---
title: 列出聊天
description: 检索用户的聊天列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5c4c061c7f78fcb907f81481ea86c6a31b0692c1
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345679"
---
# <a name="list-chats"></a><span data-ttu-id="c0c18-103">列出聊天</span><span class="sxs-lookup"><span data-stu-id="c0c18-103">List chats</span></span>

<span data-ttu-id="c0c18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0c18-105">检索用户所属的[聊天](../resources/chat.md)列表。</span><span class="sxs-lookup"><span data-stu-id="c0c18-105">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0c18-106">权限</span><span class="sxs-lookup"><span data-stu-id="c0c18-106">Permissions</span></span>

<span data-ttu-id="c0c18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0c18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0c18-109">Permission type</span></span>      | <span data-ttu-id="c0c18-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0c18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0c18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c18-112">User.readbasic.all、聊天、聊天和读写</span><span class="sxs-lookup"><span data-stu-id="c0c18-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="c0c18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0c18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0c18-114">Not supported.</span></span>    |
|<span data-ttu-id="c0c18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0c18-115">Application</span></span> | <span data-ttu-id="c0c18-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0c18-116">Not supported.</span></span>    |

> [!NOTE]
> <span data-ttu-id="c0c18-117">在调用具有应用程序权限的此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="c0c18-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c0c18-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="c0c18-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c0c18-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0c18-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0c18-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0c18-120">Optional query parameters</span></span>

<span data-ttu-id="c0c18-121">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c0c18-121">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0c18-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0c18-122">Request headers</span></span>

| <span data-ttu-id="c0c18-123">标头</span><span class="sxs-lookup"><span data-stu-id="c0c18-123">Header</span></span>       | <span data-ttu-id="c0c18-124">值</span><span class="sxs-lookup"><span data-stu-id="c0c18-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0c18-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0c18-125">Authorization</span></span>  | <span data-ttu-id="c0c18-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0c18-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0c18-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0c18-128">Request body</span></span>

<span data-ttu-id="c0c18-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0c18-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c18-130">响应</span><span class="sxs-lookup"><span data-stu-id="c0c18-130">Response</span></span>

<span data-ttu-id="c0c18-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chat](../resources/chat.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0c18-131">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c18-132">示例</span><span class="sxs-lookup"><span data-stu-id="c0c18-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c0c18-133">请求</span><span class="sxs-lookup"><span data-stu-id="c0c18-133">Request</span></span>

<span data-ttu-id="c0c18-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0c18-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0c18-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c18-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chats"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/chats
```
# <a name="c"></a>[<span data-ttu-id="c0c18-136">C#</span><span class="sxs-lookup"><span data-stu-id="c0c18-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0c18-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0c18-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0c18-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0c18-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c0c18-139">响应</span><span class="sxs-lookup"><span data-stu-id="c0c18-139">Response</span></span>

<span data-ttu-id="c0c18-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c0c18-140">Here is an example of the response.</span></span> 

><span data-ttu-id="c0c18-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c0c18-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
