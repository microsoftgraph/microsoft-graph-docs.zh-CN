---
title: 更新 plannerAssignedToTaskBoardTaskFormat
description: 更新 **plannerAssignedToTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: af09748385da95fa26bc34ecdd49b313a3334614
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444013"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="dcbb6-103">更新 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dcbb6-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="dcbb6-104">更新 **plannerAssignedToTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-104">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dcbb6-105">权限</span><span class="sxs-lookup"><span data-stu-id="dcbb6-105">Permissions</span></span>
<span data-ttu-id="dcbb6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcbb6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcbb6-108">Permission type</span></span>      | <span data-ttu-id="dcbb6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcbb6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcbb6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcbb6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcbb6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcbb6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dcbb6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcbb6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcbb6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-113">Not supported.</span></span>    |
|<span data-ttu-id="dcbb6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcbb6-114">Application</span></span> | <span data-ttu-id="dcbb6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcbb6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcbb6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="dcbb6-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="dcbb6-117">Optional request headers</span></span>
| <span data-ttu-id="dcbb6-118">名称</span><span class="sxs-lookup"><span data-stu-id="dcbb6-118">Name</span></span>       | <span data-ttu-id="dcbb6-119">说明</span><span class="sxs-lookup"><span data-stu-id="dcbb6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dcbb6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcbb6-120">Authorization</span></span>  | <span data-ttu-id="dcbb6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dcbb6-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="dcbb6-123">If-Match</span></span>  | <span data-ttu-id="dcbb6-p103">要更新的 **plannerAssignedToTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcbb6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcbb6-126">Request body</span></span>
<span data-ttu-id="dcbb6-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dcbb6-130">属性</span><span class="sxs-lookup"><span data-stu-id="dcbb6-130">Property</span></span>     | <span data-ttu-id="dcbb6-131">类型</span><span class="sxs-lookup"><span data-stu-id="dcbb6-131">Type</span></span>   |<span data-ttu-id="dcbb6-132">说明</span><span class="sxs-lookup"><span data-stu-id="dcbb6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcbb6-133">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="dcbb6-133">orderHintsByAssignee</span></span>|[<span data-ttu-id="dcbb6-134">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="dcbb6-134">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="dcbb6-p105">用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](../resources/planner-order-hint-format.md)概述了各值的格式。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="dcbb6-138">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="dcbb6-138">unassignedOrderHint</span></span>|<span data-ttu-id="dcbb6-139">字符串</span><span class="sxs-lookup"><span data-stu-id="dcbb6-139">String</span></span>|<span data-ttu-id="dcbb6-p106">当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，用于为任务板 AssignedTo 视图上的任务进行排序的提示值。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="dcbb6-142">响应</span><span class="sxs-lookup"><span data-stu-id="dcbb6-142">Response</span></span>

<span data-ttu-id="dcbb6-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-143">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="dcbb6-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="dcbb6-147">示例</span><span class="sxs-lookup"><span data-stu-id="dcbb6-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcbb6-148">请求</span><span class="sxs-lookup"><span data-stu-id="dcbb6-148">Request</span></span>
<span data-ttu-id="dcbb6-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dcbb6-150">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dcbb6-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcbb6-151">C#</span><span class="sxs-lookup"><span data-stu-id="dcbb6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcbb6-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="dcbb6-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcbb6-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="dcbb6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dcbb6-154">响应</span><span class="sxs-lookup"><span data-stu-id="dcbb6-154">Response</span></span>
<span data-ttu-id="dcbb6-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dcbb6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
