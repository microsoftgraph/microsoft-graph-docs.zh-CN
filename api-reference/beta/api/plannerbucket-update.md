---
title: 更新 plannerbucket
description: 更新 **plannerbucket** 对象的属性。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e85cdc1ffa1781420b5ef911147f25ef97a726dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517825"
---
# <a name="update-plannerbucket"></a><span data-ttu-id="4cb97-103">更新 plannerbucket</span><span class="sxs-lookup"><span data-stu-id="4cb97-103">Update plannerbucket</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cb97-104">更新 **plannerbucket** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4cb97-104">Update the properties of **plannerbucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cb97-105">权限</span><span class="sxs-lookup"><span data-stu-id="4cb97-105">Permissions</span></span>
<span data-ttu-id="4cb97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cb97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb97-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cb97-108">Permission type</span></span>      | <span data-ttu-id="4cb97-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cb97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cb97-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cb97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4cb97-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cb97-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4cb97-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cb97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb97-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cb97-113">Not supported.</span></span>    |
|<span data-ttu-id="4cb97-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4cb97-114">Application</span></span> | <span data-ttu-id="4cb97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cb97-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cb97-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cb97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/buckets/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="4cb97-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4cb97-117">Optional request headers</span></span>
| <span data-ttu-id="4cb97-118">名称</span><span class="sxs-lookup"><span data-stu-id="4cb97-118">Name</span></span>       | <span data-ttu-id="4cb97-119">说明</span><span class="sxs-lookup"><span data-stu-id="4cb97-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4cb97-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cb97-120">Authorization</span></span>  | <span data-ttu-id="4cb97-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4cb97-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4cb97-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="4cb97-123">If-Match</span></span>  | <span data-ttu-id="4cb97-p103">要更新的 **plannerBucket** 的上次已知 ETag 值。必需。</span><span class="sxs-lookup"><span data-stu-id="4cb97-p103">Last known ETag value for the **plannerBucket** to be updated. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cb97-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cb97-126">Request body</span></span>
<span data-ttu-id="4cb97-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4cb97-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4cb97-130">属性</span><span class="sxs-lookup"><span data-stu-id="4cb97-130">Property</span></span>     | <span data-ttu-id="4cb97-131">类型</span><span class="sxs-lookup"><span data-stu-id="4cb97-131">Type</span></span>   |<span data-ttu-id="4cb97-132">说明</span><span class="sxs-lookup"><span data-stu-id="4cb97-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cb97-133">name</span><span class="sxs-lookup"><span data-stu-id="4cb97-133">name</span></span>|<span data-ttu-id="4cb97-134">String</span><span class="sxs-lookup"><span data-stu-id="4cb97-134">String</span></span>|<span data-ttu-id="4cb97-135">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="4cb97-135">Name of the bucket.</span></span>|
|<span data-ttu-id="4cb97-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="4cb97-136">orderHint</span></span>|<span data-ttu-id="4cb97-137">字符串</span><span class="sxs-lookup"><span data-stu-id="4cb97-137">String</span></span>|<span data-ttu-id="4cb97-p105">用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](../resources/planner-order-hint-format.md)定义中。</span><span class="sxs-lookup"><span data-stu-id="4cb97-p105">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](../resources/planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="4cb97-140">planId</span><span class="sxs-lookup"><span data-stu-id="4cb97-140">planId</span></span>|<span data-ttu-id="4cb97-141">String</span><span class="sxs-lookup"><span data-stu-id="4cb97-141">String</span></span>|<span data-ttu-id="4cb97-142">此存储桶所属的计划 id。</span><span class="sxs-lookup"><span data-stu-id="4cb97-142">Plan id to which the bucket belongs.</span></span>|

## <a name="response"></a><span data-ttu-id="4cb97-143">响应</span><span class="sxs-lookup"><span data-stu-id="4cb97-143">Response</span></span>

<span data-ttu-id="4cb97-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [plannerBucket](../resources/plannerbucket.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4cb97-144">If successful, this method returns a `200 OK` response code and updated [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="4cb97-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法处理的最常见的错误为 400、403、404、409 和 412 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="4cb97-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4cb97-148">示例</span><span class="sxs-lookup"><span data-stu-id="4cb97-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cb97-149">请求</span><span class="sxs-lookup"><span data-stu-id="4cb97-149">Request</span></span>
<span data-ttu-id="4cb97-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4cb97-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR
Content-type: application/json
Content-length: 27
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "name": "Development"
}
```
##### <a name="response"></a><span data-ttu-id="4cb97-151">响应</span><span class="sxs-lookup"><span data-stu-id="4cb97-151">Response</span></span>
<span data-ttu-id="4cb97-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4cb97-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Development",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerbucket-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
