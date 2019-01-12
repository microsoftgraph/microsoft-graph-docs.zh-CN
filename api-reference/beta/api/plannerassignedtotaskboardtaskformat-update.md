---
title: 更新 plannerAssignedToTaskBoardTaskFormat
description: 更新 **plannerAssignedToTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b388d3d19287c4a5c039763ce812c22b87515622
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915702"
---
# <a name="update-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="4ebb2-103">更新 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="4ebb2-103">Update plannerAssignedToTaskBoardTaskFormat</span></span>

> <span data-ttu-id="4ebb2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ebb2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ebb2-106">更新 **plannerAssignedToTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-106">Update the properties of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ebb2-107">权限</span><span class="sxs-lookup"><span data-stu-id="4ebb2-107">Permissions</span></span>
<span data-ttu-id="4ebb2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ebb2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ebb2-110">Permission type</span></span>      | <span data-ttu-id="4ebb2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ebb2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ebb2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebb2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4ebb2-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ebb2-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ebb2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebb2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ebb2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-115">Not supported.</span></span>    |
|<span data-ttu-id="4ebb2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ebb2-116">Application</span></span> | <span data-ttu-id="4ebb2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ebb2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ebb2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="4ebb2-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4ebb2-119">Optional request headers</span></span>
| <span data-ttu-id="4ebb2-120">名称</span><span class="sxs-lookup"><span data-stu-id="4ebb2-120">Name</span></span>       | <span data-ttu-id="4ebb2-121">说明</span><span class="sxs-lookup"><span data-stu-id="4ebb2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4ebb2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ebb2-122">Authorization</span></span>  | <span data-ttu-id="4ebb2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ebb2-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="4ebb2-125">If-Match</span></span>  | <span data-ttu-id="4ebb2-p104">要更新的 **plannerAssignedToTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-p104">Last known ETag value for **plannerAssignedToTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ebb2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ebb2-128">Request body</span></span>
<span data-ttu-id="4ebb2-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4ebb2-132">属性</span><span class="sxs-lookup"><span data-stu-id="4ebb2-132">Property</span></span>     | <span data-ttu-id="4ebb2-133">类型</span><span class="sxs-lookup"><span data-stu-id="4ebb2-133">Type</span></span>   |<span data-ttu-id="4ebb2-134">说明</span><span class="sxs-lookup"><span data-stu-id="4ebb2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ebb2-135">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="4ebb2-135">orderHintsByAssignee</span></span>|[<span data-ttu-id="4ebb2-136">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="4ebb2-136">plannerOrderHintsByAssignee</span></span>](../resources/plannerorderhintsbyassignee.md)|<span data-ttu-id="4ebb2-137">使用任务板的 AssignedTo 视图上的顺序任务提示的字典。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-137">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board.</span></span> <span data-ttu-id="4ebb2-138">每个条目的键是一个任务分配给用户，值为 order 提示。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-138">The key of each entry is one of the users the task is assigned to and the value is the order hint.</span></span> <span data-ttu-id="4ebb2-139">中定义的每个值的格式 [计划程序中使用订单提示 (.../ resources/planner_order_hint_format.md)。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-139">The format of each value is defined in [Using order hints in Planner(../resources/planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="4ebb2-140">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="4ebb2-140">unassignedOrderHint</span></span>|<span data-ttu-id="4ebb2-141">字符串</span><span class="sxs-lookup"><span data-stu-id="4ebb2-141">String</span></span>|<span data-ttu-id="4ebb2-142">提示值已使用任务的任务板 AssignedTo 视图时任务未分配给任何人，或 orderHintsByAssignee 词典不提供 order 提示用户任务分配给。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-142">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to.</span></span> <span data-ttu-id="4ebb2-143">[使用规划器中的顺序提示](../resources/planner-order-hint-format.md)中定义格式。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-143">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="4ebb2-144">响应</span><span class="sxs-lookup"><span data-stu-id="4ebb2-144">Response</span></span>

<span data-ttu-id="4ebb2-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-145">If successful, this method returns a `200 OK` response code and updated [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="4ebb2-p108">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-p108">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4ebb2-149">示例</span><span class="sxs-lookup"><span data-stu-id="4ebb2-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ebb2-150">请求</span><span class="sxs-lookup"><span data-stu-id="4ebb2-150">Request</span></span>
<span data-ttu-id="4ebb2-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-151">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4ebb2-152">响应</span><span class="sxs-lookup"><span data-stu-id="4ebb2-152">Response</span></span>
<span data-ttu-id="4ebb2-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ebb2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
