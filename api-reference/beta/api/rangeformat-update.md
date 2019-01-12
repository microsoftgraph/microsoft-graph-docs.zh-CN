---
title: 更新 RangeFormat
description: 更新 rangeformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a6b005ad0ffd5d8cdb59328e464fadbbff384e09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969084"
---
# <a name="update-rangeformat"></a><span data-ttu-id="c1fa4-103">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="c1fa4-103">Update rangeformat</span></span>

> <span data-ttu-id="c1fa4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1fa4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1fa4-106">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-106">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c1fa4-107">权限</span><span class="sxs-lookup"><span data-stu-id="c1fa4-107">Permissions</span></span>
<span data-ttu-id="c1fa4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1fa4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1fa4-110">Permission type</span></span>      | <span data-ttu-id="c1fa4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1fa4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1fa4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1fa4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1fa4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1fa4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1fa4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1fa4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1fa4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1fa4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c1fa4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1fa4-116">Application</span></span> | <span data-ttu-id="c1fa4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1fa4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="c1fa4-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c1fa4-119">Optional request headers</span></span>
| <span data-ttu-id="c1fa4-120">名称</span><span class="sxs-lookup"><span data-stu-id="c1fa4-120">Name</span></span>       | <span data-ttu-id="c1fa4-121">说明</span><span class="sxs-lookup"><span data-stu-id="c1fa4-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c1fa4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1fa4-122">Authorization</span></span>  | <span data-ttu-id="c1fa4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1fa4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c1fa4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c1fa4-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1fa4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1fa4-128">Request body</span></span>
<span data-ttu-id="c1fa4-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c1fa4-132">属性</span><span class="sxs-lookup"><span data-stu-id="c1fa4-132">Property</span></span>     | <span data-ttu-id="c1fa4-133">类型</span><span class="sxs-lookup"><span data-stu-id="c1fa4-133">Type</span></span>   |<span data-ttu-id="c1fa4-134">说明</span><span class="sxs-lookup"><span data-stu-id="c1fa4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1fa4-135">columnWidth</span><span class="sxs-lookup"><span data-stu-id="c1fa4-135">columnWidth</span></span>|<span data-ttu-id="c1fa4-136">double</span><span class="sxs-lookup"><span data-stu-id="c1fa4-136">double</span></span>|<span data-ttu-id="c1fa4-p106">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p106">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="c1fa4-139">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="c1fa4-139">horizontalAlignment</span></span>|<span data-ttu-id="c1fa4-140">string</span><span class="sxs-lookup"><span data-stu-id="c1fa4-140">string</span></span>|<span data-ttu-id="c1fa4-p107">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p107">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="c1fa4-143">rowHeight</span><span class="sxs-lookup"><span data-stu-id="c1fa4-143">rowHeight</span></span>|<span data-ttu-id="c1fa4-144">double</span><span class="sxs-lookup"><span data-stu-id="c1fa4-144">double</span></span>|<span data-ttu-id="c1fa4-p108">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p108">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="c1fa4-147">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="c1fa4-147">verticalAlignment</span></span>|<span data-ttu-id="c1fa4-148">string</span><span class="sxs-lookup"><span data-stu-id="c1fa4-148">string</span></span>|<span data-ttu-id="c1fa4-p109">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p109">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="c1fa4-151">wrapText</span><span class="sxs-lookup"><span data-stu-id="c1fa4-151">wrapText</span></span>|<span data-ttu-id="c1fa4-152">boolean</span><span class="sxs-lookup"><span data-stu-id="c1fa4-152">boolean</span></span>|<span data-ttu-id="c1fa4-p110">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p110">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="c1fa4-155">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-155">Response</span></span>

<span data-ttu-id="c1fa4-156">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [RangeFormat](../resources/rangeformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-156">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1fa4-157">示例</span><span class="sxs-lookup"><span data-stu-id="c1fa4-157">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="c1fa4-158">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="c1fa4-158">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="c1fa4-159">以下示例演示如何更新指定区域的 [RangeFormat](../resources/rangeformat.md)、[RangeFill](../resources/rangefill.md) 和 [RangeFont](../resources/rangefont.md) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-159">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="c1fa4-160">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-160">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="c1fa4-162">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-162">Request</span></span>
<span data-ttu-id="c1fa4-163">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-163">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-164">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-164">Response</span></span>
<span data-ttu-id="c1fa4-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c1fa4-168">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-168">Request</span></span>
<span data-ttu-id="c1fa4-169">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-169">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-170">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-170">Response</span></span>
<span data-ttu-id="c1fa4-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c1fa4-174">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-174">Request</span></span>
<span data-ttu-id="c1fa4-175">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-175">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-176">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-176">Response</span></span>
<span data-ttu-id="c1fa4-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="c1fa4-180">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-180">Request</span></span>
<span data-ttu-id="c1fa4-181">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-181">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-182">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-182">Response</span></span>
<span data-ttu-id="c1fa4-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c1fa4-186">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-186">Request</span></span>
<span data-ttu-id="c1fa4-187">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-187">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-188">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-188">Response</span></span>
<span data-ttu-id="c1fa4-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c1fa4-192">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-192">Request</span></span>
<span data-ttu-id="c1fa4-193">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-193">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-194">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-194">Response</span></span>
<span data-ttu-id="c1fa4-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c1fa4-198">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-198">Request</span></span>
<span data-ttu-id="c1fa4-199">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-199">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-200">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-200">Response</span></span>
<span data-ttu-id="c1fa4-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c1fa4-204">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-204">Request</span></span>
<span data-ttu-id="c1fa4-205">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-205">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="c1fa4-206">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-206">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="c1fa4-207">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-207">Response</span></span>
<span data-ttu-id="c1fa4-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="c1fa4-211">请求</span><span class="sxs-lookup"><span data-stu-id="c1fa4-211">Request</span></span>
<span data-ttu-id="c1fa4-212">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-212">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="c1fa4-213">响应</span><span class="sxs-lookup"><span data-stu-id="c1fa4-213">Response</span></span>
<span data-ttu-id="c1fa4-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1fa4-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
