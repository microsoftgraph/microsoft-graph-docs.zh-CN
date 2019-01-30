---
title: 更新 chartdatalabels
description: 更新 chartdatalabels 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b7eb067bed747ae2532939e61a9e0dec58ff4655
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640131"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="1698a-103">更新 chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="1698a-103">Update chartdatalabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1698a-104">更新 chartdatalabels 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1698a-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1698a-105">权限</span><span class="sxs-lookup"><span data-stu-id="1698a-105">Permissions</span></span>
<span data-ttu-id="1698a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1698a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1698a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1698a-108">Permission type</span></span>      | <span data-ttu-id="1698a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1698a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1698a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1698a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1698a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1698a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1698a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1698a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1698a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1698a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1698a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1698a-114">Application</span></span> | <span data-ttu-id="1698a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1698a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1698a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1698a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="1698a-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="1698a-117">Optional request headers</span></span>
| <span data-ttu-id="1698a-118">名称</span><span class="sxs-lookup"><span data-stu-id="1698a-118">Name</span></span>       | <span data-ttu-id="1698a-119">说明</span><span class="sxs-lookup"><span data-stu-id="1698a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1698a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1698a-120">Authorization</span></span>  | <span data-ttu-id="1698a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1698a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1698a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1698a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1698a-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1698a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1698a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1698a-126">Request body</span></span>
<span data-ttu-id="1698a-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1698a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1698a-130">属性</span><span class="sxs-lookup"><span data-stu-id="1698a-130">Property</span></span>     | <span data-ttu-id="1698a-131">类型</span><span class="sxs-lookup"><span data-stu-id="1698a-131">Type</span></span>   |<span data-ttu-id="1698a-132">说明</span><span class="sxs-lookup"><span data-stu-id="1698a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1698a-133">position</span><span class="sxs-lookup"><span data-stu-id="1698a-133">position</span></span>|<span data-ttu-id="1698a-134">string</span><span class="sxs-lookup"><span data-stu-id="1698a-134">string</span></span>|<span data-ttu-id="1698a-p105">表示数据标签位置的 DataLabelPosition 值。可能的值是：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。</span><span class="sxs-lookup"><span data-stu-id="1698a-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="1698a-137">separator</span><span class="sxs-lookup"><span data-stu-id="1698a-137">separator</span></span>|<span data-ttu-id="1698a-138">string</span><span class="sxs-lookup"><span data-stu-id="1698a-138">string</span></span>|<span data-ttu-id="1698a-139">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="1698a-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="1698a-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="1698a-140">showBubbleSize</span></span>|<span data-ttu-id="1698a-141">boolean</span><span class="sxs-lookup"><span data-stu-id="1698a-141">boolean</span></span>|<span data-ttu-id="1698a-142">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1698a-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="1698a-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="1698a-143">showCategoryName</span></span>|<span data-ttu-id="1698a-144">boolean</span><span class="sxs-lookup"><span data-stu-id="1698a-144">boolean</span></span>|<span data-ttu-id="1698a-145">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1698a-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="1698a-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="1698a-146">showLegendKey</span></span>|<span data-ttu-id="1698a-147">boolean</span><span class="sxs-lookup"><span data-stu-id="1698a-147">boolean</span></span>|<span data-ttu-id="1698a-148">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1698a-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="1698a-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="1698a-149">showPercentage</span></span>|<span data-ttu-id="1698a-150">boolean</span><span class="sxs-lookup"><span data-stu-id="1698a-150">boolean</span></span>|<span data-ttu-id="1698a-151">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1698a-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="1698a-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="1698a-152">showSeriesName</span></span>|<span data-ttu-id="1698a-153">boolean</span><span class="sxs-lookup"><span data-stu-id="1698a-153">boolean</span></span>|<span data-ttu-id="1698a-154">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1698a-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="1698a-155">showValue</span><span class="sxs-lookup"><span data-stu-id="1698a-155">showValue</span></span>|<span data-ttu-id="1698a-156">boolean</span><span class="sxs-lookup"><span data-stu-id="1698a-156">boolean</span></span>|<span data-ttu-id="1698a-157">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="1698a-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="1698a-158">响应</span><span class="sxs-lookup"><span data-stu-id="1698a-158">Response</span></span>

<span data-ttu-id="1698a-159">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartDataLabels](../resources/chartdatalabels.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1698a-159">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1698a-160">示例</span><span class="sxs-lookup"><span data-stu-id="1698a-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1698a-161">请求</span><span class="sxs-lookup"><span data-stu-id="1698a-161">Request</span></span>
<span data-ttu-id="1698a-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1698a-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/datalabels
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```
##### <a name="response"></a><span data-ttu-id="1698a-163">响应</span><span class="sxs-lookup"><span data-stu-id="1698a-163">Response</span></span>
<span data-ttu-id="1698a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1698a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartDataLabels"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "position": "position-value",
  "showValue": true,
  "showSeriesName": true,
  "showCategoryName": true,
  "showLegendKey": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartdatalabels-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
