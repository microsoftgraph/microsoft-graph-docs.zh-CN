# <a name="update-rangeformat"></a><span data-ttu-id="71a37-101">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="71a37-101">Update rangeformat</span></span>

<span data-ttu-id="71a37-102">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-102">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="71a37-103">权限</span><span class="sxs-lookup"><span data-stu-id="71a37-103">Permissions</span></span>
<span data-ttu-id="71a37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="71a37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71a37-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="71a37-106">Permission type</span></span>      | <span data-ttu-id="71a37-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71a37-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71a37-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71a37-108">Delegated (work or school account)</span></span> | <span data-ttu-id="71a37-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71a37-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71a37-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71a37-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71a37-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="71a37-111">Not supported.</span></span>    |
|<span data-ttu-id="71a37-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="71a37-112">Application</span></span> | <span data-ttu-id="71a37-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="71a37-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71a37-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71a37-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="71a37-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="71a37-115">Request headers</span></span>
| <span data-ttu-id="71a37-116">名称</span><span class="sxs-lookup"><span data-stu-id="71a37-116">Name</span></span>       | <span data-ttu-id="71a37-117">说明</span><span class="sxs-lookup"><span data-stu-id="71a37-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="71a37-118">授权</span><span class="sxs-lookup"><span data-stu-id="71a37-118">Authorization</span></span>  | <span data-ttu-id="71a37-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71a37-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71a37-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71a37-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="71a37-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="71a37-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71a37-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="71a37-124">Request body</span></span>
<span data-ttu-id="71a37-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="71a37-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71a37-128">属性</span><span class="sxs-lookup"><span data-stu-id="71a37-128">Property</span></span>     | <span data-ttu-id="71a37-129">类型</span><span class="sxs-lookup"><span data-stu-id="71a37-129">Type</span></span>   |<span data-ttu-id="71a37-130">说明</span><span class="sxs-lookup"><span data-stu-id="71a37-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71a37-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="71a37-131">columnWidth</span></span>|<span data-ttu-id="71a37-132">double</span><span class="sxs-lookup"><span data-stu-id="71a37-132">double</span></span>|<span data-ttu-id="71a37-p105">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="71a37-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="71a37-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="71a37-135">horizontalAlignment</span></span>|<span data-ttu-id="71a37-136">string</span><span class="sxs-lookup"><span data-stu-id="71a37-136">string</span></span>|<span data-ttu-id="71a37-137">代表指定对象的水平对齐方式。</span><span class="sxs-lookup"><span data-stu-id="71a37-137">Returns or sets the horizontal alignment for the specified object.</span></span> <span data-ttu-id="71a37-138">可取值为：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="71a37-138">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="71a37-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="71a37-139">rowHeight</span></span>|<span data-ttu-id="71a37-140">double</span><span class="sxs-lookup"><span data-stu-id="71a37-140">double</span></span>|<span data-ttu-id="71a37-p107">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="71a37-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="71a37-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="71a37-143">verticalAlignment</span></span>|<span data-ttu-id="71a37-144">string</span><span class="sxs-lookup"><span data-stu-id="71a37-144">string</span></span>|<span data-ttu-id="71a37-145">代表指定对象的垂直对齐方式。</span><span class="sxs-lookup"><span data-stu-id="71a37-145">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="71a37-146">可取值为：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="71a37-146">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="71a37-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="71a37-147">wrapText</span></span>|<span data-ttu-id="71a37-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="71a37-148">boolean</span></span>|<span data-ttu-id="71a37-p109">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="71a37-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="71a37-151">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-151">Response</span></span>

<span data-ttu-id="71a37-152">如果成功，此方法在响应正文中返回`200 OK`响应代码和更新的 [WorkbookRangeFormat](../resources/rangeformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71a37-152">If successful, this method returns a `200 OK` response code and updated [plannerTaskDetails](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71a37-153">示例</span><span class="sxs-lookup"><span data-stu-id="71a37-153">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="71a37-154">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="71a37-154">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="71a37-155">以下示例演示如何更新指定区域的 [WorkbookRangeFormat](../resources/rangeformat.md)、[WorkbookRangeFill](../resources/rangefill.md) 和 [WorkbookRangeFont](../resources/rangefont.md) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-155">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="71a37-156">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="71a37-156">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="71a37-158">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-158">Request</span></span>
<span data-ttu-id="71a37-159">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="71a37-159">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="71a37-160">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-160">Response</span></span>
<span data-ttu-id="71a37-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="71a37-164">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-164">Request</span></span>
<span data-ttu-id="71a37-165">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="71a37-165">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="71a37-166">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-166">Response</span></span>
<span data-ttu-id="71a37-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="71a37-170">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-170">Request</span></span>
<span data-ttu-id="71a37-171">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="71a37-171">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="71a37-172">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-172">Response</span></span>
<span data-ttu-id="71a37-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="71a37-176">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-176">Request</span></span>
<span data-ttu-id="71a37-177">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="71a37-177">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="71a37-178">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-178">Response</span></span>
<span data-ttu-id="71a37-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="71a37-182">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-182">Request</span></span>
<span data-ttu-id="71a37-183">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="71a37-183">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="71a37-184">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-184">Response</span></span>
<span data-ttu-id="71a37-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="71a37-188">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-188">Request</span></span>
<span data-ttu-id="71a37-189">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="71a37-189">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="71a37-190">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-190">Response</span></span>
<span data-ttu-id="71a37-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="71a37-194">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-194">Request</span></span>
<span data-ttu-id="71a37-195">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="71a37-195">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="71a37-196">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-196">Response</span></span>
<span data-ttu-id="71a37-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="71a37-200">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-200">Request</span></span>
<span data-ttu-id="71a37-201">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="71a37-201">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="71a37-202">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="71a37-202">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="71a37-203">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-203">Response</span></span>
<span data-ttu-id="71a37-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="71a37-207">请求</span><span class="sxs-lookup"><span data-stu-id="71a37-207">Request</span></span>
<span data-ttu-id="71a37-208">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="71a37-208">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="71a37-209">响应</span><span class="sxs-lookup"><span data-stu-id="71a37-209">Response</span></span>
<span data-ttu-id="71a37-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71a37-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:
      Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ],
  "tocPath": ""
}-->