# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="d212c-101">通过 Microsoft Graph 更新 Excel 区域格式</span><span class="sxs-lookup"><span data-stu-id="d212c-101">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="d212c-102">以下示例演示如何更新指定区域的 [RangeFormat](../api-reference/v1.0/resources/rangeformat.md)、[RangeFill](../api-reference/v1.0/resources/rangefill.md) 和 [RangeFont](../api-reference/v1.0/resources/rangefont.md) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-102">The following examples demonstrate how to update properties of the [RangeFormat](../api-reference/v1.0/resources/rangeformat.md), [RangeFill](../api-reference/v1.0/resources/rangefill.md), and [RangeFont](../api-reference/v1.0/resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="d212c-103">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="d212c-103">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="d212c-105">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-105">Request</span></span>
<span data-ttu-id="d212c-106">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="d212c-106">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d212c-107">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-107">Response</span></span>
<span data-ttu-id="d212c-p101">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p101">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="d212c-111">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-111">Request</span></span>
<span data-ttu-id="d212c-112">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="d212c-112">This request updates the font style, size, and color of the first cell.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d212c-113">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-113">Response</span></span>
<span data-ttu-id="d212c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="d212c-117">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-117">Request</span></span>
<span data-ttu-id="d212c-118">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="d212c-118">This request updates the background color of the first cell.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="d212c-119">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-119">Response</span></span>
<span data-ttu-id="d212c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#FF0000"
}
```
##### <a name="request"></a><span data-ttu-id="d212c-123">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-123">Request</span></span>
<span data-ttu-id="d212c-124">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="d212c-124">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d212c-125">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-125">Response</span></span>
<span data-ttu-id="d212c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="d212c-129">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-129">Request</span></span>
<span data-ttu-id="d212c-130">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="d212c-130">This request updates the font style and size of the second cell.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d212c-131">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-131">Response</span></span>
<span data-ttu-id="d212c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="d212c-135">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-135">Request</span></span>
<span data-ttu-id="d212c-136">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="d212c-136">This request updates the background color of the second cell.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="d212c-137">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-137">Response</span></span>
<span data-ttu-id="d212c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#00FF00"
}
```

##### <a name="request"></a><span data-ttu-id="d212c-141">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-141">Request</span></span>
<span data-ttu-id="d212c-142">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="d212c-142">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d212c-143">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-143">Response</span></span>
<span data-ttu-id="d212c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFormat"
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

##### <a name="request"></a><span data-ttu-id="d212c-147">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-147">Request</span></span>
<span data-ttu-id="d212c-148">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="d212c-148">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="d212c-149">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="d212c-149">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
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
##### <a name="response"></a><span data-ttu-id="d212c-150">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-150">Response</span></span>
<span data-ttu-id="d212c-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFont"
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

##### <a name="request"></a><span data-ttu-id="d212c-154">请求</span><span class="sxs-lookup"><span data-stu-id="d212c-154">Request</span></span>
<span data-ttu-id="d212c-155">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="d212c-155">This request updates the background color of the third cell.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="d212c-156">响应</span><span class="sxs-lookup"><span data-stu-id="d212c-156">Response</span></span>
<span data-ttu-id="d212c-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d212c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "color": "#0000FF"
}
```


## <a name="see-also"></a><span data-ttu-id="d212c-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d212c-160">See also</span></span>
* [<span data-ttu-id="d212c-161">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="d212c-161">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="d212c-162">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="d212c-162">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="d212c-163">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="d212c-163">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="d212c-164">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="d212c-164">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="d212c-165">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="d212c-165">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)
