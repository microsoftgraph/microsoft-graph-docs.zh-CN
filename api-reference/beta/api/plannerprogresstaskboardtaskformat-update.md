---
title: 更新 plannerProgressTaskBoardTaskFormat
description: 更新 **plannerProgressTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1148fe1f6d04af8206b7ba51c1e5b262e07c256d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594779"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="942d2-103">更新 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="942d2-103">Update plannerProgressTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942d2-104">更新 **plannerProgressTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="942d2-104">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="942d2-105">权限</span><span class="sxs-lookup"><span data-stu-id="942d2-105">Permissions</span></span>
<span data-ttu-id="942d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="942d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942d2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="942d2-108">Permission type</span></span>      | <span data-ttu-id="942d2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="942d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="942d2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="942d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="942d2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942d2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="942d2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="942d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="942d2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="942d2-113">Not supported.</span></span>    |
|<span data-ttu-id="942d2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="942d2-114">Application</span></span> | <span data-ttu-id="942d2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="942d2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="942d2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="942d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="942d2-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="942d2-117">Optional request headers</span></span>
| <span data-ttu-id="942d2-118">名称</span><span class="sxs-lookup"><span data-stu-id="942d2-118">Name</span></span>       | <span data-ttu-id="942d2-119">说明</span><span class="sxs-lookup"><span data-stu-id="942d2-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="942d2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="942d2-120">Authorization</span></span>  | <span data-ttu-id="942d2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="942d2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="942d2-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="942d2-123">If-Match</span></span>  | <span data-ttu-id="942d2-p103">要更新的 **plannerProgressTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="942d2-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="942d2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="942d2-126">Request body</span></span>
<span data-ttu-id="942d2-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="942d2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="942d2-130">属性</span><span class="sxs-lookup"><span data-stu-id="942d2-130">Property</span></span>     | <span data-ttu-id="942d2-131">类型</span><span class="sxs-lookup"><span data-stu-id="942d2-131">Type</span></span>   |<span data-ttu-id="942d2-132">说明</span><span class="sxs-lookup"><span data-stu-id="942d2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="942d2-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="942d2-133">orderHint</span></span>|<span data-ttu-id="942d2-134">String</span><span class="sxs-lookup"><span data-stu-id="942d2-134">String</span></span>|<span data-ttu-id="942d2-135">用于对任务板的进度视图上的任务进行排序的提示值。</span><span class="sxs-lookup"><span data-stu-id="942d2-135">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="942d2-136">格式是在计划程序[中使用 order 提示](../resources/planner-order-hint-format.md)定义的。</span><span class="sxs-lookup"><span data-stu-id="942d2-136">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="942d2-137">响应</span><span class="sxs-lookup"><span data-stu-id="942d2-137">Response</span></span>

<span data-ttu-id="942d2-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="942d2-138">If successful, this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="942d2-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="942d2-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="942d2-142">示例</span><span class="sxs-lookup"><span data-stu-id="942d2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="942d2-143">请求</span><span class="sxs-lookup"><span data-stu-id="942d2-143">Request</span></span>
<span data-ttu-id="942d2-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="942d2-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/<id>/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="942d2-145">响应</span><span class="sxs-lookup"><span data-stu-id="942d2-145">Response</span></span>
<span data-ttu-id="942d2-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="942d2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="942d2-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="942d2-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="942d2-150">语言</span><span class="sxs-lookup"><span data-stu-id="942d2-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerprogresstaskboardtaskformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="942d2-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="942d2-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerprogresstaskboardtaskformat-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerprogresstaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/plannerprogresstaskboardtaskformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
