---
title: 列出任务
description: 检索与 plannerPlan 对象关联的**plannerTask**对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: c50d658756b677d426ce70b68d8b10ebd63b5ac8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413267"
---
# <a name="list-tasks"></a><span data-ttu-id="2785d-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="2785d-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2785d-104">检索与[plannerPlan](../resources/plannerplan.md)对象关联的[plannerTask](../resources/plannertask.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2785d-104">Retrieve a list of [plannerTask](../resources/plannertask.md) objects associated with a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2785d-105">权限</span><span class="sxs-lookup"><span data-stu-id="2785d-105">Permissions</span></span>
<span data-ttu-id="2785d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2785d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2785d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2785d-108">Permission type</span></span>      | <span data-ttu-id="2785d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2785d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2785d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2785d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2785d-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2785d-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2785d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2785d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2785d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2785d-113">Not supported.</span></span>    |
|<span data-ttu-id="2785d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2785d-114">Application</span></span> | <span data-ttu-id="2785d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2785d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2785d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2785d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="2785d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2785d-117">Request headers</span></span>
| <span data-ttu-id="2785d-118">名称</span><span class="sxs-lookup"><span data-stu-id="2785d-118">Name</span></span>      |<span data-ttu-id="2785d-119">说明</span><span class="sxs-lookup"><span data-stu-id="2785d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2785d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2785d-120">Authorization</span></span>  | <span data-ttu-id="2785d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2785d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2785d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2785d-123">Request body</span></span>
<span data-ttu-id="2785d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2785d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2785d-125">响应</span><span class="sxs-lookup"><span data-stu-id="2785d-125">Response</span></span>

<span data-ttu-id="2785d-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[plannerTask](../resources/plannertask.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="2785d-126">If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="2785d-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="2785d-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="2785d-130">示例</span><span class="sxs-lookup"><span data-stu-id="2785d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2785d-131">请求</span><span class="sxs-lookup"><span data-stu-id="2785d-131">Request</span></span>
<span data-ttu-id="2785d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2785d-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2785d-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2785d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2785d-134">C#</span><span class="sxs-lookup"><span data-stu-id="2785d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2785d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2785d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2785d-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="2785d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2785d-137">响应</span><span class="sxs-lookup"><span data-stu-id="2785d-137">Response</span></span>
<span data-ttu-id="2785d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2785d-138">Here is an example of the response.</span></span> 

><span data-ttu-id="2785d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2785d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerAssignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
