---
title: 更新 RangeFormat
description: 更新 rangeformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 07c39392c9e19e0ce94d664ee61f89831534ce11
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324751"
---
# <a name="update-rangeformat"></a><span data-ttu-id="77a1d-103">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="77a1d-103">Update rangeformat</span></span>

<span data-ttu-id="77a1d-104">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-104">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="77a1d-105">权限</span><span class="sxs-lookup"><span data-stu-id="77a1d-105">Permissions</span></span>
<span data-ttu-id="77a1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77a1d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77a1d-108">Permission type</span></span>      | <span data-ttu-id="77a1d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77a1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77a1d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77a1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77a1d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77a1d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77a1d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77a1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77a1d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="77a1d-113">Not supported.</span></span>    |
|<span data-ttu-id="77a1d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77a1d-114">Application</span></span> | <span data-ttu-id="77a1d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77a1d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77a1d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="request-headers"></a><span data-ttu-id="77a1d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="77a1d-117">Request headers</span></span>
| <span data-ttu-id="77a1d-118">名称</span><span class="sxs-lookup"><span data-stu-id="77a1d-118">Name</span></span>       | <span data-ttu-id="77a1d-119">说明</span><span class="sxs-lookup"><span data-stu-id="77a1d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="77a1d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77a1d-120">Authorization</span></span>  | <span data-ttu-id="77a1d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77a1d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="77a1d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="77a1d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77a1d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="77a1d-126">Request body</span></span>
<span data-ttu-id="77a1d-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="77a1d-130">属性</span><span class="sxs-lookup"><span data-stu-id="77a1d-130">Property</span></span>     | <span data-ttu-id="77a1d-131">类型</span><span class="sxs-lookup"><span data-stu-id="77a1d-131">Type</span></span>   |<span data-ttu-id="77a1d-132">说明</span><span class="sxs-lookup"><span data-stu-id="77a1d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77a1d-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="77a1d-133">columnWidth</span></span>|<span data-ttu-id="77a1d-134">double</span><span class="sxs-lookup"><span data-stu-id="77a1d-134">double</span></span>|<span data-ttu-id="77a1d-p105">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="77a1d-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="77a1d-137">horizontalAlignment</span></span>|<span data-ttu-id="77a1d-138">string</span><span class="sxs-lookup"><span data-stu-id="77a1d-138">string</span></span>|<span data-ttu-id="77a1d-139">表示指定对象的水平对齐方式。</span><span class="sxs-lookup"><span data-stu-id="77a1d-139">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="77a1d-140">可能的值为: `General`、 `Left`、 `Center` `Right` `Fill` `Justify` `CenterAcrossSelection`、、、、 `Distributed`。</span><span class="sxs-lookup"><span data-stu-id="77a1d-140">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="77a1d-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="77a1d-141">rowHeight</span></span>|<span data-ttu-id="77a1d-142">double</span><span class="sxs-lookup"><span data-stu-id="77a1d-142">double</span></span>|<span data-ttu-id="77a1d-p107">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="77a1d-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="77a1d-145">verticalAlignment</span></span>|<span data-ttu-id="77a1d-146">string</span><span class="sxs-lookup"><span data-stu-id="77a1d-146">string</span></span>|<span data-ttu-id="77a1d-147">表示指定对象的垂直对齐方式。</span><span class="sxs-lookup"><span data-stu-id="77a1d-147">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="77a1d-148">可能的值包括 `Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="77a1d-148">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="77a1d-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="77a1d-149">wrapText</span></span>|<span data-ttu-id="77a1d-150">boolean</span><span class="sxs-lookup"><span data-stu-id="77a1d-150">boolean</span></span>|<span data-ttu-id="77a1d-p109">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="77a1d-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="77a1d-153">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-153">Response</span></span>

<span data-ttu-id="77a1d-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookRangeFormat](../resources/rangeformat.md)对象。</span><span class="sxs-lookup"><span data-stu-id="77a1d-154">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeFormat](../resources/rangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77a1d-155">示例</span><span class="sxs-lookup"><span data-stu-id="77a1d-155">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="77a1d-156">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="77a1d-156">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="77a1d-157">下面的示例演示如何更新指定区域的[WorkbookRangeFormat](../resources/rangeformat.md)、 [WorkbookRangeFill](../resources/rangefill.md)和[WorkbookRangeFont](../resources/rangefont.md)属性的属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-157">The following examples demonstrate how to update properties of the [WorkbookRangeFormat](../resources/rangeformat.md), [WorkbookRangeFill](../resources/rangefill.md), and [WorkbookRangeFont](../resources/rangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="77a1d-158">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="77a1d-158">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="77a1d-160">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-160">Request</span></span>
<span data-ttu-id="77a1d-161">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="77a1d-161">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-162">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-162">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-163">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-166">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-167">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-167">Response</span></span>
<span data-ttu-id="77a1d-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="77a1d-171">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-171">Request</span></span>
<span data-ttu-id="77a1d-172">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="77a1d-172">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-173">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-173">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-174">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-177">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-178">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-178">Response</span></span>
<span data-ttu-id="77a1d-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="77a1d-182">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-182">Request</span></span>
<span data-ttu-id="77a1d-183">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="77a1d-183">This request updates the background color of the first cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-184">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-184">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-185">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-187">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-188">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-189">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-189">Response</span></span>
<span data-ttu-id="77a1d-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="77a1d-193">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-193">Request</span></span>
<span data-ttu-id="77a1d-194">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="77a1d-194">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-195">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-195">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-196">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-198">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-199">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-200">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-200">Response</span></span>
<span data-ttu-id="77a1d-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="77a1d-204">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-204">Request</span></span>
<span data-ttu-id="77a1d-205">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="77a1d-205">This request updates the font style and size of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-206">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-206">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-207">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-209">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-210">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-211">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-211">Response</span></span>
<span data-ttu-id="77a1d-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="77a1d-215">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-215">Request</span></span>
<span data-ttu-id="77a1d-216">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="77a1d-216">This request updates the background color of the second cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-217">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-217">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-218">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-220">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-221">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-222">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-222">Response</span></span>
<span data-ttu-id="77a1d-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="77a1d-226">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-226">Request</span></span>
<span data-ttu-id="77a1d-227">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="77a1d-227">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-228">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-228">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-229">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-231">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-232">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-233">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-233">Response</span></span>
<span data-ttu-id="77a1d-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="77a1d-237">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-237">Request</span></span>
<span data-ttu-id="77a1d-238">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="77a1d-238">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="77a1d-239">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="77a1d-239">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-240">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-240">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-241">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-241">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-242">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-242">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-243">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-243">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-244">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-244">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-245">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-245">Response</span></span>
<span data-ttu-id="77a1d-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="77a1d-249">请求</span><span class="sxs-lookup"><span data-stu-id="77a1d-249">Request</span></span>
<span data-ttu-id="77a1d-250">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="77a1d-250">This request updates the background color of the third cell.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="77a1d-251">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="77a1d-251">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="77a1d-252">C#</span><span class="sxs-lookup"><span data-stu-id="77a1d-252">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77a1d-253">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77a1d-253">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77a1d-254">目标-C</span><span class="sxs-lookup"><span data-stu-id="77a1d-254">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77a1d-255">Java</span><span class="sxs-lookup"><span data-stu-id="77a1d-255">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77a1d-256">响应</span><span class="sxs-lookup"><span data-stu-id="77a1d-256">Response</span></span>
<span data-ttu-id="77a1d-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77a1d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
