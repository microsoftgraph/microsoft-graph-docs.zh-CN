---
title: 列出线程
description: 获取某个组的所有线程。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 051728fb5f077c9d82b6bff431e47913e75572d3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263005"
---
# <a name="list-threads"></a><span data-ttu-id="ca9f3-103">列出线程</span><span class="sxs-lookup"><span data-stu-id="ca9f3-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca9f3-104">获取某个组的所有线程。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-104">Get all the threads of a group.</span></span>

<span data-ttu-id="ca9f3-105">注意：还可以 [获取会话的所有线程](conversation-list-threads.md)。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca9f3-106">权限</span><span class="sxs-lookup"><span data-stu-id="ca9f3-106">Permissions</span></span>
<span data-ttu-id="ca9f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca9f3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca9f3-109">Permission type</span></span>      | <span data-ttu-id="ca9f3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca9f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca9f3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca9f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca9f3-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca9f3-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca9f3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca9f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca9f3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-114">Not supported.</span></span>    |
|<span data-ttu-id="ca9f3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca9f3-115">Application</span></span> | <span data-ttu-id="ca9f3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca9f3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca9f3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca9f3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ca9f3-118">Optional query parameters</span></span>
<span data-ttu-id="ca9f3-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca9f3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca9f3-120">Request headers</span></span>
| <span data-ttu-id="ca9f3-121">标头</span><span class="sxs-lookup"><span data-stu-id="ca9f3-121">Header</span></span>       | <span data-ttu-id="ca9f3-122">值</span><span class="sxs-lookup"><span data-stu-id="ca9f3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ca9f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca9f3-123">Authorization</span></span>  | <span data-ttu-id="ca9f3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ca9f3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca9f3-126">Request body</span></span>
<span data-ttu-id="ca9f3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca9f3-128">响应</span><span class="sxs-lookup"><span data-stu-id="ca9f3-128">Response</span></span>
<span data-ttu-id="ca9f3-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [conversationThread](../resources/conversationthread.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca9f3-130">示例</span><span class="sxs-lookup"><span data-stu-id="ca9f3-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ca9f3-131">请求</span><span class="sxs-lookup"><span data-stu-id="ca9f3-131">Request</span></span>
<span data-ttu-id="ca9f3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="ca9f3-133">响应</span><span class="sxs-lookup"><span data-stu-id="ca9f3-133">Response</span></span>
<span data-ttu-id="ca9f3-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-134">The following is an example of the response.</span></span>
><span data-ttu-id="ca9f3-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ca9f3-136">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ca9f3-136">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ca9f3-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ca9f3-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ca9f3-138">C#</span><span class="sxs-lookup"><span data-stu-id="ca9f3-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_threads-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ca9f3-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ca9f3-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_threads-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ca9f3-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="ca9f3-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_threads-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
