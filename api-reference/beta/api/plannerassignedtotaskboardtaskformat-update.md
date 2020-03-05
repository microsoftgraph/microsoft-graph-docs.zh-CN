---
title: 更新 plannerAssignedToTaskBoardTaskFormat
description: 更新 **plannerAssignedToTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 7e862657e737e561ec934a46aeb6cef2d6e07c8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455772"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="97d9a-103">更新 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="97d9a-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="97d9a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="97d9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d9a-105">更新 **plannerAssignedToTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97d9a-105">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="97d9a-106">权限</span><span class="sxs-lookup"><span data-stu-id="97d9a-106">Permissions</span></span>
<span data-ttu-id="97d9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97d9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d9a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97d9a-109">Permission type</span></span>      | <span data-ttu-id="97d9a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97d9a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97d9a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97d9a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97d9a-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d9a-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97d9a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97d9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97d9a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="97d9a-114">Not supported.</span></span>    |
|<span data-ttu-id="97d9a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97d9a-115">Application</span></span> | <span data-ttu-id="97d9a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="97d9a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97d9a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97d9a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="97d9a-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="97d9a-118">Optional request headers</span></span>
| <span data-ttu-id="97d9a-119">名称</span><span class="sxs-lookup"><span data-stu-id="97d9a-119">Name</span></span>       | <span data-ttu-id="97d9a-120">说明</span><span class="sxs-lookup"><span data-stu-id="97d9a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="97d9a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97d9a-121">Authorization</span></span>  | <span data-ttu-id="97d9a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97d9a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97d9a-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="97d9a-124">If-Match</span></span>  | <span data-ttu-id="97d9a-p103">要更新的 **plannerAssignedToTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="97d9a-p103">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97d9a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="97d9a-127">Request body</span></span>
<span data-ttu-id="97d9a-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="97d9a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97d9a-131">属性</span><span class="sxs-lookup"><span data-stu-id="97d9a-131">Property</span></span>     | <span data-ttu-id="97d9a-132">类型</span><span class="sxs-lookup"><span data-stu-id="97d9a-132">Type</span></span>   |<span data-ttu-id="97d9a-133">说明</span><span class="sxs-lookup"><span data-stu-id="97d9a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97d9a-134">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="97d9a-134">orderHintsByAssignee</span></span>|[<span data-ttu-id="97d9a-135">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="97d9a-135">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="97d9a-136">用于对任务板的 "分配" 视图上的任务进行排序的提示的字典。</span><span class="sxs-lookup"><span data-stu-id="97d9a-136">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="97d9a-137">每个条目的键是任务分配到的用户之一，值是 order 提示。</span><span class="sxs-lookup"><span data-stu-id="97d9a-137">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="97d9a-138">每个值的格式在 [使用 Planner 中的排序提示] （.。/resources/planner_order_hint_format）。</span><span class="sxs-lookup"><span data-stu-id="97d9a-138">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="97d9a-139">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="97d9a-139">unassignedOrderHint</span></span>|<span data-ttu-id="97d9a-140">字符串</span><span class="sxs-lookup"><span data-stu-id="97d9a-140">String</span></span>|<span data-ttu-id="97d9a-141">在任务未分配给任何人时，或者如果 orderHintsByAssignee 字典没有为任务分配到的用户提供 order 提示，用于在任务板的 "分配给" 视图中对任务进行排序的提示值。</span><span class="sxs-lookup"><span data-stu-id="97d9a-141">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="97d9a-142">格式是在计划程序[中使用 order 提示](../resources/planner-order-hint-format.md)定义的。</span><span class="sxs-lookup"><span data-stu-id="97d9a-142">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="97d9a-143">响应</span><span class="sxs-lookup"><span data-stu-id="97d9a-143">Response</span></span>

<span data-ttu-id="97d9a-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="97d9a-144">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="97d9a-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="97d9a-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="97d9a-148">示例</span><span class="sxs-lookup"><span data-stu-id="97d9a-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97d9a-149">请求</span><span class="sxs-lookup"><span data-stu-id="97d9a-149">Request</span></span>
<span data-ttu-id="97d9a-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97d9a-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97d9a-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="97d9a-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="97d9a-152">C#</span><span class="sxs-lookup"><span data-stu-id="97d9a-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerassignedtotaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97d9a-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97d9a-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerassignedtotaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97d9a-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97d9a-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerassignedtotaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97d9a-155">响应</span><span class="sxs-lookup"><span data-stu-id="97d9a-155">Response</span></span>
<span data-ttu-id="97d9a-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97d9a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
