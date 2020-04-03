---
title: 'group: addFavorite'
description: 将组添加到当前用户的收藏夹组列表中。仅支持 Office 365 组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4d78fc0890226a753778e3dd9f5782465135cae1
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123935"
---
# <a name="group-addfavorite"></a><span data-ttu-id="5b004-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="5b004-104">group: addFavorite</span></span>

<span data-ttu-id="5b004-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b004-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b004-p102">将组添加到当前用户的收藏夹组列表中。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="5b004-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b004-108">权限</span><span class="sxs-lookup"><span data-stu-id="5b004-108">Permissions</span></span>
<span data-ttu-id="5b004-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b004-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b004-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b004-111">Permission type</span></span>      | <span data-ttu-id="5b004-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b004-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b004-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b004-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b004-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b004-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5b004-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b004-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b004-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b004-116">Not supported.</span></span>    |
|<span data-ttu-id="5b004-117">Application</span><span class="sxs-lookup"><span data-stu-id="5b004-117">Application</span></span> | <span data-ttu-id="5b004-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b004-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b004-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b004-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="5b004-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b004-120">Request headers</span></span>
| <span data-ttu-id="5b004-121">标头</span><span class="sxs-lookup"><span data-stu-id="5b004-121">Header</span></span>       | <span data-ttu-id="5b004-122">值</span><span class="sxs-lookup"><span data-stu-id="5b004-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b004-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b004-123">Authorization</span></span>  | <span data-ttu-id="5b004-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b004-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b004-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="5b004-126">Prefer</span></span> | <span data-ttu-id="5b004-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="5b004-127">return=minimal.</span></span> <span data-ttu-id="5b004-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="5b004-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="5b004-129">可选。</span><span class="sxs-lookup"><span data-stu-id="5b004-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="5b004-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b004-130">Request body</span></span>
<span data-ttu-id="5b004-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b004-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b004-132">响应</span><span class="sxs-lookup"><span data-stu-id="5b004-132">Response</span></span>
<span data-ttu-id="5b004-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5b004-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b004-135">示例</span><span class="sxs-lookup"><span data-stu-id="5b004-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5b004-136">请求</span><span class="sxs-lookup"><span data-stu-id="5b004-136">Request</span></span>
<span data-ttu-id="5b004-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b004-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b004-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b004-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```
# <a name="c"></a>[<span data-ttu-id="5b004-139">C#</span><span class="sxs-lookup"><span data-stu-id="5b004-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-addfavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b004-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b004-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-addfavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b004-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b004-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-addfavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5b004-142">响应</span><span class="sxs-lookup"><span data-stu-id="5b004-142">Response</span></span>
<span data-ttu-id="5b004-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b004-143">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

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
  ]
}
-->
