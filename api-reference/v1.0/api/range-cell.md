---
title: Range:单元格
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 239911c34978cd2fd8ee766fd318343a28057a8c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365113"
---
# <a name="range-cell"></a><span data-ttu-id="f70c2-105">Range:单元格</span><span class="sxs-lookup"><span data-stu-id="f70c2-105">Range: Cell</span></span>

<span data-ttu-id="f70c2-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。</span><span class="sxs-lookup"><span data-stu-id="f70c2-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f70c2-109">权限</span><span class="sxs-lookup"><span data-stu-id="f70c2-109">Permissions</span></span>
<span data-ttu-id="f70c2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f70c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f70c2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f70c2-112">Permission type</span></span>      | <span data-ttu-id="f70c2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f70c2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f70c2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f70c2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f70c2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f70c2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f70c2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f70c2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f70c2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f70c2-117">Not supported.</span></span>    |
|<span data-ttu-id="f70c2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f70c2-118">Application</span></span> | <span data-ttu-id="f70c2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f70c2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f70c2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f70c2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="f70c2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f70c2-121">Request headers</span></span>
| <span data-ttu-id="f70c2-122">名称</span><span class="sxs-lookup"><span data-stu-id="f70c2-122">Name</span></span>       | <span data-ttu-id="f70c2-123">说明</span><span class="sxs-lookup"><span data-stu-id="f70c2-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f70c2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f70c2-124">Authorization</span></span>  | <span data-ttu-id="f70c2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f70c2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f70c2-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f70c2-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="f70c2-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f70c2-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="f70c2-130">路径参数</span><span class="sxs-lookup"><span data-stu-id="f70c2-130">Path parameters</span></span>
<span data-ttu-id="f70c2-131">在路径中, 提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="f70c2-131">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="f70c2-132">参数</span><span class="sxs-lookup"><span data-stu-id="f70c2-132">Parameter</span></span>    | <span data-ttu-id="f70c2-133">类型</span><span class="sxs-lookup"><span data-stu-id="f70c2-133">Type</span></span>   |<span data-ttu-id="f70c2-134">说明</span><span class="sxs-lookup"><span data-stu-id="f70c2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f70c2-135">row</span><span class="sxs-lookup"><span data-stu-id="f70c2-135">row</span></span>|<span data-ttu-id="f70c2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f70c2-136">Int32</span></span>|<span data-ttu-id="f70c2-p106">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="f70c2-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="f70c2-139">column</span><span class="sxs-lookup"><span data-stu-id="f70c2-139">column</span></span>|<span data-ttu-id="f70c2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f70c2-140">Int32</span></span>|<span data-ttu-id="f70c2-p107">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="f70c2-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f70c2-143">响应</span><span class="sxs-lookup"><span data-stu-id="f70c2-143">Response</span></span>

<span data-ttu-id="f70c2-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f70c2-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f70c2-145">示例</span><span class="sxs-lookup"><span data-stu-id="f70c2-145">Example</span></span>
<span data-ttu-id="f70c2-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f70c2-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f70c2-147">请求</span><span class="sxs-lookup"><span data-stu-id="f70c2-147">Request</span></span>
<span data-ttu-id="f70c2-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f70c2-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f70c2-149">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f70c2-149">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f70c2-150">C#</span><span class="sxs-lookup"><span data-stu-id="f70c2-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-cell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f70c2-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f70c2-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-cell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f70c2-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="f70c2-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-cell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f70c2-153">Java</span><span class="sxs-lookup"><span data-stu-id="f70c2-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-cell-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f70c2-154">响应</span><span class="sxs-lookup"><span data-stu-id="f70c2-154">Response</span></span>
<span data-ttu-id="f70c2-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f70c2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
