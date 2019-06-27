---
title: 通过 Microsoft Graph 更新 Excel 区域格式
description: 下面的几个示例展示了如何更新指定区域的 RangeFormat、RangeFill 和 RangeFont 属性。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 8eb2bdb587ca32a61f9f3804491df2e81e6e5f4b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272945"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="dfed4-103">使用 Microsoft Graph 更新 Excel 中的区域格式</span><span class="sxs-lookup"><span data-stu-id="dfed4-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="dfed4-104">以下示例演示如何更新指定区域的 [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0)、[RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0) 和 [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="dfed4-105">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="dfed4-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="dfed4-107">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-107">Request</span></span>
<span data-ttu-id="dfed4-108">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="dfed4-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-109">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-109">Response</span></span>
<span data-ttu-id="dfed4-p101">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "General",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-113">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-113">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-114">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-114">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-115">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-115">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-116">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-116">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="dfed4-117">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-117">Request</span></span>
<span data-ttu-id="dfed4-118">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="dfed4-118">This request updates the font style, size, and color of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-119">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-119">Response</span></span>
<span data-ttu-id="dfed4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": true,
    "color": "#4B180E",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-123">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-123">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-124">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-124">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-126">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-126">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="dfed4-127">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-127">Request</span></span>
<span data-ttu-id="dfed4-128">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="dfed4-128">This request updates the background color of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-129">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-129">Response</span></span>
<span data-ttu-id="dfed4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-134">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="dfed4-137">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-137">Request</span></span>
<span data-ttu-id="dfed4-138">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="dfed4-138">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-139">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-139">Response</span></span>
<span data-ttu-id="dfed4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Center",
    "rowHeight": 49,
    "verticalAlignment": "Center",
    "wrapText": false
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-144">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="dfed4-147">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-147">Request</span></span>
<span data-ttu-id="dfed4-148">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="dfed4-148">This request updates the font style and size of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-149">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-149">Response</span></span>
<span data-ttu-id="dfed4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#000000",
    "italic": true,
    "name": "Calibri",
    "size": 26,
    "underline": "None"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-154">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="dfed4-157">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-157">Request</span></span>
<span data-ttu-id="dfed4-158">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="dfed4-158">This request updates the background color of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-159">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-159">Response</span></span>
<span data-ttu-id="dfed4-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-163">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-164">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-166">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="dfed4-167">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-167">Request</span></span>
<span data-ttu-id="dfed4-168">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="dfed4-168">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-169">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-169">Response</span></span>
<span data-ttu-id="dfed4-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "columnWidth": 135,
    "horizontalAlignment": "Right",
    "rowHeight": 49,
    "verticalAlignment": "Top",
    "wrapText": false
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-173">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-174">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="dfed4-177">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-177">Request</span></span>
<span data-ttu-id="dfed4-178">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="dfed4-178">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="dfed4-179">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="dfed4-179">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-180">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-180">Response</span></span>
<span data-ttu-id="dfed4-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "bold": false,
    "color": "#FFFFFF",
    "italic": false,
    "name": "Calibri",
    "size": 26,
    "underline": "Single"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-184">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-184">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-185">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-185">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-187">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-187">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="dfed4-188">请求</span><span class="sxs-lookup"><span data-stu-id="dfed4-188">Request</span></span>
<span data-ttu-id="dfed4-189">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="dfed4-189">This request updates the background color of the third cell.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Sheet1"],
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="dfed4-190">响应</span><span class="sxs-lookup"><span data-stu-id="dfed4-190">Response</span></span>
<span data-ttu-id="dfed4-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfed4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfed4-194">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="dfed4-194">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfed4-195">C#</span><span class="sxs-lookup"><span data-stu-id="dfed4-195">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfed4-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="dfed4-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dfed4-197">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfed4-197">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="see-also"></a><span data-ttu-id="dfed4-198">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dfed4-198">See also</span></span>
* [<span data-ttu-id="dfed4-199">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="dfed4-199">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="dfed4-200">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="dfed4-200">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="dfed4-201">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="dfed4-201">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="dfed4-202">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="dfed4-202">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="dfed4-203">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="dfed4-203">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update a range format in Excel with Microsoft Graph",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/excel-update-range-format.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
