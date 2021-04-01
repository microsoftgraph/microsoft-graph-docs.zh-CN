---
title: 获取 plannerPlanDetails
description: 检索 **plannerplandetails** 对象的属性和关系。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 3754cb9680052ede387b5835508ea619a2c2ad4b
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473624"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="b5a96-103">获取 plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b5a96-103">Get plannerPlanDetails</span></span>

<span data-ttu-id="b5a96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5a96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5a96-105">检索 **plannerplandetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5a96-105">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5a96-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5a96-106">Permissions</span></span>
<span data-ttu-id="b5a96-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5a96-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5a96-109">Permission type</span></span>      | <span data-ttu-id="b5a96-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5a96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5a96-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5a96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5a96-112">Tasks.Read、Tasks.ReadWrite、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5a96-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b5a96-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5a96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5a96-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5a96-114">Not supported.</span></span>    |
|<span data-ttu-id="b5a96-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5a96-115">Application</span></span> | <span data-ttu-id="b5a96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5a96-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5a96-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5a96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="b5a96-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5a96-118">Request headers</span></span>
| <span data-ttu-id="b5a96-119">名称</span><span class="sxs-lookup"><span data-stu-id="b5a96-119">Name</span></span>      |<span data-ttu-id="b5a96-120">说明</span><span class="sxs-lookup"><span data-stu-id="b5a96-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5a96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5a96-121">Authorization</span></span>  | <span data-ttu-id="b5a96-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5a96-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5a96-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5a96-124">Request body</span></span>
<span data-ttu-id="b5a96-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5a96-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5a96-126">响应</span><span class="sxs-lookup"><span data-stu-id="b5a96-126">Response</span></span>

<span data-ttu-id="b5a96-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlanDetails](../resources/plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5a96-127">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="b5a96-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="b5a96-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b5a96-131">示例</span><span class="sxs-lookup"><span data-stu-id="b5a96-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5a96-132">请求</span><span class="sxs-lookup"><span data-stu-id="b5a96-132">Request</span></span>
<span data-ttu-id="b5a96-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5a96-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5a96-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5a96-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
# <a name="c"></a>[<span data-ttu-id="b5a96-135">C#</span><span class="sxs-lookup"><span data-stu-id="b5a96-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannerplandetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5a96-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5a96-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannerplandetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5a96-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5a96-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannerplandetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5a96-138">Java</span><span class="sxs-lookup"><span data-stu-id="b5a96-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannerplandetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5a96-139">响应</span><span class="sxs-lookup"><span data-stu-id="b5a96-139">Response</span></span>
<span data-ttu-id="b5a96-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5a96-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


