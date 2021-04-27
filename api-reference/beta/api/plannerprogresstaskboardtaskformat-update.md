---
title: 更新 plannerProgressTaskBoardTaskFormat
description: 更新 **plannerProgressTaskBoardTaskFormat** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 5a871fee114f43d5c6e54caa9b90639a59b71e0e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050001"
---
# <a name="update-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="b77c4-103">更新 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b77c4-103">Update plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="b77c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b77c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b77c4-105">更新 **plannerProgressTaskBoardTaskFormat** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b77c4-105">Update the properties of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b77c4-106">权限</span><span class="sxs-lookup"><span data-stu-id="b77c4-106">Permissions</span></span>
<span data-ttu-id="b77c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b77c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b77c4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b77c4-109">Permission type</span></span>      | <span data-ttu-id="b77c4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b77c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b77c4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b77c4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b77c4-112">Tasks.ReadWrite，Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b77c4-112">Tasks.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b77c4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b77c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b77c4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b77c4-114">Not supported.</span></span>    |
|<span data-ttu-id="b77c4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b77c4-115">Application</span></span> | <span data-ttu-id="b77c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b77c4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b77c4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b77c4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/{id}/progressTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="b77c4-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b77c4-118">Optional request headers</span></span>
| <span data-ttu-id="b77c4-119">名称</span><span class="sxs-lookup"><span data-stu-id="b77c4-119">Name</span></span>       | <span data-ttu-id="b77c4-120">说明</span><span class="sxs-lookup"><span data-stu-id="b77c4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b77c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b77c4-121">Authorization</span></span>  | <span data-ttu-id="b77c4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b77c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b77c4-124">If-Match</span><span class="sxs-lookup"><span data-stu-id="b77c4-124">If-Match</span></span>  | <span data-ttu-id="b77c4-p103">要更新的 **plannerProgressTaskBoardTaskFormat** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="b77c4-p103">Last known ETag value for the **plannerProgressTaskBoardTaskFormat** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b77c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b77c4-127">Request body</span></span>
<span data-ttu-id="b77c4-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b77c4-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b77c4-131">属性</span><span class="sxs-lookup"><span data-stu-id="b77c4-131">Property</span></span>     | <span data-ttu-id="b77c4-132">类型</span><span class="sxs-lookup"><span data-stu-id="b77c4-132">Type</span></span>   |<span data-ttu-id="b77c4-133">说明</span><span class="sxs-lookup"><span data-stu-id="b77c4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b77c4-134">orderHint</span><span class="sxs-lookup"><span data-stu-id="b77c4-134">orderHint</span></span>|<span data-ttu-id="b77c4-135">String</span><span class="sxs-lookup"><span data-stu-id="b77c4-135">String</span></span>|<span data-ttu-id="b77c4-136">用于对任务板"进度"视图上的任务排序的提示值。</span><span class="sxs-lookup"><span data-stu-id="b77c4-136">Hint value used to order the task on the Progress view of the Task Board.</span></span> <span data-ttu-id="b77c4-137">格式在使用 Planner 中的 [排序提示中定义](../resources/planner-order-hint-format.md)。</span><span class="sxs-lookup"><span data-stu-id="b77c4-137">The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="b77c4-138">响应</span><span class="sxs-lookup"><span data-stu-id="b77c4-138">Response</span></span>

<span data-ttu-id="b77c4-139">如果成功，此方法将返回 `204 No Content` 响应和空内容。</span><span class="sxs-lookup"><span data-stu-id="b77c4-139">If successful, this method returns `204 No Content` response and empty content.</span></span> <span data-ttu-id="b77c4-140">如果请求指定具有首选项的标头，则此方法在响应正文中返回 响应代码和更新的 `Prefer` `return=representation` `200 OK` [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b77c4-140">If the request specifies `Prefer` header with `return=representation` preference, then this method returns a `200 OK` response code and updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="b77c4-p107">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="b77c4-p107">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b77c4-144">示例</span><span class="sxs-lookup"><span data-stu-id="b77c4-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b77c4-145">请求</span><span class="sxs-lookup"><span data-stu-id="b77c4-145">Request</span></span>
<span data-ttu-id="b77c4-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b77c4-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b77c4-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b77c4-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/{id}/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
Prefer: return=representation
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
# <a name="c"></a>[<span data-ttu-id="b77c4-148">C#</span><span class="sxs-lookup"><span data-stu-id="b77c4-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-plannerprogresstaskboardtaskformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b77c4-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b77c4-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-plannerprogresstaskboardtaskformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b77c4-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b77c4-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-plannerprogresstaskboardtaskformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b77c4-151">Java</span><span class="sxs-lookup"><span data-stu-id="b77c4-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-plannerprogresstaskboardtaskformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b77c4-152">响应</span><span class="sxs-lookup"><span data-stu-id="b77c4-152">Response</span></span>
<span data-ttu-id="b77c4-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b77c4-153">Here is an example of the response.</span></span> <span data-ttu-id="b77c4-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b77c4-154">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


