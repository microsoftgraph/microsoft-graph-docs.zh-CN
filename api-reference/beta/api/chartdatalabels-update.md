---
title: 更新 workbookChartDataLabels
description: 更新 workbookchartdatalabels 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 72e8704c986a1339e2a1ac6197b27f926bbbb674
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958779"
---
# <a name="update-workbookchartdatalabels"></a><span data-ttu-id="dac66-103">更新 workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="dac66-103">Update workbookChartDataLabels</span></span>

<span data-ttu-id="dac66-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dac66-105">更新 chartdatalabels 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dac66-105">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dac66-106">权限</span><span class="sxs-lookup"><span data-stu-id="dac66-106">Permissions</span></span>
<span data-ttu-id="dac66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dac66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac66-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dac66-109">Permission type</span></span>      | <span data-ttu-id="dac66-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dac66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dac66-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dac66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dac66-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dac66-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dac66-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dac66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac66-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dac66-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dac66-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dac66-115">Application</span></span> | <span data-ttu-id="dac66-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dac66-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dac66-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dac66-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/datalabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="dac66-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="dac66-118">Optional request headers</span></span>
| <span data-ttu-id="dac66-119">名称</span><span class="sxs-lookup"><span data-stu-id="dac66-119">Name</span></span>       | <span data-ttu-id="dac66-120">说明</span><span class="sxs-lookup"><span data-stu-id="dac66-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dac66-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dac66-121">Authorization</span></span>  | <span data-ttu-id="dac66-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dac66-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dac66-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dac66-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="dac66-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="dac66-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dac66-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dac66-127">Request body</span></span>
<span data-ttu-id="dac66-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="dac66-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dac66-131">属性</span><span class="sxs-lookup"><span data-stu-id="dac66-131">Property</span></span>     | <span data-ttu-id="dac66-132">类型</span><span class="sxs-lookup"><span data-stu-id="dac66-132">Type</span></span>   |<span data-ttu-id="dac66-133">说明</span><span class="sxs-lookup"><span data-stu-id="dac66-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dac66-134">position</span><span class="sxs-lookup"><span data-stu-id="dac66-134">position</span></span>|<span data-ttu-id="dac66-135">string</span><span class="sxs-lookup"><span data-stu-id="dac66-135">string</span></span>|<span data-ttu-id="dac66-p105">表示数据标签位置的 DataLabelPosition 值。可能的值是：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。</span><span class="sxs-lookup"><span data-stu-id="dac66-p105">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="dac66-138">separator</span><span class="sxs-lookup"><span data-stu-id="dac66-138">separator</span></span>|<span data-ttu-id="dac66-139">string</span><span class="sxs-lookup"><span data-stu-id="dac66-139">string</span></span>|<span data-ttu-id="dac66-140">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="dac66-140">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="dac66-141">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="dac66-141">showBubbleSize</span></span>|<span data-ttu-id="dac66-142">布尔</span><span class="sxs-lookup"><span data-stu-id="dac66-142">boolean</span></span>|<span data-ttu-id="dac66-143">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="dac66-143">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="dac66-144">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="dac66-144">showCategoryName</span></span>|<span data-ttu-id="dac66-145">布尔</span><span class="sxs-lookup"><span data-stu-id="dac66-145">boolean</span></span>|<span data-ttu-id="dac66-146">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="dac66-146">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="dac66-147">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="dac66-147">showLegendKey</span></span>|<span data-ttu-id="dac66-148">布尔</span><span class="sxs-lookup"><span data-stu-id="dac66-148">boolean</span></span>|<span data-ttu-id="dac66-149">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="dac66-149">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="dac66-150">showPercentage</span><span class="sxs-lookup"><span data-stu-id="dac66-150">showPercentage</span></span>|<span data-ttu-id="dac66-151">布尔</span><span class="sxs-lookup"><span data-stu-id="dac66-151">boolean</span></span>|<span data-ttu-id="dac66-152">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="dac66-152">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="dac66-153">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="dac66-153">showSeriesName</span></span>|<span data-ttu-id="dac66-154">布尔</span><span class="sxs-lookup"><span data-stu-id="dac66-154">boolean</span></span>|<span data-ttu-id="dac66-155">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="dac66-155">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="dac66-156">showValue</span><span class="sxs-lookup"><span data-stu-id="dac66-156">showValue</span></span>|<span data-ttu-id="dac66-157">布尔</span><span class="sxs-lookup"><span data-stu-id="dac66-157">boolean</span></span>|<span data-ttu-id="dac66-158">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="dac66-158">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="dac66-159">响应</span><span class="sxs-lookup"><span data-stu-id="dac66-159">Response</span></span>

<span data-ttu-id="dac66-160">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workbookChartDataLabels](../resources/workbookchartdatalabels.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dac66-160">If successful, this method returns a `200 OK` response code and updated [workbookChartDataLabels](../resources/workbookchartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dac66-161">示例</span><span class="sxs-lookup"><span data-stu-id="dac66-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dac66-162">请求</span><span class="sxs-lookup"><span data-stu-id="dac66-162">Request</span></span>
<span data-ttu-id="dac66-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dac66-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dac66-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="dac66-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartdatalabels"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels
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
# <a name="c"></a>[<span data-ttu-id="dac66-165">C#</span><span class="sxs-lookup"><span data-stu-id="dac66-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dac66-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dac66-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dac66-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dac66-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dac66-168">Java</span><span class="sxs-lookup"><span data-stu-id="dac66-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dac66-169">响应</span><span class="sxs-lookup"><span data-stu-id="dac66-169">Response</span></span>
<span data-ttu-id="dac66-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dac66-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->


