---
title: Range:单元格
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 491313183aa29b3acb38b3e9003ac7dc06bf819a
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575992"
---
# <a name="range-cell"></a><span data-ttu-id="8ab0b-105">Range:单元格</span><span class="sxs-lookup"><span data-stu-id="8ab0b-105">Range: Cell</span></span>

<span data-ttu-id="8ab0b-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ab0b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ab0b-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ab0b-110">权限</span><span class="sxs-lookup"><span data-stu-id="8ab0b-110">Permissions</span></span>
<span data-ttu-id="8ab0b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ab0b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ab0b-113">Permission type</span></span>      | <span data-ttu-id="8ab0b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ab0b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ab0b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ab0b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8ab0b-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ab0b-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ab0b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ab0b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ab0b-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ab0b-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ab0b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ab0b-119">Application</span></span> | <span data-ttu-id="8ab0b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ab0b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ab0b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/names/{name}/range/Cell
GET /me/drive/root:/{item-path}:/workbook/names/{name}/range/Cell
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/range/Cell
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="8ab0b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ab0b-122">Request headers</span></span>
| <span data-ttu-id="8ab0b-123">名称</span><span class="sxs-lookup"><span data-stu-id="8ab0b-123">Name</span></span>       | <span data-ttu-id="8ab0b-124">说明</span><span class="sxs-lookup"><span data-stu-id="8ab0b-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ab0b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ab0b-125">Authorization</span></span>  | <span data-ttu-id="8ab0b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ab0b-128">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ab0b-128">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ab0b-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ab0b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ab0b-131">Request body</span></span>
<span data-ttu-id="8ab0b-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ab0b-133">参数</span><span class="sxs-lookup"><span data-stu-id="8ab0b-133">Parameter</span></span>    | <span data-ttu-id="8ab0b-134">类型</span><span class="sxs-lookup"><span data-stu-id="8ab0b-134">Type</span></span>   |<span data-ttu-id="8ab0b-135">说明</span><span class="sxs-lookup"><span data-stu-id="8ab0b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ab0b-136">row</span><span class="sxs-lookup"><span data-stu-id="8ab0b-136">row</span></span>|<span data-ttu-id="8ab0b-137">number</span><span class="sxs-lookup"><span data-stu-id="8ab0b-137">number</span></span>|<span data-ttu-id="8ab0b-p106">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="8ab0b-140">column</span><span class="sxs-lookup"><span data-stu-id="8ab0b-140">column</span></span>|<span data-ttu-id="8ab0b-141">number</span><span class="sxs-lookup"><span data-stu-id="8ab0b-141">number</span></span>|<span data-ttu-id="8ab0b-p107">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="8ab0b-144">响应</span><span class="sxs-lookup"><span data-stu-id="8ab0b-144">Response</span></span>

<span data-ttu-id="8ab0b-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ab0b-146">示例</span><span class="sxs-lookup"><span data-stu-id="8ab0b-146">Example</span></span>
<span data-ttu-id="8ab0b-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8ab0b-148">请求</span><span class="sxs-lookup"><span data-stu-id="8ab0b-148">Request</span></span>
<span data-ttu-id="8ab0b-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="8ab0b-150">响应</span><span class="sxs-lookup"><span data-stu-id="8ab0b-150">Response</span></span>
<span data-ttu-id="8ab0b-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ab0b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


