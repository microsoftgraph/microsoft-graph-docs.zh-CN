---
title: 列出任务
description: 检索与 plannerPlan 对象关联的 **plannerTask** 对象的列表。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 3aaa96e3e5755dc366b514a32c8b85f445488973
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473862"
---
# <a name="list-tasks"></a><span data-ttu-id="6e7d3-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="6e7d3-103">List tasks</span></span>

<span data-ttu-id="6e7d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e7d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6e7d3-105">检索与[plannerPlan](../resources/plannerplan.md)对象关联的[plannerTask](../resources/plannertask.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-105">Retrieve a list of [plannerTask](../resources/plannertask.md) objects associated with a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e7d3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e7d3-106">Permissions</span></span>
<span data-ttu-id="6e7d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e7d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e7d3-109">Permission type</span></span>      | <span data-ttu-id="6e7d3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e7d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e7d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e7d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6e7d3-112">Tasks.Read、Tasks.ReadWrite、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e7d3-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6e7d3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e7d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e7d3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-114">Not supported.</span></span>    |
|<span data-ttu-id="6e7d3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e7d3-115">Application</span></span> | <span data-ttu-id="6e7d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e7d3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e7d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{plan-id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="6e7d3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e7d3-118">Request headers</span></span>
| <span data-ttu-id="6e7d3-119">名称</span><span class="sxs-lookup"><span data-stu-id="6e7d3-119">Name</span></span>      |<span data-ttu-id="6e7d3-120">说明</span><span class="sxs-lookup"><span data-stu-id="6e7d3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e7d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e7d3-121">Authorization</span></span>  | <span data-ttu-id="6e7d3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e7d3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e7d3-124">Request body</span></span>
<span data-ttu-id="6e7d3-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e7d3-126">响应</span><span class="sxs-lookup"><span data-stu-id="6e7d3-126">Response</span></span>

<span data-ttu-id="6e7d3-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [plannerTask](../resources/plannertask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-127">If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="6e7d3-p103">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6e7d3-131">示例</span><span class="sxs-lookup"><span data-stu-id="6e7d3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e7d3-132">请求</span><span class="sxs-lookup"><span data-stu-id="6e7d3-132">Request</span></span>
<span data-ttu-id="6e7d3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e7d3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e7d3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "plannerplan_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/tasks
```
# <a name="c"></a>[<span data-ttu-id="6e7d3-135">C#</span><span class="sxs-lookup"><span data-stu-id="6e7d3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/plannerplan-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e7d3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e7d3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/plannerplan-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e7d3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e7d3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/plannerplan-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e7d3-138">Java</span><span class="sxs-lookup"><span data-stu-id="6e7d3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/plannerplan-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6e7d3-139">响应</span><span class="sxs-lookup"><span data-stu-id="6e7d3-139">Response</span></span>
<span data-ttu-id="6e7d3-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-140">Here is an example of the response.</span></span> 

><span data-ttu-id="6e7d3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e7d3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

