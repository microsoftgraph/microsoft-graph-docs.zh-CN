---
title: 获取用户的 transitiveReports
description: 获取用户的可传递报告数。
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5d04b1240c54b186a2e5f5cfb77f651e032f1eda
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316606"
---
# <a name="get-transitivereports-for-a-user"></a><span data-ttu-id="88ee4-103">获取用户的 transitiveReports</span><span class="sxs-lookup"><span data-stu-id="88ee4-103">Get transitiveReports for a user</span></span>

<span data-ttu-id="88ee4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ee4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88ee4-105">检索用户的可传递报告计数。</span><span class="sxs-lookup"><span data-stu-id="88ee4-105">Retrieve a count of transitive reports for a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="88ee4-106">权限</span><span class="sxs-lookup"><span data-stu-id="88ee4-106">Permissions</span></span>

<span data-ttu-id="88ee4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88ee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="88ee4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88ee4-109">Permission type</span></span> | <span data-ttu-id="88ee4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88ee4-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="88ee4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88ee4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88ee4-112">User.Read、User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="88ee4-112">User.Read, User.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="88ee4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88ee4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88ee4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88ee4-114">Not supported.</span></span> |
| <span data-ttu-id="88ee4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88ee4-115">Application</span></span> | <span data-ttu-id="88ee4-116">User.Read、User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="88ee4-116">User.Read, User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88ee4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88ee4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/transitiveReports/$count
```
## <a name="optional-query-parameters"></a><span data-ttu-id="88ee4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="88ee4-118">Optional query parameters</span></span>

<span data-ttu-id="88ee4-119">此方法仅支持 `$filter` **accountEnabled 属性的查询** 参数。</span><span class="sxs-lookup"><span data-stu-id="88ee4-119">This method supports the `$filter` query parameter for only the **accountEnabled** property.</span></span> <span data-ttu-id="88ee4-120">有关使用查询参数的信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="88ee4-120">For more information about using query parameters, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="88ee4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="88ee4-121">Request headers</span></span>

| <span data-ttu-id="88ee4-122">标头</span><span class="sxs-lookup"><span data-stu-id="88ee4-122">Header</span></span>       | <span data-ttu-id="88ee4-123">值</span><span class="sxs-lookup"><span data-stu-id="88ee4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88ee4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88ee4-124">Authorization</span></span>  | <span data-ttu-id="88ee4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88ee4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="88ee4-127">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="88ee4-127">ConsistencyLevel</span></span> | <span data-ttu-id="88ee4-128">最终。</span><span class="sxs-lookup"><span data-stu-id="88ee4-128">eventual.</span></span> <span data-ttu-id="88ee4-129">必填。</span><span class="sxs-lookup"><span data-stu-id="88ee4-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88ee4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="88ee4-130">Request body</span></span>

<span data-ttu-id="88ee4-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88ee4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88ee4-132">响应</span><span class="sxs-lookup"><span data-stu-id="88ee4-132">Response</span></span>

<span data-ttu-id="88ee4-133">如果成功，此方法在响应正文中返回 响应代码和用户的可 `200 OK` 传递报告计数。</span><span class="sxs-lookup"><span data-stu-id="88ee4-133">If successful, this method returns a `200 OK` response code and a count of transitive reports for the user in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88ee4-134">示例</span><span class="sxs-lookup"><span data-stu-id="88ee4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88ee4-135">请求</span><span class="sxs-lookup"><span data-stu-id="88ee4-135">Request</span></span>

<span data-ttu-id="88ee4-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88ee4-136">The following is an example of the request.</span></span> <span data-ttu-id="88ee4-137">查询 `$count` 段是必需的。</span><span class="sxs-lookup"><span data-stu-id="88ee4-137">The `$count` query segment is required.</span></span>


# <a name="http"></a>[<span data-ttu-id="88ee4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="88ee4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivereports_user"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count
```
# <a name="c"></a>[<span data-ttu-id="88ee4-139">C#</span><span class="sxs-lookup"><span data-stu-id="88ee4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivereports-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88ee4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88ee4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivereports-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88ee4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88ee4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivereports-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88ee4-142">Java</span><span class="sxs-lookup"><span data-stu-id="88ee4-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-transitivereports-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="88ee4-143">响应</span><span class="sxs-lookup"><span data-stu-id="88ee4-143">Response</span></span>

<span data-ttu-id="88ee4-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="88ee4-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="88ee4-145">5 </span><span class="sxs-lookup"><span data-stu-id="88ee4-145">5</span></span>

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
