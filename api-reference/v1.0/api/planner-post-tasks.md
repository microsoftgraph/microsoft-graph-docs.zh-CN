---
title: 创建 plannerTask
description: 使用此 API 新建 **plannerTask**。
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: a7800ee4331b3a81a16accd2d01f132a53bc511d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681683"
---
# <a name="create-plannertask"></a><span data-ttu-id="bd852-103">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="bd852-103">Create plannerTask</span></span>

<span data-ttu-id="bd852-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd852-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd852-105">使用此 API 新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="bd852-105">Use this API to create a new **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd852-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd852-106">Permissions</span></span>
<span data-ttu-id="bd852-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bd852-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bd852-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd852-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd852-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd852-109">Permission type</span></span>      | <span data-ttu-id="bd852-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd852-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd852-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd852-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bd852-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd852-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd852-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd852-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd852-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd852-114">Not supported.</span></span>    |
|<span data-ttu-id="bd852-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd852-115">Application</span></span> | <span data-ttu-id="bd852-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd852-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd852-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd852-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/tasks
```
## <a name="request-headers"></a><span data-ttu-id="bd852-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd852-118">Request headers</span></span>
| <span data-ttu-id="bd852-119">名称</span><span class="sxs-lookup"><span data-stu-id="bd852-119">Name</span></span>       | <span data-ttu-id="bd852-120">说明</span><span class="sxs-lookup"><span data-stu-id="bd852-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bd852-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd852-121">Authorization</span></span>  | <span data-ttu-id="bd852-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="bd852-122">Bearer {token}.</span></span> <span data-ttu-id="bd852-123">Required.</span><span class="sxs-lookup"><span data-stu-id="bd852-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd852-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd852-124">Request body</span></span>
<span data-ttu-id="bd852-125">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span><span class="sxs-lookup"><span data-stu-id="bd852-125">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
<span data-ttu-id="bd852-126">The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span><span class="sxs-lookup"><span data-stu-id="bd852-126">The **plannerTask** planId property must be set to an existing [plannerPlan](../resources/plannerplan.md) object's id.</span></span>

## <a name="response"></a><span data-ttu-id="bd852-127">响应</span><span class="sxs-lookup"><span data-stu-id="bd852-127">Response</span></span>

<span data-ttu-id="bd852-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerTask](../resources/plannertask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd852-128">If successful, this method returns `201 Created` response code and [plannerTask](../resources/plannertask.md) object in the response body.</span></span>

<span data-ttu-id="bd852-129">This method can return any of the [HTTP status codes](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="bd852-129">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="bd852-130">The most common errors that apps should handle for this method are the 400, 403 and 404 responses.</span><span class="sxs-lookup"><span data-stu-id="bd852-130">The most common errors that apps should handle for this method are the 400, 403 and 404 responses.</span></span> <span data-ttu-id="bd852-131">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="bd852-131">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="bd852-132">示例</span><span class="sxs-lookup"><span data-stu-id="bd852-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd852-133">请求</span><span class="sxs-lookup"><span data-stu-id="bd852-133">Request</span></span>
<span data-ttu-id="bd852-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd852-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd852-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd852-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/tasks
Content-type: application/json
Content-length: 285

{
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "orderHint": " !"
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="bd852-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd852-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannertask-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="bd852-137">C#</span><span class="sxs-lookup"><span data-stu-id="bd852-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannertask-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bd852-138">在请求正文中，提供 [plannerTask](../resources/plannertask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd852-138">In the request body, supply a JSON representation of [plannerTask](../resources/plannertask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bd852-139">响应</span><span class="sxs-lookup"><span data-stu-id="bd852-139">Response</span></span>
<span data-ttu-id="bd852-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="bd852-140">Here is an example of the response.</span></span> <span data-ttu-id="bd852-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="bd852-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bd852-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bd852-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 677

{
  "createdBy": {
    "user": {
      "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
    }
  },
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "bucketId": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "title": "Update client list",
  "orderHint": "85752723360752+",
  "createdDateTime": "2015-03-25T18:36:49.2407981Z",
  "assignments": {
    "fbab97d0-4932-4511-b675-204639209557": {
      "@odata.type": "#microsoft.graph.plannerAssignment",
      "assignedBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "assignedDateTime": "2015-03-25T18:36:49.2407981Z",
      "orderHint": "RWk1"
    }
  },
  "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
