---
title: 'group: addFavorite'
description: 将组添加到当前用户的收藏夹组列表中。 仅支持 Microsoft 365 组。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1f8c0b327fabd60f52747cc7c78ff398709fe3ff
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786970"
---
# <a name="group-addfavorite"></a><span data-ttu-id="f7b2d-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="f7b2d-104">group: addFavorite</span></span>

<span data-ttu-id="f7b2d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7b2d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b2d-106">将组添加到当前用户的收藏夹组列表中。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-106">Add the group to the list of the current user's favorite groups.</span></span> <span data-ttu-id="f7b2d-107">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b2d-108">权限</span><span class="sxs-lookup"><span data-stu-id="f7b2d-108">Permissions</span></span>
<span data-ttu-id="f7b2d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7b2d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7b2d-111">Permission type</span></span>      | <span data-ttu-id="f7b2d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7b2d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7b2d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b2d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f7b2d-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7b2d-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7b2d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7b2d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b2d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-116">Not supported.</span></span>    |
|<span data-ttu-id="f7b2d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7b2d-117">Application</span></span> | <span data-ttu-id="f7b2d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b2d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7b2d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="f7b2d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7b2d-120">Request headers</span></span>
| <span data-ttu-id="f7b2d-121">标头</span><span class="sxs-lookup"><span data-stu-id="f7b2d-121">Header</span></span>       | <span data-ttu-id="f7b2d-122">值</span><span class="sxs-lookup"><span data-stu-id="f7b2d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7b2d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7b2d-123">Authorization</span></span>  | <span data-ttu-id="f7b2d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7b2d-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="f7b2d-126">Prefer</span></span> | <span data-ttu-id="f7b2d-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-127">return=minimal.</span></span> <span data-ttu-id="f7b2d-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f7b2d-129">可选。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f7b2d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7b2d-130">Request body</span></span>
<span data-ttu-id="f7b2d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7b2d-132">响应</span><span class="sxs-lookup"><span data-stu-id="f7b2d-132">Response</span></span>
<span data-ttu-id="f7b2d-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7b2d-135">示例</span><span class="sxs-lookup"><span data-stu-id="f7b2d-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f7b2d-136">请求</span><span class="sxs-lookup"><span data-stu-id="f7b2d-136">Request</span></span>
<span data-ttu-id="f7b2d-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7b2d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7b2d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```
# <a name="c"></a>[<span data-ttu-id="f7b2d-139">C#</span><span class="sxs-lookup"><span data-stu-id="f7b2d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-addfavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7b2d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7b2d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-addfavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7b2d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7b2d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-addfavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7b2d-142">Java</span><span class="sxs-lookup"><span data-stu-id="f7b2d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-addfavorite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7b2d-143">响应</span><span class="sxs-lookup"><span data-stu-id="f7b2d-143">Response</span></span>
<span data-ttu-id="f7b2d-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7b2d-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
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


