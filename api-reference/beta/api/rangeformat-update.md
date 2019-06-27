---
title: 更新 RangeFormat
description: 更新 rangeformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7be6aee49e177501554c124e3a3bd7c4618392c0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268006"
---
# <a name="update-rangeformat"></a><span data-ttu-id="5bfe7-103">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="5bfe7-103">Update rangeformat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bfe7-104">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5bfe7-105">权限</span><span class="sxs-lookup"><span data-stu-id="5bfe7-105">Permissions</span></span>
<span data-ttu-id="5bfe7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bfe7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bfe7-108">Permission type</span></span>      | <span data-ttu-id="5bfe7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bfe7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bfe7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bfe7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5bfe7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bfe7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5bfe7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bfe7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bfe7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5bfe7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5bfe7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bfe7-114">Application</span></span> | <span data-ttu-id="5bfe7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bfe7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="5bfe7-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="5bfe7-117">Optional request headers</span></span>
| <span data-ttu-id="5bfe7-118">名称</span><span class="sxs-lookup"><span data-stu-id="5bfe7-118">Name</span></span>       | <span data-ttu-id="5bfe7-119">说明</span><span class="sxs-lookup"><span data-stu-id="5bfe7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5bfe7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bfe7-120">Authorization</span></span>  | <span data-ttu-id="5bfe7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5bfe7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5bfe7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5bfe7-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bfe7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bfe7-126">Request body</span></span>
<span data-ttu-id="5bfe7-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5bfe7-130">属性</span><span class="sxs-lookup"><span data-stu-id="5bfe7-130">Property</span></span>     | <span data-ttu-id="5bfe7-131">类型</span><span class="sxs-lookup"><span data-stu-id="5bfe7-131">Type</span></span>   |<span data-ttu-id="5bfe7-132">说明</span><span class="sxs-lookup"><span data-stu-id="5bfe7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bfe7-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="5bfe7-133">columnWidth</span></span>|<span data-ttu-id="5bfe7-134">double</span><span class="sxs-lookup"><span data-stu-id="5bfe7-134">double</span></span>|<span data-ttu-id="5bfe7-p105">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="5bfe7-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="5bfe7-137">horizontalAlignment</span></span>|<span data-ttu-id="5bfe7-138">string</span><span class="sxs-lookup"><span data-stu-id="5bfe7-138">string</span></span>|<span data-ttu-id="5bfe7-p106">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="5bfe7-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="5bfe7-141">rowHeight</span></span>|<span data-ttu-id="5bfe7-142">double</span><span class="sxs-lookup"><span data-stu-id="5bfe7-142">double</span></span>|<span data-ttu-id="5bfe7-p107">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="5bfe7-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="5bfe7-145">verticalAlignment</span></span>|<span data-ttu-id="5bfe7-146">string</span><span class="sxs-lookup"><span data-stu-id="5bfe7-146">string</span></span>|<span data-ttu-id="5bfe7-p108">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="5bfe7-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="5bfe7-149">wrapText</span></span>|<span data-ttu-id="5bfe7-150">boolean</span><span class="sxs-lookup"><span data-stu-id="5bfe7-150">boolean</span></span>|<span data-ttu-id="5bfe7-p109">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="5bfe7-153">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-153">Response</span></span>

<span data-ttu-id="5bfe7-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookRangeFormat](../resources/workbookrangeformat.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-154">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5bfe7-155">示例</span><span class="sxs-lookup"><span data-stu-id="5bfe7-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="5bfe7-156">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="5bfe7-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="5bfe7-157">下面的示例演示如何更新指定区域的[workbookRangeFormat](../resources/workbookrangeformat.md)、 [workbookRangeFill](../resources/workbookrangefill.md)和[workbookRangeFont](../resources/workbookrangefont.md)属性的属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-157">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="5bfe7-158">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="5bfe7-160">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-160">Request</span></span>
<span data-ttu-id="5bfe7-161">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-162">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-162">Response</span></span>
<span data-ttu-id="5bfe7-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-166">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-167">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-168">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-169">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-169">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="5bfe7-170">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-170">Request</span></span>
<span data-ttu-id="5bfe7-171">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-171">This request updates the font style, size, and color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font
Content-type: application/json

{
  "bold": true,
  "color": "#4B180E",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-172">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-172">Response</span></span>
<span data-ttu-id="5bfe7-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-176">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-177">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-178">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-179">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-179">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="5bfe7-180">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-180">Request</span></span>
<span data-ttu-id="5bfe7-181">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-181">This request updates the background color of the first cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill
Content-type: application/json

{
  "color": "#FF0000"
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-182">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-182">Response</span></span>
<span data-ttu-id="5bfe7-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-186">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-187">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-188">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-189">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-189">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="5bfe7-190">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-190">Request</span></span>
<span data-ttu-id="5bfe7-191">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-191">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Center",
  "verticalAlignment": "Center",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-192">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-192">Response</span></span>
<span data-ttu-id="5bfe7-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-196">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-196">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-197">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-197">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-198">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-198">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-199">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-199">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="5bfe7-200">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-200">Request</span></span>
<span data-ttu-id="5bfe7-201">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-201">This request updates the font style and size of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font
Content-type: application/json

{
  "italic": true,
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-202">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-202">Response</span></span>
<span data-ttu-id="5bfe7-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-206">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-206">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-207">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-207">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-208">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-209">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-209">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="5bfe7-210">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-210">Request</span></span>
<span data-ttu-id="5bfe7-211">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-211">This request updates the background color of the second cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_two"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill
Content-type: application/json

{
  "color": "#00FF00"
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-212">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-212">Response</span></span>
<span data-ttu-id="5bfe7-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-216">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-216">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-217">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-217">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-218">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-218">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-219">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-219">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_two-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="5bfe7-220">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-220">Request</span></span>
<span data-ttu-id="5bfe7-221">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-221">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format
Content-type: application/json

{
  "columnWidth": 135,
  "horizontalAlignment": "Right",
  "verticalAlignment": "Top",
  "rowHeight": 49,
  "wrapText": false
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-222">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-222">Response</span></span>
<span data-ttu-id="5bfe7-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-226">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-226">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-227">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-227">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-228">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-228">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-229">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-229">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="5bfe7-230">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-230">Request</span></span>
<span data-ttu-id="5bfe7-231">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-231">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="5bfe7-232">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-232">Note that the underline property takes **Single** or **Double** as values.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_font_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font
Content-type: application/json

{
  "underline": "Single",
  "color": "#FFFFFF",
  "size": 26
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-233">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-233">Response</span></span>
<span data-ttu-id="5bfe7-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-237">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-237">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-238">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-238">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-239">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-239">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-240">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-240">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_font_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request"></a><span data-ttu-id="5bfe7-241">请求</span><span class="sxs-lookup"><span data-stu-id="5bfe7-241">Request</span></span>
<span data-ttu-id="5bfe7-242">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-242">This request updates the background color of the third cell.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_rangeformat_fill_three"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill
Content-type: application/json

{
  "color": "#0000FF"
}
```
##### <a name="response"></a><span data-ttu-id="5bfe7-243">响应</span><span class="sxs-lookup"><span data-stu-id="5bfe7-243">Response</span></span>
<span data-ttu-id="5bfe7-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bfe7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5bfe7-247">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5bfe7-247">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5bfe7-248">C#</span><span class="sxs-lookup"><span data-stu-id="5bfe7-248">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bfe7-249">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bfe7-249">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5bfe7-250">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bfe7-250">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_rangeformat_fill_three-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


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
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/rangeformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: update_rangeformat_font_three/underline:\r\n       Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ]
}
-->
