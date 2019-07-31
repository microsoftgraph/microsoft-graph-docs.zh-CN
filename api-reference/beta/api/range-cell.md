---
title: Range:单元格
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9dffd75ed5e70e373f824d11fdcc287ce09f051a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991945"
---
# <a name="range-cell"></a><span data-ttu-id="9410c-105">Range:单元格</span><span class="sxs-lookup"><span data-stu-id="9410c-105">Range: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9410c-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。</span><span class="sxs-lookup"><span data-stu-id="9410c-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="9410c-109">权限</span><span class="sxs-lookup"><span data-stu-id="9410c-109">Permissions</span></span>
<span data-ttu-id="9410c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9410c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9410c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="9410c-112">Permission type</span></span>      | <span data-ttu-id="9410c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9410c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9410c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9410c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9410c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9410c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9410c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9410c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9410c-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9410c-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9410c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="9410c-118">Application</span></span> | <span data-ttu-id="9410c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9410c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9410c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9410c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="9410c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9410c-121">Request headers</span></span>
| <span data-ttu-id="9410c-122">名称</span><span class="sxs-lookup"><span data-stu-id="9410c-122">Name</span></span>       | <span data-ttu-id="9410c-123">说明</span><span class="sxs-lookup"><span data-stu-id="9410c-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9410c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9410c-124">Authorization</span></span>  | <span data-ttu-id="9410c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9410c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9410c-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9410c-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="9410c-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9410c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9410c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="9410c-130">Request body</span></span>
<span data-ttu-id="9410c-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9410c-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9410c-132">参数</span><span class="sxs-lookup"><span data-stu-id="9410c-132">Parameter</span></span>    | <span data-ttu-id="9410c-133">类型</span><span class="sxs-lookup"><span data-stu-id="9410c-133">Type</span></span>   |<span data-ttu-id="9410c-134">说明</span><span class="sxs-lookup"><span data-stu-id="9410c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9410c-135">row</span><span class="sxs-lookup"><span data-stu-id="9410c-135">row</span></span>|<span data-ttu-id="9410c-136">number</span><span class="sxs-lookup"><span data-stu-id="9410c-136">number</span></span>|<span data-ttu-id="9410c-p106">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="9410c-p106">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="9410c-139">column</span><span class="sxs-lookup"><span data-stu-id="9410c-139">column</span></span>|<span data-ttu-id="9410c-140">number</span><span class="sxs-lookup"><span data-stu-id="9410c-140">number</span></span>|<span data-ttu-id="9410c-p107">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="9410c-p107">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="9410c-143">响应</span><span class="sxs-lookup"><span data-stu-id="9410c-143">Response</span></span>

<span data-ttu-id="9410c-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9410c-144">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9410c-145">示例</span><span class="sxs-lookup"><span data-stu-id="9410c-145">Example</span></span>
<span data-ttu-id="9410c-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9410c-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9410c-147">请求</span><span class="sxs-lookup"><span data-stu-id="9410c-147">Request</span></span>
<span data-ttu-id="9410c-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9410c-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9410c-149">响应</span><span class="sxs-lookup"><span data-stu-id="9410c-149">Response</span></span>
<span data-ttu-id="9410c-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9410c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
