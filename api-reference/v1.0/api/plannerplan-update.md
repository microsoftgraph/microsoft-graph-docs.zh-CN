---
title: 更新 plannerPlan
description: 更新**plannerPlan**对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 72811b69c77e12d84bbb29813b8b3f1019ab2f05
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608783"
---
# <a name="update-plannerplan"></a><span data-ttu-id="8479d-103">更新 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="8479d-103">Update plannerPlan</span></span>

<span data-ttu-id="8479d-104">更新**plannerPlan**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8479d-104">Update the properties of **plannerPlan** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8479d-105">权限</span><span class="sxs-lookup"><span data-stu-id="8479d-105">Permissions</span></span>
<span data-ttu-id="8479d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8479d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8479d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8479d-108">Permission type</span></span>      | <span data-ttu-id="8479d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8479d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8479d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8479d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8479d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8479d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8479d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8479d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8479d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8479d-113">Not supported.</span></span>    |
|<span data-ttu-id="8479d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8479d-114">Application</span></span> | <span data-ttu-id="8479d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8479d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8479d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8479d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/plans/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8479d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8479d-117">Request headers</span></span>

| <span data-ttu-id="8479d-118">名称</span><span class="sxs-lookup"><span data-stu-id="8479d-118">Name</span></span>       | <span data-ttu-id="8479d-119">说明</span><span class="sxs-lookup"><span data-stu-id="8479d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8479d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8479d-120">Authorization</span></span>  | <span data-ttu-id="8479d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8479d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8479d-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="8479d-123">If-Match</span></span>  | <span data-ttu-id="8479d-p103">要更新的 plannerPlan 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="8479d-p103">Last known ETag value for the plannerPlan to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8479d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8479d-126">Request body</span></span>
<span data-ttu-id="8479d-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8479d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8479d-130">属性</span><span class="sxs-lookup"><span data-stu-id="8479d-130">Property</span></span>     | <span data-ttu-id="8479d-131">类型</span><span class="sxs-lookup"><span data-stu-id="8479d-131">Type</span></span>   |<span data-ttu-id="8479d-132">说明</span><span class="sxs-lookup"><span data-stu-id="8479d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8479d-133">owner</span><span class="sxs-lookup"><span data-stu-id="8479d-133">owner</span></span>|<span data-ttu-id="8479d-134">String</span><span class="sxs-lookup"><span data-stu-id="8479d-134">String</span></span>|<span data-ttu-id="8479d-p105">拥有计划的[组](../resources/group.md)`id`。必须存在有效的组才能设置此字段。设置后，只能由所有者更新此字段。</span><span class="sxs-lookup"><span data-stu-id="8479d-p105">[Group](../resources/group.md) `id` by which the plan is owned. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="8479d-138">title</span><span class="sxs-lookup"><span data-stu-id="8479d-138">title</span></span>|<span data-ttu-id="8479d-139">String</span><span class="sxs-lookup"><span data-stu-id="8479d-139">String</span></span>|<span data-ttu-id="8479d-140">计划的标题。</span><span class="sxs-lookup"><span data-stu-id="8479d-140">Title of the plan.</span></span>|

## <a name="response"></a><span data-ttu-id="8479d-141">响应</span><span class="sxs-lookup"><span data-stu-id="8479d-141">Response</span></span>

<span data-ttu-id="8479d-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerPlan](../resources/plannerplan.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8479d-142">If successful, this method returns a `200 OK` response code and updated [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="8479d-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="8479d-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8479d-146">示例</span><span class="sxs-lookup"><span data-stu-id="8479d-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8479d-147">请求</span><span class="sxs-lookup"><span data-stu-id="8479d-147">Request</span></span>
<span data-ttu-id="8479d-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8479d-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerplan"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
Content-type: application/json
Content-length: 29
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "title": "title-value"
}
```
##### <a name="response"></a><span data-ttu-id="8479d-149">响应</span><span class="sxs-lookup"><span data-stu-id="8479d-149">Response</span></span>
<span data-ttu-id="8479d-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8479d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8479d-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8479d-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8479d-154">语言</span><span class="sxs-lookup"><span data-stu-id="8479d-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_plannerplan-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8479d-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="8479d-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_plannerplan-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerplan",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/plannerplan-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/plannerplan-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
