---
title: 'group: removeFavorite'
description: 从当前用户收藏夹组列表中删除组。 仅支持 Microsoft 365 组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fe33a3ada951a87ea82f6f4875ab11843e9971b8
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895802"
---
# <a name="group-removefavorite"></a><span data-ttu-id="68843-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="68843-104">group: removeFavorite</span></span>

<span data-ttu-id="68843-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68843-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68843-106">从当前用户收藏夹组列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="68843-106">Remove the group from the list of the current user's favorite groups.</span></span> <span data-ttu-id="68843-107">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="68843-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="68843-108">权限</span><span class="sxs-lookup"><span data-stu-id="68843-108">Permissions</span></span>
<span data-ttu-id="68843-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="68843-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="68843-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68843-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68843-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="68843-111">Permission type</span></span>      | <span data-ttu-id="68843-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68843-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68843-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68843-113">Delegated (work or school account)</span></span> | <span data-ttu-id="68843-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68843-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="68843-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68843-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68843-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="68843-116">Not supported.</span></span>    |
|<span data-ttu-id="68843-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="68843-117">Application</span></span> | <span data-ttu-id="68843-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="68843-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68843-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68843-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="68843-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="68843-120">Request headers</span></span>
| <span data-ttu-id="68843-121">标头</span><span class="sxs-lookup"><span data-stu-id="68843-121">Header</span></span>       | <span data-ttu-id="68843-122">值</span><span class="sxs-lookup"><span data-stu-id="68843-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68843-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68843-123">Authorization</span></span>  | <span data-ttu-id="68843-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="68843-124">Bearer {token}.</span></span> <span data-ttu-id="68843-125">Required.</span><span class="sxs-lookup"><span data-stu-id="68843-125">Required.</span></span>  |
| <span data-ttu-id="68843-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="68843-126">Prefer</span></span> | <span data-ttu-id="68843-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="68843-127">return=minimal.</span></span> <span data-ttu-id="68843-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="68843-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="68843-129">可选。</span><span class="sxs-lookup"><span data-stu-id="68843-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="68843-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="68843-130">Request body</span></span>
<span data-ttu-id="68843-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68843-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68843-132">响应</span><span class="sxs-lookup"><span data-stu-id="68843-132">Response</span></span>
<span data-ttu-id="68843-133">If successful, this method returns `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="68843-133">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="68843-134">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="68843-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68843-135">示例</span><span class="sxs-lookup"><span data-stu-id="68843-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="68843-136">请求</span><span class="sxs-lookup"><span data-stu-id="68843-136">Request</span></span>
<span data-ttu-id="68843-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="68843-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="68843-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="68843-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```
# <a name="c"></a>[<span data-ttu-id="68843-139">C#</span><span class="sxs-lookup"><span data-stu-id="68843-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-removefavorite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68843-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68843-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-removefavorite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68843-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68843-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-removefavorite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="68843-142">响应</span><span class="sxs-lookup"><span data-stu-id="68843-142">Response</span></span>
<span data-ttu-id="68843-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="68843-143">The following is an example of the response.</span></span>
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
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
