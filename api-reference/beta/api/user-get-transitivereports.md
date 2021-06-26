---
title: 获取用户的 transitiveReports
description: 获取用户的可传递报告数。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a1ec6b231592ffec0d8847282b50e4ad227ecf06
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151777"
---
# <a name="get-transitivereports-for-a-user"></a><span data-ttu-id="73a07-103">获取用户的 transitiveReports</span><span class="sxs-lookup"><span data-stu-id="73a07-103">Get transitiveReports for a user</span></span>

<span data-ttu-id="73a07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73a07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73a07-105">检索用户的可传递报告计数。</span><span class="sxs-lookup"><span data-stu-id="73a07-105">Retrieve a count of transitive reports for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="73a07-106">权限</span><span class="sxs-lookup"><span data-stu-id="73a07-106">Permissions</span></span>

<span data-ttu-id="73a07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="73a07-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73a07-109">Permission type</span></span> | <span data-ttu-id="73a07-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73a07-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="73a07-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73a07-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73a07-112">User.Read、User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="73a07-112">User.Read, User.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="73a07-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73a07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73a07-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73a07-114">Not supported.</span></span> |
| <span data-ttu-id="73a07-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73a07-115">Application</span></span> | <span data-ttu-id="73a07-116">User.Read、User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="73a07-116">User.Read, User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73a07-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73a07-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/transitiveReports/$count
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73a07-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73a07-118">Optional query parameters</span></span>

<span data-ttu-id="73a07-119">此方法仅支持 `$filter` **accountEnabled 属性的查询** 参数。</span><span class="sxs-lookup"><span data-stu-id="73a07-119">This method supports the `$filter` query parameter for only the **accountEnabled** property.</span></span> <span data-ttu-id="73a07-120">有关使用查询参数的信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="73a07-120">For more information about using query parameters, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="73a07-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="73a07-121">Request headers</span></span>

| <span data-ttu-id="73a07-122">标头</span><span class="sxs-lookup"><span data-stu-id="73a07-122">Header</span></span>       | <span data-ttu-id="73a07-123">值</span><span class="sxs-lookup"><span data-stu-id="73a07-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73a07-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="73a07-124">Authorization</span></span>  | <span data-ttu-id="73a07-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73a07-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73a07-127">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="73a07-127">ConsistencyLevel</span></span> | <span data-ttu-id="73a07-128">最终。</span><span class="sxs-lookup"><span data-stu-id="73a07-128">eventual.</span></span> <span data-ttu-id="73a07-129">必填。</span><span class="sxs-lookup"><span data-stu-id="73a07-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73a07-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="73a07-130">Request body</span></span>

<span data-ttu-id="73a07-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73a07-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73a07-132">响应</span><span class="sxs-lookup"><span data-stu-id="73a07-132">Response</span></span>

<span data-ttu-id="73a07-133">如果成功，此方法在响应正文中返回 响应代码和用户的可 `200 OK` 传递报告计数。</span><span class="sxs-lookup"><span data-stu-id="73a07-133">If successful, this method returns a `200 OK` response code and a count of transitive reports for the user in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73a07-134">示例</span><span class="sxs-lookup"><span data-stu-id="73a07-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73a07-135">请求</span><span class="sxs-lookup"><span data-stu-id="73a07-135">Request</span></span>

<span data-ttu-id="73a07-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73a07-136">The following is an example of the request.</span></span> <span data-ttu-id="73a07-137">查询 `$count` 段是必需的。</span><span class="sxs-lookup"><span data-stu-id="73a07-137">The `$count` query segment is required.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_transitivereports_user"
}-->
```http
GET https://graph.microsoft.com/beta/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```

### <a name="response"></a><span data-ttu-id="73a07-138">响应</span><span class="sxs-lookup"><span data-stu-id="73a07-138">Response</span></span>

<span data-ttu-id="73a07-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73a07-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="73a07-140">5 </span><span class="sxs-lookup"><span data-stu-id="73a07-140">5</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get transitiveReports for a user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
