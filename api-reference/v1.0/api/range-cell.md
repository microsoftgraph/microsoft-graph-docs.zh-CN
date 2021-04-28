---
title: Range:单元格
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cb55594acc0b31ca9ce8f4f18d87df4f1529b2a0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050358"
---
# <a name="range-cell"></a><span data-ttu-id="bb86c-105">Range:单元格</span><span class="sxs-lookup"><span data-stu-id="bb86c-105">Range: Cell</span></span>

<span data-ttu-id="bb86c-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb86c-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb86c-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。</span><span class="sxs-lookup"><span data-stu-id="bb86c-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb86c-110">权限</span><span class="sxs-lookup"><span data-stu-id="bb86c-110">Permissions</span></span>
<span data-ttu-id="bb86c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb86c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb86c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb86c-113">Permission type</span></span>      | <span data-ttu-id="bb86c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb86c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb86c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb86c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bb86c-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb86c-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bb86c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb86c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb86c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb86c-118">Not supported.</span></span>    |
|<span data-ttu-id="bb86c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb86c-119">Application</span></span> | <span data-ttu-id="bb86c-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb86c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb86c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb86c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/cell
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/cell
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/cell
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="bb86c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb86c-122">Request headers</span></span>
| <span data-ttu-id="bb86c-123">名称</span><span class="sxs-lookup"><span data-stu-id="bb86c-123">Name</span></span>       | <span data-ttu-id="bb86c-124">说明</span><span class="sxs-lookup"><span data-stu-id="bb86c-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bb86c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb86c-125">Authorization</span></span>  | <span data-ttu-id="bb86c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb86c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb86c-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bb86c-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="bb86c-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="bb86c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="bb86c-131">路径参数</span><span class="sxs-lookup"><span data-stu-id="bb86c-131">Path parameters</span></span>
<span data-ttu-id="bb86c-132">在路径中，提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="bb86c-132">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="bb86c-133">参数</span><span class="sxs-lookup"><span data-stu-id="bb86c-133">Parameter</span></span>    | <span data-ttu-id="bb86c-134">类型</span><span class="sxs-lookup"><span data-stu-id="bb86c-134">Type</span></span>   |<span data-ttu-id="bb86c-135">说明</span><span class="sxs-lookup"><span data-stu-id="bb86c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb86c-136">row</span><span class="sxs-lookup"><span data-stu-id="bb86c-136">row</span></span>|<span data-ttu-id="bb86c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bb86c-137">Int32</span></span>|<span data-ttu-id="bb86c-p106">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="bb86c-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="bb86c-140">column</span><span class="sxs-lookup"><span data-stu-id="bb86c-140">column</span></span>|<span data-ttu-id="bb86c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bb86c-141">Int32</span></span>|<span data-ttu-id="bb86c-p107">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="bb86c-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="bb86c-144">响应</span><span class="sxs-lookup"><span data-stu-id="bb86c-144">Response</span></span>

<span data-ttu-id="bb86c-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb86c-145">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb86c-146">示例</span><span class="sxs-lookup"><span data-stu-id="bb86c-146">Example</span></span>
<span data-ttu-id="bb86c-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="bb86c-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bb86c-148">请求</span><span class="sxs-lookup"><span data-stu-id="bb86c-148">Request</span></span>
<span data-ttu-id="bb86c-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb86c-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb86c-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb86c-150">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```
# <a name="c"></a>[<span data-ttu-id="bb86c-151">C#</span><span class="sxs-lookup"><span data-stu-id="bb86c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-cell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb86c-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb86c-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-cell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb86c-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb86c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-cell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb86c-154">Java</span><span class="sxs-lookup"><span data-stu-id="bb86c-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-cell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb86c-155">响应</span><span class="sxs-lookup"><span data-stu-id="bb86c-155">Response</span></span>
<span data-ttu-id="bb86c-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bb86c-156">Here is an example of the response.</span></span> <span data-ttu-id="bb86c-157">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bb86c-157">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

