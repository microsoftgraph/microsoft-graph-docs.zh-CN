---
title: 获取 plannerPlanDetails
description: 检索 **plannerplandetails** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 3f95a3fe8f867f65f1a4e34b19a9fbc3226bed72
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979034"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="bd87a-103">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="bd87a-103">Get plannerPlanDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd87a-104">检索 **plannerplandetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd87a-104">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd87a-105">权限</span><span class="sxs-lookup"><span data-stu-id="bd87a-105">Permissions</span></span>
<span data-ttu-id="bd87a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd87a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd87a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd87a-108">Permission type</span></span>      | <span data-ttu-id="bd87a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd87a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd87a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd87a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd87a-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd87a-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd87a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd87a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd87a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd87a-113">Not supported.</span></span>    |
|<span data-ttu-id="bd87a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd87a-114">Application</span></span> | <span data-ttu-id="bd87a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd87a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd87a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd87a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="bd87a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd87a-117">Request headers</span></span>
| <span data-ttu-id="bd87a-118">名称</span><span class="sxs-lookup"><span data-stu-id="bd87a-118">Name</span></span>      |<span data-ttu-id="bd87a-119">说明</span><span class="sxs-lookup"><span data-stu-id="bd87a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bd87a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd87a-120">Authorization</span></span>  | <span data-ttu-id="bd87a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd87a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd87a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd87a-123">Request body</span></span>
<span data-ttu-id="bd87a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd87a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd87a-125">响应</span><span class="sxs-lookup"><span data-stu-id="bd87a-125">Response</span></span>

<span data-ttu-id="bd87a-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd87a-126">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="bd87a-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="bd87a-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bd87a-130">示例</span><span class="sxs-lookup"><span data-stu-id="bd87a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd87a-131">请求</span><span class="sxs-lookup"><span data-stu-id="bd87a-131">Request</span></span>
<span data-ttu-id="bd87a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd87a-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bd87a-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bd87a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd87a-134">C#</span><span class="sxs-lookup"><span data-stu-id="bd87a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd87a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="bd87a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd87a-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="bd87a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bd87a-137">Java</span><span class="sxs-lookup"><span data-stu-id="bd87a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bd87a-138">响应</span><span class="sxs-lookup"><span data-stu-id="bd87a-138">Response</span></span>
<span data-ttu-id="bd87a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd87a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
