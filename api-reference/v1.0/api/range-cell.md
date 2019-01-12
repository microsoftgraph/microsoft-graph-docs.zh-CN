---
title: Range:单元格
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a46f0e43a9eb1099c2df615b88f15576afa30e9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951479"
---
# <a name="range-cell"></a><span data-ttu-id="a39c1-105">Range:单元格</span><span class="sxs-lookup"><span data-stu-id="a39c1-105">Range: Cell</span></span>

<span data-ttu-id="a39c1-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。</span><span class="sxs-lookup"><span data-stu-id="a39c1-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="a39c1-109">权限</span><span class="sxs-lookup"><span data-stu-id="a39c1-109">Permissions</span></span>
<span data-ttu-id="a39c1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a39c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a39c1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a39c1-112">Permission type</span></span>      | <span data-ttu-id="a39c1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a39c1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a39c1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a39c1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a39c1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a39c1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a39c1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a39c1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a39c1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a39c1-117">Not supported.</span></span>    |
|<span data-ttu-id="a39c1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a39c1-118">Application</span></span> | <span data-ttu-id="a39c1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a39c1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a39c1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a39c1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/cell

```
## <a name="request-headers"></a><span data-ttu-id="a39c1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a39c1-121">Request headers</span></span>
| <span data-ttu-id="a39c1-122">名称</span><span class="sxs-lookup"><span data-stu-id="a39c1-122">Name</span></span>       | <span data-ttu-id="a39c1-123">说明</span><span class="sxs-lookup"><span data-stu-id="a39c1-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a39c1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a39c1-124">Authorization</span></span>  | <span data-ttu-id="a39c1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a39c1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a39c1-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a39c1-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="a39c1-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a39c1-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="a39c1-130">路径参数</span><span class="sxs-lookup"><span data-stu-id="a39c1-130">Path parameters</span></span>
<span data-ttu-id="a39c1-131">在路径中，提供了以下参数。</span><span class="sxs-lookup"><span data-stu-id="a39c1-131">In the path, provide the following parameters.</span></span>

| <span data-ttu-id="a39c1-132">参数</span><span class="sxs-lookup"><span data-stu-id="a39c1-132">Parameter</span></span>    | <span data-ttu-id="a39c1-133">类型</span><span class="sxs-lookup"><span data-stu-id="a39c1-133">Type</span></span>   |<span data-ttu-id="a39c1-134">说明</span><span class="sxs-lookup"><span data-stu-id="a39c1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a39c1-135">row</span><span class="sxs-lookup"><span data-stu-id="a39c1-135">row</span></span>|<span data-ttu-id="a39c1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a39c1-136">Int32</span></span>|<span data-ttu-id="a39c1-p106">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="a39c1-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="a39c1-139">column</span><span class="sxs-lookup"><span data-stu-id="a39c1-139">column</span></span>|<span data-ttu-id="a39c1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a39c1-140">Int32</span></span>|<span data-ttu-id="a39c1-p107">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="a39c1-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="a39c1-143">响应</span><span class="sxs-lookup"><span data-stu-id="a39c1-143">Response</span></span>

<span data-ttu-id="a39c1-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a39c1-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a39c1-145">示例</span><span class="sxs-lookup"><span data-stu-id="a39c1-145">Example</span></span>
<span data-ttu-id="a39c1-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a39c1-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a39c1-147">请求</span><span class="sxs-lookup"><span data-stu-id="a39c1-147">Request</span></span>
<span data-ttu-id="a39c1-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a39c1-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)
```

##### <a name="response"></a><span data-ttu-id="a39c1-149">响应</span><span class="sxs-lookup"><span data-stu-id="a39c1-149">Response</span></span>
<span data-ttu-id="a39c1-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a39c1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
