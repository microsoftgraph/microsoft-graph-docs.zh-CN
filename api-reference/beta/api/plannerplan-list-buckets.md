---
title: 列出存储桶
description: 检索 plannerPlan 对象包含的 **plannerbucket** 对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b2722ea6f6c30c185579fe3afa42e54d1444a68d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876419"
---
# <a name="list-buckets"></a><span data-ttu-id="958e8-103">列出存储桶</span><span class="sxs-lookup"><span data-stu-id="958e8-103">List buckets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="958e8-104">检索[plannerPlan](../resources/plannerplan.md)对象包含的[plannerBucket](../resources/plannerbucket.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="958e8-104">Retrieve a list of [plannerBucket](../resources/plannerbucket.md) objects contained by a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="958e8-105">权限</span><span class="sxs-lookup"><span data-stu-id="958e8-105">Permissions</span></span>
<span data-ttu-id="958e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="958e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="958e8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="958e8-108">Permission type</span></span>      | <span data-ttu-id="958e8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="958e8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="958e8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="958e8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="958e8-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="958e8-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="958e8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="958e8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="958e8-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="958e8-113">Not supported.</span></span>    |
|<span data-ttu-id="958e8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="958e8-114">Application</span></span> | <span data-ttu-id="958e8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="958e8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="958e8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="958e8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/buckets
```

## <a name="request-headers"></a><span data-ttu-id="958e8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="958e8-117">Request headers</span></span>
| <span data-ttu-id="958e8-118">名称</span><span class="sxs-lookup"><span data-stu-id="958e8-118">Name</span></span>      |<span data-ttu-id="958e8-119">说明</span><span class="sxs-lookup"><span data-stu-id="958e8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="958e8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="958e8-120">Authorization</span></span>  | <span data-ttu-id="958e8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="958e8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="958e8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="958e8-123">Request body</span></span>
<span data-ttu-id="958e8-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="958e8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="958e8-125">响应</span><span class="sxs-lookup"><span data-stu-id="958e8-125">Response</span></span>

<span data-ttu-id="958e8-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[plannerBucket](../resources/plannerbucket.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="958e8-126">If successful, this method returns a `200 OK` response code and a collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="958e8-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="958e8-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="958e8-130">示例</span><span class="sxs-lookup"><span data-stu-id="958e8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="958e8-131">请求</span><span class="sxs-lookup"><span data-stu-id="958e8-131">Request</span></span>
<span data-ttu-id="958e8-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="958e8-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="958e8-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="958e8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/2txjA-BMZEq-bKi6Wfj5aGQAB1OJ/buckets
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="958e8-134">C#</span><span class="sxs-lookup"><span data-stu-id="958e8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-buckets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="958e8-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="958e8-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-buckets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="958e8-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="958e8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-buckets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="958e8-137">Java</span><span class="sxs-lookup"><span data-stu-id="958e8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-buckets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="958e8-138">响应</span><span class="sxs-lookup"><span data-stu-id="958e8-138">Response</span></span>
<span data-ttu-id="958e8-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="958e8-139">Here is an example of the response.</span></span> 

><span data-ttu-id="958e8-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="958e8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
