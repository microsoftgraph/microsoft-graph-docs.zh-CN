---
title: 通过 Microsoft Graph 更新 Excel 区域格式
description: 下面的几个示例展示了如何更新指定区域的 RangeFormat、RangeFill 和 RangeFont 属性。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ae373ef28a77584d403adda5d4c948fa4c1325ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050176"
---
# <a name="update-a-range-format-in-excel-with-microsoft-graph"></a><span data-ttu-id="b259e-103">使用 Microsoft Graph 更新 Excel 中的区域格式</span><span class="sxs-lookup"><span data-stu-id="b259e-103">Update a range format in Excel with Microsoft Graph</span></span>

<span data-ttu-id="b259e-104">以下示例演示如何更新指定区域的 [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0)、[RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0) 和 [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) 属性的属性。</span><span class="sxs-lookup"><span data-stu-id="b259e-104">The following examples demonstrate how to update properties of the [RangeFormat](/graph/api/resources/rangeformat?view=graph-rest-1.0), [RangeFill](/graph/api/resources/rangefill?view=graph-rest-1.0), and [RangeFont](/graph/api/resources/rangefont?view=graph-rest-1.0) properties of a specified range.</span></span>

<span data-ttu-id="b259e-105">这组请求的结果是一个表格，其中的三个单元格的格式如下图中的前三个单元格所示。</span><span class="sxs-lookup"><span data-stu-id="b259e-105">The result of this set of requests is a table with three cells formatted like the top three cells in the image below.</span></span>

![其中的三个单元格的格式、填充和字体属性已更新的 Excel 图表表格。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/ExcelRangeFormatting.png)

##### <a name="request"></a><span data-ttu-id="b259e-107">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-107">Request</span></span>
<span data-ttu-id="b259e-108">此请求更新第一个单元格的垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="b259e-108">This request updates the vertical alignment, row height, and column height of the first cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-109">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-109">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-110">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-110">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-111">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-111">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-112">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-112">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-113">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-113">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-114">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-114">Response</span></span>
<span data-ttu-id="b259e-115">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-115">Here is an example of the response.</span></span> <span data-ttu-id="b259e-116">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-116">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="b259e-117">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-117">Request</span></span>
<span data-ttu-id="b259e-118">此请求更新第一个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="b259e-118">This request updates the font style, size, and color of the first cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-119">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-120">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-123">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-124">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-124">Response</span></span>
<span data-ttu-id="b259e-125">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-125">Here is an example of the response.</span></span> <span data-ttu-id="b259e-126">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-126">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="b259e-127">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-127">Request</span></span>
<span data-ttu-id="b259e-128">此请求更新第一个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="b259e-128">This request updates the background color of the first cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-129">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-130">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-133">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-134">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-134">Response</span></span>
<span data-ttu-id="b259e-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-135">Here is an example of the response.</span></span> <span data-ttu-id="b259e-136">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-136">Note: The response object shown here might be shortened for readability.</span></span>
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
##### <a name="request"></a><span data-ttu-id="b259e-137">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-137">Request</span></span>
<span data-ttu-id="b259e-138">此请求更新第二个单元格的垂直对齐方式、水平对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="b259e-138">This request updates the vertical alignment, horizontal alignment, row height, and column height of the second cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-140">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-143">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-144">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-144">Response</span></span>
<span data-ttu-id="b259e-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-145">Here is an example of the response.</span></span> <span data-ttu-id="b259e-146">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-146">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="b259e-147">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-147">Request</span></span>
<span data-ttu-id="b259e-148">此请求更新第二个单元格的字形和大小。</span><span class="sxs-lookup"><span data-stu-id="b259e-148">This request updates the font style and size of the second cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-150">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-153">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-154">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-154">Response</span></span>
<span data-ttu-id="b259e-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-155">Here is an example of the response.</span></span> <span data-ttu-id="b259e-156">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-156">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="b259e-157">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-157">Request</span></span>
<span data-ttu-id="b259e-158">此请求更新第二个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="b259e-158">This request updates the background color of the second cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-160">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-two-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-two-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-two-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-163">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-two-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-164">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-164">Response</span></span>
<span data-ttu-id="b259e-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-165">Here is an example of the response.</span></span> <span data-ttu-id="b259e-166">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-166">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="b259e-167">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-167">Request</span></span>
<span data-ttu-id="b259e-168">此请求更新第三个单元格的水平对齐方式、垂直对齐方式、行高和列高。</span><span class="sxs-lookup"><span data-stu-id="b259e-168">This request updates the horizontal alignment, vertical alignment, row height, and column height of the third cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-169">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-170">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-173">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-174">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-174">Response</span></span>
<span data-ttu-id="b259e-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-175">Here is an example of the response.</span></span> <span data-ttu-id="b259e-176">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-176">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="b259e-177">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-177">Request</span></span>
<span data-ttu-id="b259e-178">此请求更新第三个单元格的字形、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="b259e-178">This request updates the font style, size, and color of the third cell.</span></span> <span data-ttu-id="b259e-179">请注意，下划线属性采用 **单** 或 **双** 作为值。</span><span class="sxs-lookup"><span data-stu-id="b259e-179">Note that the underline property takes **Single** or **Double** as values.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-181">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-font-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-font-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-font-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-184">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-font-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-185">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-185">Response</span></span>
<span data-ttu-id="b259e-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-186">Here is an example of the response.</span></span> <span data-ttu-id="b259e-187">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-187">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request"></a><span data-ttu-id="b259e-188">请求</span><span class="sxs-lookup"><span data-stu-id="b259e-188">Request</span></span>
<span data-ttu-id="b259e-189">此请求更新第三个单元格的背景色。</span><span class="sxs-lookup"><span data-stu-id="b259e-189">This request updates the background color of the third cell.</span></span>


# <a name="http"></a>[<span data-ttu-id="b259e-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="b259e-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b259e-191">C#</span><span class="sxs-lookup"><span data-stu-id="b259e-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeformat-fill-three-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b259e-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b259e-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeformat-fill-three-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b259e-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b259e-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeformat-fill-three-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b259e-194">Java</span><span class="sxs-lookup"><span data-stu-id="b259e-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-rangeformat-fill-three-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b259e-195">响应</span><span class="sxs-lookup"><span data-stu-id="b259e-195">Response</span></span>
<span data-ttu-id="b259e-196">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b259e-196">Here is an example of the response.</span></span> <span data-ttu-id="b259e-197">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b259e-197">Note: The response object shown here might be shortened for readability.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="b259e-198">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b259e-198">See also</span></span>
* [<span data-ttu-id="b259e-199">通过 Microsoft Graph 管理 Excel 会话</span><span class="sxs-lookup"><span data-stu-id="b259e-199">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="b259e-200">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="b259e-200">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="b259e-201">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="b259e-201">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="b259e-202">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="b259e-202">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="b259e-203">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="b259e-203">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update a range format in Excel with Microsoft Graph",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
