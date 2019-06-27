---
title: 'group: addFavorite'
description: 将组添加到当前用户的收藏夹组列表中。仅支持 Office 365 组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 4c9560cb633d6472aba9634cebf6c1c07025a155
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263417"
---
# <a name="group-addfavorite"></a><span data-ttu-id="7ffab-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="7ffab-104">group: addFavorite</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ffab-p102">将组添加到当前用户的收藏夹组列表中。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="7ffab-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ffab-107">权限</span><span class="sxs-lookup"><span data-stu-id="7ffab-107">Permissions</span></span>
<span data-ttu-id="7ffab-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ffab-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ffab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ffab-110">Permission type</span></span>      | <span data-ttu-id="7ffab-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ffab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ffab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ffab-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7ffab-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ffab-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ffab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ffab-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ffab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ffab-115">Not supported.</span></span>    |
|<span data-ttu-id="7ffab-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ffab-116">Application</span></span> | <span data-ttu-id="7ffab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ffab-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ffab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ffab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="7ffab-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ffab-119">Request headers</span></span>
| <span data-ttu-id="7ffab-120">标头</span><span class="sxs-lookup"><span data-stu-id="7ffab-120">Header</span></span>       | <span data-ttu-id="7ffab-121">值</span><span class="sxs-lookup"><span data-stu-id="7ffab-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ffab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ffab-122">Authorization</span></span>  | <span data-ttu-id="7ffab-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ffab-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7ffab-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="7ffab-125">Prefer</span></span> | <span data-ttu-id="7ffab-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="7ffab-126">return=minimal.</span></span> <span data-ttu-id="7ffab-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="7ffab-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="7ffab-128">可选。</span><span class="sxs-lookup"><span data-stu-id="7ffab-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="7ffab-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ffab-129">Request body</span></span>
<span data-ttu-id="7ffab-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ffab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ffab-131">响应</span><span class="sxs-lookup"><span data-stu-id="7ffab-131">Response</span></span>
<span data-ttu-id="7ffab-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7ffab-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ffab-134">示例</span><span class="sxs-lookup"><span data-stu-id="7ffab-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7ffab-135">请求</span><span class="sxs-lookup"><span data-stu-id="7ffab-135">Request</span></span>
<span data-ttu-id="7ffab-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7ffab-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="7ffab-137">响应</span><span class="sxs-lookup"><span data-stu-id="7ffab-137">Response</span></span>
<span data-ttu-id="7ffab-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7ffab-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7ffab-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7ffab-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7ffab-140">C#</span><span class="sxs-lookup"><span data-stu-id="7ffab-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_addfavorite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ffab-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="7ffab-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_addfavorite-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7ffab-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="7ffab-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_addfavorite-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-addfavorite.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-addfavorite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-addfavorite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
