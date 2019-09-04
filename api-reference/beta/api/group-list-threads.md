---
title: 列出线程
description: 获取某个组的所有线程。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6eaa699ce343043f0f5af2446f8faa1f482581d0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721549"
---
# <a name="list-threads"></a><span data-ttu-id="546ba-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="546ba-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="546ba-104">获取某个组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="546ba-104">Get all the threads of a group.</span></span>

<span data-ttu-id="546ba-105">注意：还可以 [获取会话的所有线程](conversation-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="546ba-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="546ba-106">权限</span><span class="sxs-lookup"><span data-stu-id="546ba-106">Permissions</span></span>
<span data-ttu-id="546ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="546ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546ba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="546ba-109">Permission type</span></span>      | <span data-ttu-id="546ba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="546ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="546ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="546ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="546ba-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546ba-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="546ba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="546ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="546ba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="546ba-114">Not supported.</span></span>    |
|<span data-ttu-id="546ba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="546ba-115">Application</span></span> | <span data-ttu-id="546ba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="546ba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="546ba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="546ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="546ba-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="546ba-118">Optional query parameters</span></span>
<span data-ttu-id="546ba-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="546ba-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="546ba-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="546ba-120">Request headers</span></span>
| <span data-ttu-id="546ba-121">标头</span><span class="sxs-lookup"><span data-stu-id="546ba-121">Header</span></span>       | <span data-ttu-id="546ba-122">值</span><span class="sxs-lookup"><span data-stu-id="546ba-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="546ba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="546ba-123">Authorization</span></span>  | <span data-ttu-id="546ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="546ba-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="546ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="546ba-126">Request body</span></span>
<span data-ttu-id="546ba-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="546ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="546ba-128">响应</span><span class="sxs-lookup"><span data-stu-id="546ba-128">Response</span></span>
<span data-ttu-id="546ba-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="546ba-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="546ba-130">示例</span><span class="sxs-lookup"><span data-stu-id="546ba-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="546ba-131">请求</span><span class="sxs-lookup"><span data-stu-id="546ba-131">Request</span></span>
<span data-ttu-id="546ba-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="546ba-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="546ba-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="546ba-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="546ba-134">C#</span><span class="sxs-lookup"><span data-stu-id="546ba-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="546ba-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="546ba-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="546ba-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="546ba-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="546ba-137">响应</span><span class="sxs-lookup"><span data-stu-id="546ba-137">Response</span></span>
<span data-ttu-id="546ba-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="546ba-138">The following is an example of the response.</span></span>
><span data-ttu-id="546ba-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="546ba-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="546ba-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="546ba-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
    {
      "toRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ],
      "topic": "topic-value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
      "uniqueSenders": [
        "uniqueSenders-value"
      ],
      "ccRecipients": [
        {
          "emailAddress": {
            "name": "name-value",
            "address": "address-value"
          }
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
