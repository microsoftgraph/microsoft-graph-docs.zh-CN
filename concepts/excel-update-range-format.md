---
title: 通过 Microsoft Graph 更新 Excel 区域格式
description: 下面的几个示例展示了如何更新指定区域的 RangeFormat、RangeFill 和 RangeFont 属性。
ms.openlocfilehash: 17c8a8cc8e20887329ff79b4983f69e25d1e2dee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091772"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="3b668-103">使用 Microsoft Graph 更新 Excel 中的区域格式</span><span class="sxs-lookup"><span data-stu-id="3b668-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="3b668-104">以下示例演示如何更新指定区域的 [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0)、[RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0) 和 [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="3b668-105">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="3b668-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="3b668-107">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-107">Request</span></span>
<span data-ttu-id="3b668-108">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="3b668-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-109">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-109">Response</span></span>
<span data-ttu-id="3b668-p101">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="3b668-113">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-113">Request</span></span>
<span data-ttu-id="3b668-114">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="3b668-114">This request updates the font style, size, and color of the first cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-115">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-115">Response</span></span>
<span data-ttu-id="3b668-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="3b668-119">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-119">Request</span></span>
<span data-ttu-id="3b668-120">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="3b668-120">This request updates the background color of the first cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-121">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-121">Response</span></span>
<span data-ttu-id="3b668-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="3b668-125">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-125">Request</span></span>
<span data-ttu-id="3b668-126">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="3b668-126">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-127">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-127">Response</span></span>
<span data-ttu-id="3b668-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="3b668-131">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-131">Request</span></span>
<span data-ttu-id="3b668-132">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="3b668-132">This request updates the font style and size of the second cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-133">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-133">Response</span></span>
<span data-ttu-id="3b668-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="3b668-137">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-137">Request</span></span>
<span data-ttu-id="3b668-138">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="3b668-138">This request updates the background color of the second cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-139">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-139">Response</span></span>
<span data-ttu-id="3b668-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="3b668-143">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-143">Request</span></span>
<span data-ttu-id="3b668-144">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="3b668-144">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-145">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-145">Response</span></span>
<span data-ttu-id="3b668-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="3b668-149">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-149">Request</span></span>
<span data-ttu-id="3b668-150">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="3b668-150">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="3b668-151">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="3b668-151">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-152">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-152">Response</span></span>
<span data-ttu-id="3b668-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="3b668-156">请求</span><span class="sxs-lookup"><span data-stu-id="3b668-156">Request</span></span>
<span data-ttu-id="3b668-157">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="3b668-157">This request updates the background color of the third cell.</span></span>

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
##### <a name="response"></a><span data-ttu-id="3b668-158">响应</span><span class="sxs-lookup"><span data-stu-id="3b668-158">Response</span></span>
<span data-ttu-id="3b668-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b668-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="3b668-162">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3b668-162">See also</span></span>
* [<span data-ttu-id="3b668-163">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="3b668-163">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="3b668-164">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="3b668-164">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="3b668-165">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="3b668-165">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="3b668-166">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="3b668-166">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="3b668-167">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="3b668-167">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
