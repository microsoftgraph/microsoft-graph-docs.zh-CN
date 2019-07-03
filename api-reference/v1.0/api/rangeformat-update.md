---
title: 更新 RangeFormat
description: 更新 rangeformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c3e2554de8d3c600bff14034b49bd2254d5c0774
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459704"
---
# <a name="update-rangeformat"></a><span data-ttu-id="152ae-103">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="152ae-103">Update rangeformat</span></span>

<span data-ttu-id="152ae-104">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="152ae-105">权限</span><span class="sxs-lookup"><span data-stu-id="152ae-105">Permissions</span></span>
<span data-ttu-id="152ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="152ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="152ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="152ae-108">Permission type</span></span>      | <span data-ttu-id="152ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="152ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="152ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="152ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="152ae-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="152ae-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="152ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="152ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="152ae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="152ae-113">Not supported.</span></span>    |
|<span data-ttu-id="152ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="152ae-114">Application</span></span> | <span data-ttu-id="152ae-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="152ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="152ae-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="152ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="152ae-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="152ae-117">Request headers</span></span>
| <span data-ttu-id="152ae-118">名称</span><span class="sxs-lookup"><span data-stu-id="152ae-118">Name</span></span>       | <span data-ttu-id="152ae-119">说明</span><span class="sxs-lookup"><span data-stu-id="152ae-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="152ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="152ae-120">Authorization</span></span>  | <span data-ttu-id="152ae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="152ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="152ae-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="152ae-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="152ae-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="152ae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="152ae-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="152ae-126">Request body</span></span>
<span data-ttu-id="152ae-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="152ae-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="152ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="152ae-130">Property</span></span>     | <span data-ttu-id="152ae-131">类型</span><span class="sxs-lookup"><span data-stu-id="152ae-131">Type</span></span>   |<span data-ttu-id="152ae-132">说明</span><span class="sxs-lookup"><span data-stu-id="152ae-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="152ae-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="152ae-133">columnWidth</span></span>|<span data-ttu-id="152ae-134">double</span><span class="sxs-lookup"><span data-stu-id="152ae-134">double</span></span>|<span data-ttu-id="152ae-p105">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="152ae-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="152ae-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="152ae-137">horizontalAlignment</span></span>|<span data-ttu-id="152ae-138">string</span><span class="sxs-lookup"><span data-stu-id="152ae-138">string</span></span>|<span data-ttu-id="152ae-139">表示指定对象的水平对齐方式。</span><span class="sxs-lookup"><span data-stu-id="152ae-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="152ae-140">可能的值为: `General`、 `Left`、 `Center` `Right` `Fill` `Justify` `CenterAcrossSelection`、、、、 `Distributed`。</span><span class="sxs-lookup"><span data-stu-id="152ae-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="152ae-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="152ae-141">rowHeight</span></span>|<span data-ttu-id="152ae-142">double</span><span class="sxs-lookup"><span data-stu-id="152ae-142">double</span></span>|<span data-ttu-id="152ae-p107">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="152ae-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="152ae-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="152ae-145">verticalAlignment</span></span>|<span data-ttu-id="152ae-146">string</span><span class="sxs-lookup"><span data-stu-id="152ae-146">string</span></span>|<span data-ttu-id="152ae-147">表示指定对象的垂直对齐方式。</span><span class="sxs-lookup"><span data-stu-id="152ae-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="152ae-148">可能的值包括 `Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="152ae-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="152ae-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="152ae-149">wrapText</span></span>|<span data-ttu-id="152ae-150">boolean</span><span class="sxs-lookup"><span data-stu-id="152ae-150">boolean</span></span>|<span data-ttu-id="152ae-p109">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="152ae-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="152ae-153">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-153">Response</span></span>

<span data-ttu-id="152ae-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookRangeFormat](../resources/rangeformat.md)对象。</span><span class="sxs-lookup"><span data-stu-id="152ae-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="152ae-155">示例</span><span class="sxs-lookup"><span data-stu-id="152ae-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="152ae-156">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="152ae-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="152ae-157">下面的示例演示如何更新指定区域的[WorkbookRangeFormat](../resources/rangeformat.md)、 [WorkbookRangeFill](../resources/rangefill.md)和[WorkbookRangeFont](../resources/rangefont.md)属性的属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="152ae-158">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="152ae-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="152ae-160">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-160">Request</span></span>
<span data-ttu-id="152ae-161">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="152ae-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-162">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-162">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-163">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-166">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-166">Response</span></span>
<span data-ttu-id="152ae-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="152ae-170">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-170">Request</span></span>
<span data-ttu-id="152ae-171">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="152ae-171">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-172">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-172">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-173">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-175">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-176">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-176">Response</span></span>
<span data-ttu-id="152ae-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="152ae-180">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-180">Request</span></span>
<span data-ttu-id="152ae-181">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="152ae-181">This request updates the background color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-182">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-182">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-183">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-184">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-185">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-186">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-186">Response</span></span>
<span data-ttu-id="152ae-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="152ae-190">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-190">Request</span></span>
<span data-ttu-id="152ae-191">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="152ae-191">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-192">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-192">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-193">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-194">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-194">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-195">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-196">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-196">Response</span></span>
<span data-ttu-id="152ae-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="152ae-200">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-200">Request</span></span>
<span data-ttu-id="152ae-201">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="152ae-201">This request updates the font style and size of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-202">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-202">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-203">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-203">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-204">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-204">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-205">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-205">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-206">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-206">Response</span></span>
<span data-ttu-id="152ae-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="152ae-210">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-210">Request</span></span>
<span data-ttu-id="152ae-211">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="152ae-211">This request updates the background color of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-212">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-212">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-213">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-214">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-214">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-215">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-216">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-216">Response</span></span>
<span data-ttu-id="152ae-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="152ae-220">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-220">Request</span></span>
<span data-ttu-id="152ae-221">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="152ae-221">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-222">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-222">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-223">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-223">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-224">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-224">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-225">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-225">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-226">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-226">Response</span></span>
<span data-ttu-id="152ae-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="152ae-230">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-230">Request</span></span>
<span data-ttu-id="152ae-231">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="152ae-231">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="152ae-232">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="152ae-232">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-233">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-233">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-234">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-235">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-235">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-236">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-236">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-237">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-237">Response</span></span>
<span data-ttu-id="152ae-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="152ae-241">请求</span><span class="sxs-lookup"><span data-stu-id="152ae-241">Request</span></span>
<span data-ttu-id="152ae-242">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="152ae-242">This request updates the background color of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="152ae-243">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="152ae-243">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="152ae-244">C#</span><span class="sxs-lookup"><span data-stu-id="152ae-244">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152ae-245">Javascript</span><span class="sxs-lookup"><span data-stu-id="152ae-245">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152ae-246">目标-C</span><span class="sxs-lookup"><span data-stu-id="152ae-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152ae-247">响应</span><span class="sxs-lookup"><span data-stu-id="152ae-247">Response</span></span>
<span data-ttu-id="152ae-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="152ae-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
