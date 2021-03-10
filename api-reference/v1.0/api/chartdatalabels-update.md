---
title: 更新 chartdatalabels
description: 更新 chartdatalabels 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 91efcaf38191b4f975ce27d1219fc3ba7c862b91
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573906"
---
# <a name="update-chartdatalabels"></a><span data-ttu-id="0012b-103">更新 chartdatalabels</span><span class="sxs-lookup"><span data-stu-id="0012b-103">Update chartdatalabels</span></span>

<span data-ttu-id="0012b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0012b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0012b-105">更新 chartdatalabels 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0012b-105">Update the properties of chartdatalabels object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0012b-106">权限</span><span class="sxs-lookup"><span data-stu-id="0012b-106">Permissions</span></span>
<span data-ttu-id="0012b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0012b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0012b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0012b-109">Permission type</span></span>      | <span data-ttu-id="0012b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0012b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0012b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0012b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0012b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0012b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0012b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0012b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0012b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0012b-114">Not supported.</span></span>    |
|<span data-ttu-id="0012b-115">Application</span><span class="sxs-lookup"><span data-stu-id="0012b-115">Application</span></span> | <span data-ttu-id="0012b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0012b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0012b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0012b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/dataLabels
```
## <a name="optional-request-headers"></a><span data-ttu-id="0012b-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0012b-118">Optional request headers</span></span>
| <span data-ttu-id="0012b-119">名称</span><span class="sxs-lookup"><span data-stu-id="0012b-119">Name</span></span>       | <span data-ttu-id="0012b-120">说明</span><span class="sxs-lookup"><span data-stu-id="0012b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0012b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0012b-121">Authorization</span></span>  | <span data-ttu-id="0012b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0012b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0012b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0012b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0012b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0012b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0012b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0012b-127">Request body</span></span>
<span data-ttu-id="0012b-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0012b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0012b-131">属性</span><span class="sxs-lookup"><span data-stu-id="0012b-131">Property</span></span>     | <span data-ttu-id="0012b-132">类型</span><span class="sxs-lookup"><span data-stu-id="0012b-132">Type</span></span>   |<span data-ttu-id="0012b-133">说明</span><span class="sxs-lookup"><span data-stu-id="0012b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0012b-134">position</span><span class="sxs-lookup"><span data-stu-id="0012b-134">position</span></span>|<span data-ttu-id="0012b-135">string</span><span class="sxs-lookup"><span data-stu-id="0012b-135">string</span></span>|<span data-ttu-id="0012b-136">表示数据标签的位置的 DataLabelPosition 值。</span><span class="sxs-lookup"><span data-stu-id="0012b-136">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="0012b-137">可能的值是： `None` ， `Center` ， ， ， ， ， `InsideEnd` ， `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom` `BestFit` `Callout` 。</span><span class="sxs-lookup"><span data-stu-id="0012b-137">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="0012b-138">Separator</span><span class="sxs-lookup"><span data-stu-id="0012b-138">separator</span></span>|<span data-ttu-id="0012b-139">string</span><span class="sxs-lookup"><span data-stu-id="0012b-139">string</span></span>|<span data-ttu-id="0012b-140">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="0012b-140">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0012b-141">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0012b-141">showBubbleSize</span></span>|<span data-ttu-id="0012b-142">布尔</span><span class="sxs-lookup"><span data-stu-id="0012b-142">boolean</span></span>|<span data-ttu-id="0012b-143">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0012b-143">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0012b-144">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0012b-144">showCategoryName</span></span>|<span data-ttu-id="0012b-145">布尔</span><span class="sxs-lookup"><span data-stu-id="0012b-145">boolean</span></span>|<span data-ttu-id="0012b-146">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0012b-146">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0012b-147">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0012b-147">showLegendKey</span></span>|<span data-ttu-id="0012b-148">布尔</span><span class="sxs-lookup"><span data-stu-id="0012b-148">boolean</span></span>|<span data-ttu-id="0012b-149">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0012b-149">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0012b-150">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0012b-150">showPercentage</span></span>|<span data-ttu-id="0012b-151">布尔</span><span class="sxs-lookup"><span data-stu-id="0012b-151">boolean</span></span>|<span data-ttu-id="0012b-152">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0012b-152">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0012b-153">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0012b-153">showSeriesName</span></span>|<span data-ttu-id="0012b-154">布尔</span><span class="sxs-lookup"><span data-stu-id="0012b-154">boolean</span></span>|<span data-ttu-id="0012b-155">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0012b-155">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0012b-156">showValue</span><span class="sxs-lookup"><span data-stu-id="0012b-156">showValue</span></span>|<span data-ttu-id="0012b-157">布尔</span><span class="sxs-lookup"><span data-stu-id="0012b-157">boolean</span></span>|<span data-ttu-id="0012b-158">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0012b-158">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="response"></a><span data-ttu-id="0012b-159">响应</span><span class="sxs-lookup"><span data-stu-id="0012b-159">Response</span></span>

<span data-ttu-id="0012b-160">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [WorkbookChartDataLabels](../resources/chartdatalabels.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0012b-160">If successful, this method returns a `200 OK` response code and updated [WorkbookChartDataLabels](../resources/chartdatalabels.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0012b-161">示例</span><span class="sxs-lookup"><span data-stu-id="0012b-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0012b-162">请求</span><span class="sxs-lookup"><span data-stu-id="0012b-162">Request</span></span>
<span data-ttu-id="0012b-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0012b-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0012b-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="0012b-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0012b-165">C#</span><span class="sxs-lookup"><span data-stu-id="0012b-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartdatalabels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0012b-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0012b-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartdatalabels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0012b-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0012b-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartdatalabels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0012b-168">Java</span><span class="sxs-lookup"><span data-stu-id="0012b-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartdatalabels-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0012b-169">响应</span><span class="sxs-lookup"><span data-stu-id="0012b-169">Response</span></span>
<span data-ttu-id="0012b-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0012b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartdatalabels",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

