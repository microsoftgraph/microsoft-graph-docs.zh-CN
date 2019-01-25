---
title: 更新 RangeFormat
description: 更新 rangeformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2bd576fcb30facd220e9abf7a8a1fee8d22f80a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524490"
---
# <a name="update-rangeformat"></a><span data-ttu-id="43132-103">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="43132-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43132-104">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="43132-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="43132-105">权限</span><span class="sxs-lookup"><span data-stu-id="43132-105">Permissions</span></span>
<span data-ttu-id="43132-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43132-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="43132-108">Permission type</span></span>      | <span data-ttu-id="43132-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43132-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43132-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43132-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43132-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43132-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="43132-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43132-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43132-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43132-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="43132-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="43132-114">Application</span></span> | <span data-ttu-id="43132-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="43132-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43132-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43132-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="43132-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="43132-117">Optional request headers</span></span>
| <span data-ttu-id="43132-118">名称</span><span class="sxs-lookup"><span data-stu-id="43132-118">Name</span></span>       | <span data-ttu-id="43132-119">说明</span><span class="sxs-lookup"><span data-stu-id="43132-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="43132-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="43132-120">Authorization</span></span>  | <span data-ttu-id="43132-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43132-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43132-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="43132-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="43132-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="43132-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43132-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="43132-126">Request body</span></span>
<span data-ttu-id="43132-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="43132-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="43132-130">属性</span><span class="sxs-lookup"><span data-stu-id="43132-130">Property</span></span>     | <span data-ttu-id="43132-131">类型</span><span class="sxs-lookup"><span data-stu-id="43132-131">Type</span></span>   |<span data-ttu-id="43132-132">说明</span><span class="sxs-lookup"><span data-stu-id="43132-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43132-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="43132-133">columnWidth</span></span>|<span data-ttu-id="43132-134">double</span><span class="sxs-lookup"><span data-stu-id="43132-134">double</span></span>|<span data-ttu-id="43132-p105">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="43132-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="43132-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="43132-137">horizontalAlignment</span></span>|<span data-ttu-id="43132-138">string</span><span class="sxs-lookup"><span data-stu-id="43132-138">string</span></span>|<span data-ttu-id="43132-p106">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="43132-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="43132-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="43132-141">rowHeight</span></span>|<span data-ttu-id="43132-142">double</span><span class="sxs-lookup"><span data-stu-id="43132-142">double</span></span>|<span data-ttu-id="43132-p107">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="43132-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="43132-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="43132-145">verticalAlignment</span></span>|<span data-ttu-id="43132-146">string</span><span class="sxs-lookup"><span data-stu-id="43132-146">string</span></span>|<span data-ttu-id="43132-p108">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="43132-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="43132-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="43132-149">wrapText</span></span>|<span data-ttu-id="43132-150">布尔</span><span class="sxs-lookup"><span data-stu-id="43132-150">boolean</span></span>|<span data-ttu-id="43132-p109">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="43132-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="43132-153">响应</span><span class="sxs-lookup"><span data-stu-id="43132-153">Response</span></span>

<span data-ttu-id="43132-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [RangeFormat](../resources/rangeformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43132-154">If successful, this method returns a `200 OK` response code and updated [RangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43132-155">示例</span><span class="sxs-lookup"><span data-stu-id="43132-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="43132-156">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="43132-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="43132-157">以下示例演示如何更新指定区域的 [RangeFormat](../resources/rangeformat.md)、[RangeFill](../resources/rangefill.md) 和 [RangeFont](../resources/rangefont.md) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="43132-157">The following examples demonstrate how to update properties of the [RangeFormat](../resources/rangeformat.md), [RangeFill](../resources/rangefill.md), and [RangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="43132-158">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="43132-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="43132-160">请求</span><span class="sxs-lookup"><span data-stu-id="43132-160">Request</span></span>
<span data-ttu-id="43132-161">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="43132-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-162">响应</span><span class="sxs-lookup"><span data-stu-id="43132-162">Response</span></span>
<span data-ttu-id="43132-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="43132-166">请求</span><span class="sxs-lookup"><span data-stu-id="43132-166">Request</span></span>
<span data-ttu-id="43132-167">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="43132-167">This request updates the font style, size, and color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-168">响应</span><span class="sxs-lookup"><span data-stu-id="43132-168">Response</span></span>
<span data-ttu-id="43132-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="43132-172">请求</span><span class="sxs-lookup"><span data-stu-id="43132-172">Request</span></span>
<span data-ttu-id="43132-173">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="43132-173">This request updates the background color of the first cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-174">响应</span><span class="sxs-lookup"><span data-stu-id="43132-174">Response</span></span>
<span data-ttu-id="43132-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="43132-178">请求</span><span class="sxs-lookup"><span data-stu-id="43132-178">Request</span></span>
<span data-ttu-id="43132-179">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="43132-179">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-180">响应</span><span class="sxs-lookup"><span data-stu-id="43132-180">Response</span></span>
<span data-ttu-id="43132-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="43132-184">请求</span><span class="sxs-lookup"><span data-stu-id="43132-184">Request</span></span>
<span data-ttu-id="43132-185">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="43132-185">This request updates the font style and size of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-186">响应</span><span class="sxs-lookup"><span data-stu-id="43132-186">Response</span></span>
<span data-ttu-id="43132-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="43132-190">请求</span><span class="sxs-lookup"><span data-stu-id="43132-190">Request</span></span>
<span data-ttu-id="43132-191">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="43132-191">This request updates the background color of the second cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-192">响应</span><span class="sxs-lookup"><span data-stu-id="43132-192">Response</span></span>
<span data-ttu-id="43132-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="43132-196">请求</span><span class="sxs-lookup"><span data-stu-id="43132-196">Request</span></span>
<span data-ttu-id="43132-197">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="43132-197">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-198">响应</span><span class="sxs-lookup"><span data-stu-id="43132-198">Response</span></span>
<span data-ttu-id="43132-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="43132-202">请求</span><span class="sxs-lookup"><span data-stu-id="43132-202">Request</span></span>
<span data-ttu-id="43132-203">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="43132-203">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="43132-204">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="43132-204">Note that the underline property takes **Single** or **Double** as values.</span></span>

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
##### <a name="response"></a><span data-ttu-id="43132-205">响应</span><span class="sxs-lookup"><span data-stu-id="43132-205">Response</span></span>
<span data-ttu-id="43132-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="43132-209">请求</span><span class="sxs-lookup"><span data-stu-id="43132-209">Request</span></span>
<span data-ttu-id="43132-210">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="43132-210">This request updates the background color of the third cell.</span></span> 

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
##### <a name="response"></a><span data-ttu-id="43132-211">响应</span><span class="sxs-lookup"><span data-stu-id="43132-211">Response</span></span>
<span data-ttu-id="43132-p119">下面是一个响应示例。注意：为简洁起见，可能会截断此处展示的响应对象。实际调用会返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43132-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
