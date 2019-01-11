---
title: 更新 chartdatalabels
description: 更新 chartdatalabels 对象的属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b430d411a10b09ebf8a160b56bd83dcaadeee036
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824176"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="53366-103">更新 chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="53366-103">Update chartdatalabels</span></span>

> <span data-ttu-id="53366-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="53366-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53366-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53366-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53366-106">更新 chartdatalabels 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53366-106">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="53366-107">权限</span><span class="sxs-lookup"><span data-stu-id="53366-107">Permissions</span></span>
<span data-ttu-id="53366-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53366-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53366-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53366-110">Permission type</span></span>      | <span data-ttu-id="53366-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53366-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53366-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53366-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53366-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53366-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53366-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53366-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53366-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53366-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53366-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53366-116">Application</span></span> | <span data-ttu-id="53366-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="53366-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53366-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53366-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="53366-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="53366-119">Optional request headers</span></span>
| <span data-ttu-id="53366-120">名称</span><span class="sxs-lookup"><span data-stu-id="53366-120">Name</span></span>       | <span data-ttu-id="53366-121">说明</span><span class="sxs-lookup"><span data-stu-id="53366-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="53366-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53366-122">Authorization</span></span>  | <span data-ttu-id="53366-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53366-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53366-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53366-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="53366-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="53366-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53366-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="53366-128">Request body</span></span>
<span data-ttu-id="53366-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="53366-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="53366-132">属性</span><span class="sxs-lookup"><span data-stu-id="53366-132">Property</span></span>     | <span data-ttu-id="53366-133">类型</span><span class="sxs-lookup"><span data-stu-id="53366-133">Type</span></span>   |<span data-ttu-id="53366-134">说明</span><span class="sxs-lookup"><span data-stu-id="53366-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53366-135">position</span><span class="sxs-lookup"><span data-stu-id="53366-135">position</span></span>|<span data-ttu-id="53366-136">string</span><span class="sxs-lookup"><span data-stu-id="53366-136">string</span></span>|<span data-ttu-id="53366-p106">表示数据标签位置的 DataLabelPosition 值。可能的值是：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。</span><span class="sxs-lookup"><span data-stu-id="53366-p106">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="53366-139">separator</span><span class="sxs-lookup"><span data-stu-id="53366-139">separator</span></span>|<span data-ttu-id="53366-140">string</span><span class="sxs-lookup"><span data-stu-id="53366-140">string</span></span>|<span data-ttu-id="53366-141">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="53366-141">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="53366-142">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="53366-142">showBubbleSize</span></span>|<span data-ttu-id="53366-143">boolean</span><span class="sxs-lookup"><span data-stu-id="53366-143">boolean</span></span>|<span data-ttu-id="53366-144">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="53366-144">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="53366-145">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="53366-145">showCategoryName</span></span>|<span data-ttu-id="53366-146">boolean</span><span class="sxs-lookup"><span data-stu-id="53366-146">boolean</span></span>|<span data-ttu-id="53366-147">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="53366-147">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="53366-148">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="53366-148">showLegendKey</span></span>|<span data-ttu-id="53366-149">boolean</span><span class="sxs-lookup"><span data-stu-id="53366-149">boolean</span></span>|<span data-ttu-id="53366-150">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="53366-150">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="53366-151">showPercentage</span><span class="sxs-lookup"><span data-stu-id="53366-151">showPercentage</span></span>|<span data-ttu-id="53366-152">boolean</span><span class="sxs-lookup"><span data-stu-id="53366-152">boolean</span></span>|<span data-ttu-id="53366-153">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="53366-153">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="53366-154">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="53366-154">showSeriesName</span></span>|<span data-ttu-id="53366-155">boolean</span><span class="sxs-lookup"><span data-stu-id="53366-155">boolean</span></span>|<span data-ttu-id="53366-156">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="53366-156">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="53366-157">showValue</span><span class="sxs-lookup"><span data-stu-id="53366-157">showValue</span></span>|<span data-ttu-id="53366-158">boolean</span><span class="sxs-lookup"><span data-stu-id="53366-158">boolean</span></span>|<span data-ttu-id="53366-159">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="53366-159">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="53366-160">响应</span><span class="sxs-lookup"><span data-stu-id="53366-160">Response</span></span>

<span data-ttu-id="53366-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartDataLabels](../resources/chartdatalabels.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53366-161">If successful, this method returns a `200 OK` response code and updated [ChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53366-162">示例</span><span class="sxs-lookup"><span data-stu-id="53366-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53366-163">请求</span><span class="sxs-lookup"><span data-stu-id="53366-163">Request</span></span>
<span data-ttu-id="53366-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53366-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="53366-165">响应</span><span class="sxs-lookup"><span data-stu-id="53366-165">Response</span></span>
<span data-ttu-id="53366-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53366-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
