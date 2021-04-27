---
title: 更新 RangeFormat
description: 更新 rangeformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: e91791f155f3e53f6fd565239fcbcb02ad254b47
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051023"
---
# <a name="update-rangeformat"></a><span data-ttu-id="0b500-103">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="0b500-103">Update rangeformat</span></span>

<span data-ttu-id="0b500-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b500-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b500-105">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b500-105">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0b500-106">权限</span><span class="sxs-lookup"><span data-stu-id="0b500-106">Permissions</span></span>
<span data-ttu-id="0b500-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b500-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b500-109">Permission type</span></span>      | <span data-ttu-id="0b500-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b500-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b500-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b500-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b500-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b500-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b500-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b500-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b500-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b500-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0b500-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b500-115">Application</span></span> | <span data-ttu-id="0b500-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b500-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b500-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b500-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/names/{name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/names/{name}/range/format
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/format
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="0b500-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0b500-118">Optional request headers</span></span>
| <span data-ttu-id="0b500-119">名称</span><span class="sxs-lookup"><span data-stu-id="0b500-119">Name</span></span>       | <span data-ttu-id="0b500-120">说明</span><span class="sxs-lookup"><span data-stu-id="0b500-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0b500-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b500-121">Authorization</span></span>  | <span data-ttu-id="0b500-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b500-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b500-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0b500-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0b500-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0b500-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b500-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b500-127">Request body</span></span>
<span data-ttu-id="0b500-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0b500-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b500-131">属性</span><span class="sxs-lookup"><span data-stu-id="0b500-131">Property</span></span>     | <span data-ttu-id="0b500-132">类型</span><span class="sxs-lookup"><span data-stu-id="0b500-132">Type</span></span>   |<span data-ttu-id="0b500-133">说明</span><span class="sxs-lookup"><span data-stu-id="0b500-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b500-134">columnWidth</span><span class="sxs-lookup"><span data-stu-id="0b500-134">columnWidth</span></span>|<span data-ttu-id="0b500-135">double</span><span class="sxs-lookup"><span data-stu-id="0b500-135">double</span></span>|<span data-ttu-id="0b500-p105">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="0b500-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="0b500-138">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="0b500-138">horizontalAlignment</span></span>|<span data-ttu-id="0b500-139">string</span><span class="sxs-lookup"><span data-stu-id="0b500-139">string</span></span>|<span data-ttu-id="0b500-p106">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="0b500-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="0b500-142">rowHeight</span><span class="sxs-lookup"><span data-stu-id="0b500-142">rowHeight</span></span>|<span data-ttu-id="0b500-143">double</span><span class="sxs-lookup"><span data-stu-id="0b500-143">double</span></span>|<span data-ttu-id="0b500-p107">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="0b500-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="0b500-146">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="0b500-146">verticalAlignment</span></span>|<span data-ttu-id="0b500-147">string</span><span class="sxs-lookup"><span data-stu-id="0b500-147">string</span></span>|<span data-ttu-id="0b500-p108">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="0b500-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="0b500-150">wrapText</span><span class="sxs-lookup"><span data-stu-id="0b500-150">wrapText</span></span>|<span data-ttu-id="0b500-151">boolean</span><span class="sxs-lookup"><span data-stu-id="0b500-151">boolean</span></span>|<span data-ttu-id="0b500-p109">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="0b500-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="0b500-154">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-154">Response</span></span>

<span data-ttu-id="0b500-155">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [workbookRangeFormat](../resources/workbookrangeformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-155">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b500-156">示例</span><span class="sxs-lookup"><span data-stu-id="0b500-156">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="0b500-157">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="0b500-157">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="0b500-158">以下示例演示如何更新指定范围的[workbookRangeFormat、workbookRangeFill](../resources/workbookrangeformat.md)[](../resources/workbookrangefill.md)和[workbookRangeFont](../resources/workbookrangefont.md)属性的属性。</span><span class="sxs-lookup"><span data-stu-id="0b500-158">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="0b500-159">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="0b500-159">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="0b500-161">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-161">Request</span></span>
<span data-ttu-id="0b500-162">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="0b500-162">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-164">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-167">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-168">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-168">Response</span></span>
<span data-ttu-id="0b500-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-169">Here is an example of the response.</span></span> <span data-ttu-id="0b500-170">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-170">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="0b500-171">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-171">Request</span></span>
<span data-ttu-id="0b500-172">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="0b500-172">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-174">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-177">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-178">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-178">Response</span></span>
<span data-ttu-id="0b500-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-179">Here is an example of the response.</span></span> <span data-ttu-id="0b500-180">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-180">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="0b500-181">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-181">Request</span></span>
<span data-ttu-id="0b500-182">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="0b500-182">This request updates the background color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-183">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-184">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-187">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-188">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-188">Response</span></span>
<span data-ttu-id="0b500-189">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-189">Here is an example of the response.</span></span> <span data-ttu-id="0b500-190">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-190">Note: The response object shown here might be shortened for readability.</span></span>
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
##### <a name="request"></a><span data-ttu-id="0b500-191">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-191">Request</span></span>
<span data-ttu-id="0b500-192">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="0b500-192">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-193">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-194">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-197">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-198">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-198">Response</span></span>
<span data-ttu-id="0b500-199">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-199">Here is an example of the response.</span></span> <span data-ttu-id="0b500-200">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-200">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="0b500-201">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-201">Request</span></span>
<span data-ttu-id="0b500-202">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="0b500-202">This request updates the font style and size of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-203">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-204">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-207">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-208">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-208">Response</span></span>
<span data-ttu-id="0b500-209">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-209">Here is an example of the response.</span></span> <span data-ttu-id="0b500-210">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-210">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="0b500-211">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-211">Request</span></span>
<span data-ttu-id="0b500-212">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="0b500-212">This request updates the background color of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-214">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-217">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-218">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-218">Response</span></span>
<span data-ttu-id="0b500-219">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-219">Here is an example of the response.</span></span> <span data-ttu-id="0b500-220">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-220">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="0b500-221">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-221">Request</span></span>
<span data-ttu-id="0b500-222">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="0b500-222">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-224">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-227">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-227">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-228">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-228">Response</span></span>
<span data-ttu-id="0b500-229">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-229">Here is an example of the response.</span></span> <span data-ttu-id="0b500-230">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-230">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="0b500-231">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-231">Request</span></span>
<span data-ttu-id="0b500-232">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="0b500-232">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="0b500-233">请注意，下划线属性采用 **单** 或 **双** 作为值。</span><span class="sxs-lookup"><span data-stu-id="0b500-233">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b500-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-234">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-235">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-238">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-238">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-239">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-239">Response</span></span>
<span data-ttu-id="0b500-240">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-240">Here is an example of the response.</span></span> <span data-ttu-id="0b500-241">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-241">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="0b500-242">请求</span><span class="sxs-lookup"><span data-stu-id="0b500-242">Request</span></span>
<span data-ttu-id="0b500-243">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="0b500-243">This request updates the background color of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0b500-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b500-244">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b500-245">C#</span><span class="sxs-lookup"><span data-stu-id="0b500-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b500-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b500-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b500-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b500-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b500-248">Java</span><span class="sxs-lookup"><span data-stu-id="0b500-248">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b500-249">响应</span><span class="sxs-lookup"><span data-stu-id="0b500-249">Response</span></span>
<span data-ttu-id="0b500-250">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b500-250">Here is an example of the response.</span></span> <span data-ttu-id="0b500-251">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b500-251">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_rangeformat_font_three/underline:\r\n       Expected type String but actual was Single. Property: underline, actual value: 'Single'"
  ]
}
-->


