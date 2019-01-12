---
title: Range:单元格
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ef9888c934a0d85f66c49e062074c2c328cafa13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915653"
---
# <a name="range-cell"></a><span data-ttu-id="d2cdb-105">Range:单元格</span><span class="sxs-lookup"><span data-stu-id="d2cdb-105">Range: Cell</span></span>

> <span data-ttu-id="d2cdb-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2cdb-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2cdb-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2cdb-111">权限</span><span class="sxs-lookup"><span data-stu-id="d2cdb-111">Permissions</span></span>
<span data-ttu-id="d2cdb-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2cdb-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2cdb-114">Permission type</span></span>      | <span data-ttu-id="d2cdb-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2cdb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2cdb-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2cdb-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d2cdb-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2cdb-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2cdb-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2cdb-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2cdb-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2cdb-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d2cdb-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2cdb-120">Application</span></span> | <span data-ttu-id="d2cdb-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2cdb-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2cdb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="d2cdb-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2cdb-123">Request headers</span></span>
| <span data-ttu-id="d2cdb-124">名称</span><span class="sxs-lookup"><span data-stu-id="d2cdb-124">Name</span></span>       | <span data-ttu-id="d2cdb-125">说明</span><span class="sxs-lookup"><span data-stu-id="d2cdb-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d2cdb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2cdb-126">Authorization</span></span>  | <span data-ttu-id="d2cdb-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2cdb-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d2cdb-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="d2cdb-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2cdb-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2cdb-132">Request body</span></span>
<span data-ttu-id="d2cdb-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d2cdb-134">参数</span><span class="sxs-lookup"><span data-stu-id="d2cdb-134">Parameter</span></span>    | <span data-ttu-id="d2cdb-135">类型</span><span class="sxs-lookup"><span data-stu-id="d2cdb-135">Type</span></span>   |<span data-ttu-id="d2cdb-136">说明</span><span class="sxs-lookup"><span data-stu-id="d2cdb-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2cdb-137">row</span><span class="sxs-lookup"><span data-stu-id="d2cdb-137">row</span></span>|<span data-ttu-id="d2cdb-138">number</span><span class="sxs-lookup"><span data-stu-id="d2cdb-138">number</span></span>|<span data-ttu-id="d2cdb-p107">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-p107">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="d2cdb-141">column</span><span class="sxs-lookup"><span data-stu-id="d2cdb-141">column</span></span>|<span data-ttu-id="d2cdb-142">number</span><span class="sxs-lookup"><span data-stu-id="d2cdb-142">number</span></span>|<span data-ttu-id="d2cdb-p108">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-p108">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="d2cdb-145">响应</span><span class="sxs-lookup"><span data-stu-id="d2cdb-145">Response</span></span>

<span data-ttu-id="d2cdb-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2cdb-147">示例</span><span class="sxs-lookup"><span data-stu-id="d2cdb-147">Example</span></span>
<span data-ttu-id="d2cdb-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2cdb-149">请求</span><span class="sxs-lookup"><span data-stu-id="d2cdb-149">Request</span></span>
<span data-ttu-id="d2cdb-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="d2cdb-151">响应</span><span class="sxs-lookup"><span data-stu-id="d2cdb-151">Response</span></span>
<span data-ttu-id="d2cdb-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2cdb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
