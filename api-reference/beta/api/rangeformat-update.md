---
title: 更新 RangeFormat
description: 更新 rangeformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 169578d91ac115975f36c07c4405a810ad8c2da1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999242"
---
# <a name="update-rangeformat"></a><span data-ttu-id="19877-103">更新 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="19877-103">Update rangeformat</span></span>

<span data-ttu-id="19877-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19877-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19877-105">更新 rangeformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="19877-105">Update the properties of rangeformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="19877-106">权限</span><span class="sxs-lookup"><span data-stu-id="19877-106">Permissions</span></span>
<span data-ttu-id="19877-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19877-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="19877-109">Permission type</span></span>      | <span data-ttu-id="19877-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19877-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19877-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19877-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19877-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19877-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19877-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19877-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19877-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19877-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19877-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="19877-115">Application</span></span> | <span data-ttu-id="19877-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19877-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19877-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19877-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format
```
## <a name="optional-request-headers"></a><span data-ttu-id="19877-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="19877-118">Optional request headers</span></span>
| <span data-ttu-id="19877-119">名称</span><span class="sxs-lookup"><span data-stu-id="19877-119">Name</span></span>       | <span data-ttu-id="19877-120">说明</span><span class="sxs-lookup"><span data-stu-id="19877-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="19877-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="19877-121">Authorization</span></span>  | <span data-ttu-id="19877-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19877-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19877-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19877-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="19877-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="19877-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19877-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19877-127">Request body</span></span>
<span data-ttu-id="19877-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="19877-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="19877-131">属性</span><span class="sxs-lookup"><span data-stu-id="19877-131">Property</span></span>     | <span data-ttu-id="19877-132">类型</span><span class="sxs-lookup"><span data-stu-id="19877-132">Type</span></span>   |<span data-ttu-id="19877-133">说明</span><span class="sxs-lookup"><span data-stu-id="19877-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19877-134">columnWidth</span><span class="sxs-lookup"><span data-stu-id="19877-134">columnWidth</span></span>|<span data-ttu-id="19877-135">double</span><span class="sxs-lookup"><span data-stu-id="19877-135">double</span></span>|<span data-ttu-id="19877-p105">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="19877-p105">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="19877-138">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="19877-138">horizontalAlignment</span></span>|<span data-ttu-id="19877-139">string</span><span class="sxs-lookup"><span data-stu-id="19877-139">string</span></span>|<span data-ttu-id="19877-p106">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="19877-p106">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="19877-142">rowHeight</span><span class="sxs-lookup"><span data-stu-id="19877-142">rowHeight</span></span>|<span data-ttu-id="19877-143">double</span><span class="sxs-lookup"><span data-stu-id="19877-143">double</span></span>|<span data-ttu-id="19877-p107">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="19877-p107">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="19877-146">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="19877-146">verticalAlignment</span></span>|<span data-ttu-id="19877-147">string</span><span class="sxs-lookup"><span data-stu-id="19877-147">string</span></span>|<span data-ttu-id="19877-p108">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="19877-p108">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="19877-150">wrapText</span><span class="sxs-lookup"><span data-stu-id="19877-150">wrapText</span></span>|<span data-ttu-id="19877-151">boolean</span><span class="sxs-lookup"><span data-stu-id="19877-151">boolean</span></span>|<span data-ttu-id="19877-p109">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="19877-p109">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="response"></a><span data-ttu-id="19877-154">响应</span><span class="sxs-lookup"><span data-stu-id="19877-154">Response</span></span>

<span data-ttu-id="19877-155">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workbookRangeFormat](../resources/workbookrangeformat.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19877-155">If successful, this method returns a `200 OK` response code and updated [workbookRangeFormat](../resources/workbookrangeformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19877-156">示例</span><span class="sxs-lookup"><span data-stu-id="19877-156">Example</span></span>

### <a name="update-the-format-fill-and-font-properties-in-three-table-cells"></a><span data-ttu-id="19877-157">更新三个表格单元格的格式、填充和字体属性</span><span class="sxs-lookup"><span data-stu-id="19877-157">Update the format, fill, and font properties in three table cells</span></span>

<span data-ttu-id="19877-158">下面的示例演示如何更新指定区域的 [workbookRangeFormat](../resources/workbookrangeformat.md)、 [workbookRangeFill](../resources/workbookrangefill.md)和 [workbookRangeFont](../resources/workbookrangefont.md) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="19877-158">The following examples demonstrate how to update properties of the [workbookRangeFormat](../resources/workbookrangeformat.md), [workbookRangeFill](../resources/workbookrangefill.md), and [workbookRangeFont](../resources/workbookrangefont.md) properties of a specified range.</span></span>

<span data-ttu-id="19877-159">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="19877-159">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="19877-161">请求</span><span class="sxs-lookup"><span data-stu-id="19877-161">Request</span></span>
<span data-ttu-id="19877-162">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="19877-162">This request updates the vertical alignment, row height, and column height of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-164">C#</span><span class="sxs-lookup"><span data-stu-id="19877-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-167">响应</span><span class="sxs-lookup"><span data-stu-id="19877-167">Response</span></span>
<span data-ttu-id="19877-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="19877-171">请求</span><span class="sxs-lookup"><span data-stu-id="19877-171">Request</span></span>
<span data-ttu-id="19877-172">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="19877-172">This request updates the font style, size, and color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-174">C#</span><span class="sxs-lookup"><span data-stu-id="19877-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-177">响应</span><span class="sxs-lookup"><span data-stu-id="19877-177">Response</span></span>
<span data-ttu-id="19877-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="19877-181">请求</span><span class="sxs-lookup"><span data-stu-id="19877-181">Request</span></span>
<span data-ttu-id="19877-182">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="19877-182">This request updates the background color of the first cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-183">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-184">C#</span><span class="sxs-lookup"><span data-stu-id="19877-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-187">响应</span><span class="sxs-lookup"><span data-stu-id="19877-187">Response</span></span>
<span data-ttu-id="19877-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
##### <a name="request"></a><span data-ttu-id="19877-191">请求</span><span class="sxs-lookup"><span data-stu-id="19877-191">Request</span></span>
<span data-ttu-id="19877-192">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="19877-192">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-193">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-194">C#</span><span class="sxs-lookup"><span data-stu-id="19877-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-195">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-195">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-196">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-197">响应</span><span class="sxs-lookup"><span data-stu-id="19877-197">Response</span></span>
<span data-ttu-id="19877-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="19877-201">请求</span><span class="sxs-lookup"><span data-stu-id="19877-201">Request</span></span>
<span data-ttu-id="19877-202">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="19877-202">This request updates the font style and size of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-203">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-204">C#</span><span class="sxs-lookup"><span data-stu-id="19877-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-207">响应</span><span class="sxs-lookup"><span data-stu-id="19877-207">Response</span></span>
<span data-ttu-id="19877-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="19877-211">请求</span><span class="sxs-lookup"><span data-stu-id="19877-211">Request</span></span>
<span data-ttu-id="19877-212">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="19877-212">This request updates the background color of the second cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-214">C#</span><span class="sxs-lookup"><span data-stu-id="19877-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-217">响应</span><span class="sxs-lookup"><span data-stu-id="19877-217">Response</span></span>
<span data-ttu-id="19877-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="19877-221">请求</span><span class="sxs-lookup"><span data-stu-id="19877-221">Request</span></span>
<span data-ttu-id="19877-222">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="19877-222">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-224">C#</span><span class="sxs-lookup"><span data-stu-id="19877-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-227">响应</span><span class="sxs-lookup"><span data-stu-id="19877-227">Response</span></span>
<span data-ttu-id="19877-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="19877-231">请求</span><span class="sxs-lookup"><span data-stu-id="19877-231">Request</span></span>
<span data-ttu-id="19877-232">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="19877-232">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="19877-233">请注意，下划线属性采用**单**或**双**作为值。</span><span class="sxs-lookup"><span data-stu-id="19877-233">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="19877-234">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-234">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-235">C#</span><span class="sxs-lookup"><span data-stu-id="19877-235">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-236">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-236">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-237">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-237">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-238">响应</span><span class="sxs-lookup"><span data-stu-id="19877-238">Response</span></span>
<span data-ttu-id="19877-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request"></a><span data-ttu-id="19877-242">请求</span><span class="sxs-lookup"><span data-stu-id="19877-242">Request</span></span>
<span data-ttu-id="19877-243">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="19877-243">This request updates the background color of the third cell.</span></span> 


# <a name="http"></a>[<span data-ttu-id="19877-244">HTTP</span><span class="sxs-lookup"><span data-stu-id="19877-244">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="19877-245">C#</span><span class="sxs-lookup"><span data-stu-id="19877-245">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19877-246">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19877-246">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19877-247">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19877-247">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="19877-248">响应</span><span class="sxs-lookup"><span data-stu-id="19877-248">Response</span></span>
<span data-ttu-id="19877-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19877-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


