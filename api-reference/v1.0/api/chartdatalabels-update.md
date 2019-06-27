---
title: 更新 chartdatalabels
description: 更新 chartdatalabels 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4ad66f2cbf4d78c1fd3570d9e98184370b0ef075
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272518"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="6754e-103">更新 chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="6754e-103">Update chartdatalabels</span></span>

<span data-ttu-id="6754e-104">更新 chartdatalabels 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6754e-104">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6754e-105">权限</span><span class="sxs-lookup"><span data-stu-id="6754e-105">Permissions</span></span>
<span data-ttu-id="6754e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6754e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6754e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6754e-108">Permission type</span></span>      | <span data-ttu-id="6754e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6754e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6754e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6754e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6754e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6754e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6754e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6754e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6754e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6754e-113">Not supported.</span></span>    |
|<span data-ttu-id="6754e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6754e-114">Application</span></span> | <span data-ttu-id="6754e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6754e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6754e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6754e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="6754e-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="6754e-117">Optional request headers</span></span>
| <span data-ttu-id="6754e-118">名称</span><span class="sxs-lookup"><span data-stu-id="6754e-118">Name</span></span>       | <span data-ttu-id="6754e-119">说明</span><span class="sxs-lookup"><span data-stu-id="6754e-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6754e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6754e-120">Authorization</span></span>  | <span data-ttu-id="6754e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6754e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6754e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6754e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6754e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6754e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6754e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6754e-126">Request body</span></span>
<span data-ttu-id="6754e-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6754e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6754e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6754e-130">Property</span></span>     | <span data-ttu-id="6754e-131">类型</span><span class="sxs-lookup"><span data-stu-id="6754e-131">Type</span></span>   |<span data-ttu-id="6754e-132">说明</span><span class="sxs-lookup"><span data-stu-id="6754e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6754e-133">position</span><span class="sxs-lookup"><span data-stu-id="6754e-133">position</span></span>|<span data-ttu-id="6754e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6754e-134">string</span></span>|<span data-ttu-id="6754e-135">表示数据标签的位置的 DataLabelPosition 值。</span><span class="sxs-lookup"><span data-stu-id="6754e-135">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="6754e-136">可能的值为: `None`、 `Center`、 `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom`、、、、、、、、 `Callout` `BestFit`。</span><span class="sxs-lookup"><span data-stu-id="6754e-136">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="6754e-137">Separator</span><span class="sxs-lookup"><span data-stu-id="6754e-137">separator</span></span>|<span data-ttu-id="6754e-138">string</span><span class="sxs-lookup"><span data-stu-id="6754e-138">string</span></span>|<span data-ttu-id="6754e-139">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="6754e-139">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="6754e-140">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="6754e-140">showBubbleSize</span></span>|<span data-ttu-id="6754e-141">boolean</span><span class="sxs-lookup"><span data-stu-id="6754e-141">boolean</span></span>|<span data-ttu-id="6754e-142">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6754e-142">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="6754e-143">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="6754e-143">showCategoryName</span></span>|<span data-ttu-id="6754e-144">boolean</span><span class="sxs-lookup"><span data-stu-id="6754e-144">boolean</span></span>|<span data-ttu-id="6754e-145">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6754e-145">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="6754e-146">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="6754e-146">showLegendKey</span></span>|<span data-ttu-id="6754e-147">boolean</span><span class="sxs-lookup"><span data-stu-id="6754e-147">boolean</span></span>|<span data-ttu-id="6754e-148">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6754e-148">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="6754e-149">showPercentage</span><span class="sxs-lookup"><span data-stu-id="6754e-149">showPercentage</span></span>|<span data-ttu-id="6754e-150">boolean</span><span class="sxs-lookup"><span data-stu-id="6754e-150">boolean</span></span>|<span data-ttu-id="6754e-151">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6754e-151">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="6754e-152">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="6754e-152">showSeriesName</span></span>|<span data-ttu-id="6754e-153">boolean</span><span class="sxs-lookup"><span data-stu-id="6754e-153">boolean</span></span>|<span data-ttu-id="6754e-154">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6754e-154">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="6754e-155">showValue</span><span class="sxs-lookup"><span data-stu-id="6754e-155">showValue</span></span>|<span data-ttu-id="6754e-156">布尔</span><span class="sxs-lookup"><span data-stu-id="6754e-156">boolean</span></span>|<span data-ttu-id="6754e-157">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="6754e-157">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="6754e-158">响应</span><span class="sxs-lookup"><span data-stu-id="6754e-158">Response</span></span>

<span data-ttu-id="6754e-159">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookChartDataLabels](../resources/chartdatalabels.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6754e-159">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6754e-160">示例</span><span class="sxs-lookup"><span data-stu-id="6754e-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6754e-161">请求</span><span class="sxs-lookup"><span data-stu-id="6754e-161">Request</span></span>
<span data-ttu-id="6754e-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6754e-162">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
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
##### <a name="response"></a><span data-ttu-id="6754e-163">响应</span><span class="sxs-lookup"><span data-stu-id="6754e-163">Response</span></span>
<span data-ttu-id="6754e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6754e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6754e-167">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6754e-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6754e-168">C#</span><span class="sxs-lookup"><span data-stu-id="6754e-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6754e-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="6754e-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6754e-170">目标-C</span><span class="sxs-lookup"><span data-stu-id="6754e-170">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartdatalabels-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartdatalabels-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
