---
title: 列出 rejectedSender
description: '获取此组的“遭拒的发件人”列表中的用户或组列表。 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a9d2ac3fe041e58ddba7d35d08f2f15856b2bd0d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263061"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="ce140-103">列出 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="ce140-103">List rejectedSenders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce140-104">获取此组的“遭拒的发件人”列表中的用户或组列表。</span><span class="sxs-lookup"><span data-stu-id="ce140-104">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="ce140-p101">已拒绝的发件人列表中的用户无法发布到组对话（在 GET 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="ce140-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce140-107">权限</span><span class="sxs-lookup"><span data-stu-id="ce140-107">Permissions</span></span>
<span data-ttu-id="ce140-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce140-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce140-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce140-110">Permission type</span></span>      | <span data-ttu-id="ce140-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce140-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce140-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce140-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce140-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce140-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce140-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce140-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce140-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce140-115">Not supported.</span></span>    |
|<span data-ttu-id="ce140-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce140-116">Application</span></span> | <span data-ttu-id="ce140-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce140-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce140-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce140-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce140-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ce140-119">Optional query parameters</span></span>
<span data-ttu-id="ce140-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ce140-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce140-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce140-121">Request headers</span></span>
| <span data-ttu-id="ce140-122">标头</span><span class="sxs-lookup"><span data-stu-id="ce140-122">Header</span></span>       | <span data-ttu-id="ce140-123">值</span><span class="sxs-lookup"><span data-stu-id="ce140-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ce140-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce140-124">Authorization</span></span>  | <span data-ttu-id="ce140-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce140-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce140-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce140-127">Request body</span></span>
<span data-ttu-id="ce140-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce140-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce140-129">响应</span><span class="sxs-lookup"><span data-stu-id="ce140-129">Response</span></span>
<span data-ttu-id="ce140-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ce140-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce140-131">示例</span><span class="sxs-lookup"><span data-stu-id="ce140-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ce140-132">请求</span><span class="sxs-lookup"><span data-stu-id="ce140-132">Request</span></span>
<span data-ttu-id="ce140-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ce140-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/rejectedSenders
```

#### <a name="response"></a><span data-ttu-id="ce140-134">响应</span><span class="sxs-lookup"><span data-stu-id="ce140-134">Response</span></span>
<span data-ttu-id="ce140-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ce140-135">The following is an example of the response.</span></span>
><span data-ttu-id="ce140-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ce140-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ce140-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ce140-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ce140-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ce140-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ce140-139">C#</span><span class="sxs-lookup"><span data-stu-id="ce140-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ce140-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="ce140-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ce140-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="ce140-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_rejectedsenders-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
