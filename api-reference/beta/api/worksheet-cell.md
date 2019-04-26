---
title: Worksheet:Cell
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: aca0ee396860a1f12fe820faea2fdc99355e6f03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339590"
---
# <a name="worksheet-cell"></a><span data-ttu-id="5abf4-104">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="5abf4-104">Worksheet: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5abf4-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="5abf4-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="5abf4-107">权限</span><span class="sxs-lookup"><span data-stu-id="5abf4-107">Permissions</span></span>
<span data-ttu-id="5abf4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5abf4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5abf4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5abf4-110">Permission type</span></span>      | <span data-ttu-id="5abf4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5abf4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5abf4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5abf4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5abf4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5abf4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5abf4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5abf4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5abf4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5abf4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5abf4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5abf4-116">Application</span></span> | <span data-ttu-id="5abf4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5abf4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5abf4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5abf4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="5abf4-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="5abf4-119">Function parameters</span></span>
<span data-ttu-id="5abf4-120">在请求路径中, 提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="5abf4-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="5abf4-121">参数</span><span class="sxs-lookup"><span data-stu-id="5abf4-121">Parameter</span></span>    | <span data-ttu-id="5abf4-122">类型</span><span class="sxs-lookup"><span data-stu-id="5abf4-122">Type</span></span>   |<span data-ttu-id="5abf4-123">说明</span><span class="sxs-lookup"><span data-stu-id="5abf4-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5abf4-124">row</span><span class="sxs-lookup"><span data-stu-id="5abf4-124">row</span></span>|<span data-ttu-id="5abf4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5abf4-125">Int32</span></span>|<span data-ttu-id="5abf4-p104">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="5abf4-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="5abf4-128">column</span><span class="sxs-lookup"><span data-stu-id="5abf4-128">column</span></span>|<span data-ttu-id="5abf4-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5abf4-129">Int32</span></span>|<span data-ttu-id="5abf4-130">要检索的单元格的列号。</span><span class="sxs-lookup"><span data-stu-id="5abf4-130">Column number of the cell to be retrieved.</span></span> <span data-ttu-id="5abf4-131">从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="5abf4-131">Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5abf4-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="5abf4-132">Request headers</span></span>
| <span data-ttu-id="5abf4-133">名称</span><span class="sxs-lookup"><span data-stu-id="5abf4-133">Name</span></span>       | <span data-ttu-id="5abf4-134">说明</span><span class="sxs-lookup"><span data-stu-id="5abf4-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5abf4-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5abf4-135">Authorization</span></span>  | <span data-ttu-id="5abf4-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5abf4-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5abf4-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5abf4-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="5abf4-p107">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5abf4-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5abf4-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="5abf4-141">Request body</span></span>
<span data-ttu-id="5abf4-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5abf4-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5abf4-143">响应</span><span class="sxs-lookup"><span data-stu-id="5abf4-143">Response</span></span>

<span data-ttu-id="5abf4-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5abf4-144">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5abf4-145">示例</span><span class="sxs-lookup"><span data-stu-id="5abf4-145">Example</span></span>
<span data-ttu-id="5abf4-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5abf4-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5abf4-147">请求</span><span class="sxs-lookup"><span data-stu-id="5abf4-147">Request</span></span>
<span data-ttu-id="5abf4-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5abf4-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="5abf4-149">响应</span><span class="sxs-lookup"><span data-stu-id="5abf4-149">Response</span></span>
<span data-ttu-id="5abf4-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5abf4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
