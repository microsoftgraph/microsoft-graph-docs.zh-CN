---
title: 更新图表
description: 更新 chart 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d1377a0a8c19538ea1c0c19483512736e129559
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516383"
---
# <a name="update-chart"></a><span data-ttu-id="9389d-103">更新图表</span><span class="sxs-lookup"><span data-stu-id="9389d-103">Update chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9389d-104">更新 chart 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9389d-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9389d-105">权限</span><span class="sxs-lookup"><span data-stu-id="9389d-105">Permissions</span></span>
<span data-ttu-id="9389d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9389d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9389d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9389d-108">Permission type</span></span>      | <span data-ttu-id="9389d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9389d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9389d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9389d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9389d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9389d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9389d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9389d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9389d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9389d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9389d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9389d-114">Application</span></span> | <span data-ttu-id="9389d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9389d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9389d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9389d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="9389d-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="9389d-117">Optional request headers</span></span>
| <span data-ttu-id="9389d-118">Name</span><span class="sxs-lookup"><span data-stu-id="9389d-118">Name</span></span>       | <span data-ttu-id="9389d-119">说明</span><span class="sxs-lookup"><span data-stu-id="9389d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9389d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9389d-120">Authorization</span></span>  | <span data-ttu-id="9389d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9389d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9389d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9389d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9389d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9389d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9389d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9389d-126">Request body</span></span>
<span data-ttu-id="9389d-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9389d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9389d-130">属性</span><span class="sxs-lookup"><span data-stu-id="9389d-130">Property</span></span>     | <span data-ttu-id="9389d-131">类型</span><span class="sxs-lookup"><span data-stu-id="9389d-131">Type</span></span>   |<span data-ttu-id="9389d-132">说明</span><span class="sxs-lookup"><span data-stu-id="9389d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9389d-133">height</span><span class="sxs-lookup"><span data-stu-id="9389d-133">height</span></span>|<span data-ttu-id="9389d-134">double</span><span class="sxs-lookup"><span data-stu-id="9389d-134">double</span></span>|<span data-ttu-id="9389d-135">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="9389d-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="9389d-136">left</span><span class="sxs-lookup"><span data-stu-id="9389d-136">left</span></span>|<span data-ttu-id="9389d-137">double</span><span class="sxs-lookup"><span data-stu-id="9389d-137">double</span></span>|<span data-ttu-id="9389d-138">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="9389d-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="9389d-139">name</span><span class="sxs-lookup"><span data-stu-id="9389d-139">name</span></span>|<span data-ttu-id="9389d-140">string</span><span class="sxs-lookup"><span data-stu-id="9389d-140">string</span></span>|<span data-ttu-id="9389d-141">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="9389d-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="9389d-142">top</span><span class="sxs-lookup"><span data-stu-id="9389d-142">top</span></span>|<span data-ttu-id="9389d-143">double</span><span class="sxs-lookup"><span data-stu-id="9389d-143">double</span></span>|<span data-ttu-id="9389d-144">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="9389d-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="9389d-145">width</span><span class="sxs-lookup"><span data-stu-id="9389d-145">width</span></span>|<span data-ttu-id="9389d-146">double</span><span class="sxs-lookup"><span data-stu-id="9389d-146">double</span></span>|<span data-ttu-id="9389d-147">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="9389d-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="9389d-148">响应</span><span class="sxs-lookup"><span data-stu-id="9389d-148">Response</span></span>

<span data-ttu-id="9389d-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9389d-149">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9389d-150">示例</span><span class="sxs-lookup"><span data-stu-id="9389d-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9389d-151">请求</span><span class="sxs-lookup"><span data-stu-id="9389d-151">Request</span></span>
<span data-ttu-id="9389d-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9389d-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="9389d-153">响应</span><span class="sxs-lookup"><span data-stu-id="9389d-153">Response</span></span>
<span data-ttu-id="9389d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9389d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
