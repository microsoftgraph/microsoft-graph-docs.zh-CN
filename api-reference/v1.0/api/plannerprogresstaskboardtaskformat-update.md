---
title: 更新 plannerProgressTaskBoardTaskFormat
description: 更新 **plannerProgressTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 75ec25b895219eed1f18a504462dbb0b9b12f6c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42510849"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="dd128-103">更新 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dd128-103">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="dd128-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd128-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd128-105">更新 **plannerProgressTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dd128-105">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dd128-106">权限</span><span class="sxs-lookup"><span data-stu-id="dd128-106">Permissions</span></span>
<span data-ttu-id="dd128-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd128-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd128-109">Permission type</span></span>      | <span data-ttu-id="dd128-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd128-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd128-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd128-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd128-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd128-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dd128-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd128-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd128-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd128-114">Not supported.</span></span>    |
|<span data-ttu-id="dd128-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd128-115">Application</span></span> | <span data-ttu-id="dd128-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd128-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd128-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd128-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="dd128-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="dd128-118">Optional request headers</span></span>
| <span data-ttu-id="dd128-119">名称</span><span class="sxs-lookup"><span data-stu-id="dd128-119">Name</span></span>       | <span data-ttu-id="dd128-120">说明</span><span class="sxs-lookup"><span data-stu-id="dd128-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dd128-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd128-121">Authorization</span></span>  | <span data-ttu-id="dd128-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd128-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd128-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="dd128-124">If-Match</span></span>  | <span data-ttu-id="dd128-p103">要更新的 **plannerProgressTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="dd128-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd128-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd128-127">Request body</span></span>
<span data-ttu-id="dd128-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="dd128-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dd128-131">属性</span><span class="sxs-lookup"><span data-stu-id="dd128-131">Property</span></span>     | <span data-ttu-id="dd128-132">类型</span><span class="sxs-lookup"><span data-stu-id="dd128-132">Type</span></span>   |<span data-ttu-id="dd128-133">说明</span><span class="sxs-lookup"><span data-stu-id="dd128-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd128-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="dd128-134">orderHint</span></span>|<span data-ttu-id="dd128-135">String</span><span class="sxs-lookup"><span data-stu-id="dd128-135">String</span></span>|<span data-ttu-id="dd128-p105">用于为任务板“进度”视图上的任务进行排序的提示值。[此处](../resources/planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="dd128-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="dd128-138">响应</span><span class="sxs-lookup"><span data-stu-id="dd128-138">Response</span></span>

<span data-ttu-id="dd128-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd128-139">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="dd128-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="dd128-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="dd128-143">示例</span><span class="sxs-lookup"><span data-stu-id="dd128-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd128-144">请求</span><span class="sxs-lookup"><span data-stu-id="dd128-144">Request</span></span>
<span data-ttu-id="dd128-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd128-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd128-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd128-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="dd128-147">C#</span><span class="sxs-lookup"><span data-stu-id="dd128-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd128-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd128-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd128-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd128-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd128-150">Java</span><span class="sxs-lookup"><span data-stu-id="dd128-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerprogresstaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd128-151">响应</span><span class="sxs-lookup"><span data-stu-id="dd128-151">Response</span></span>
<span data-ttu-id="dd128-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd128-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
