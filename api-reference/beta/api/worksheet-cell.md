---
title: Worksheet:Cell
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2a5d5d108974f337d74788ddec2b3fdc05f9d3f1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051667"
---
# <a name="worksheet-cell"></a><span data-ttu-id="ee7fe-104">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="ee7fe-104">Worksheet: Cell</span></span>

<span data-ttu-id="ee7fe-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7fe-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee7fe-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee7fe-108">权限</span><span class="sxs-lookup"><span data-stu-id="ee7fe-108">Permissions</span></span>
<span data-ttu-id="ee7fe-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee7fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee7fe-111">Permission type</span></span>      | <span data-ttu-id="ee7fe-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee7fe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee7fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee7fe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ee7fe-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee7fe-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee7fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee7fe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee7fe-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee7fe-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ee7fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee7fe-117">Application</span></span> | <span data-ttu-id="ee7fe-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee7fe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee7fe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row={row},column={column})
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="ee7fe-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="ee7fe-120">Function parameters</span></span>
<span data-ttu-id="ee7fe-121">在请求路径中，提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-121">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="ee7fe-122">参数</span><span class="sxs-lookup"><span data-stu-id="ee7fe-122">Parameter</span></span>    | <span data-ttu-id="ee7fe-123">类型</span><span class="sxs-lookup"><span data-stu-id="ee7fe-123">Type</span></span>   |<span data-ttu-id="ee7fe-124">说明</span><span class="sxs-lookup"><span data-stu-id="ee7fe-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee7fe-125">row</span><span class="sxs-lookup"><span data-stu-id="ee7fe-125">row</span></span>|<span data-ttu-id="ee7fe-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ee7fe-126">Int32</span></span>|<span data-ttu-id="ee7fe-p104">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="ee7fe-129">column</span><span class="sxs-lookup"><span data-stu-id="ee7fe-129">column</span></span>|<span data-ttu-id="ee7fe-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ee7fe-130">Int32</span></span>|<span data-ttu-id="ee7fe-p105">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ee7fe-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee7fe-133">Request headers</span></span>
| <span data-ttu-id="ee7fe-134">名称</span><span class="sxs-lookup"><span data-stu-id="ee7fe-134">Name</span></span>       | <span data-ttu-id="ee7fe-135">说明</span><span class="sxs-lookup"><span data-stu-id="ee7fe-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee7fe-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee7fe-136">Authorization</span></span>  | <span data-ttu-id="ee7fe-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee7fe-139">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ee7fe-139">Workbook-Session-Id</span></span>  | <span data-ttu-id="ee7fe-p107">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee7fe-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee7fe-142">Request body</span></span>
<span data-ttu-id="ee7fe-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee7fe-144">响应</span><span class="sxs-lookup"><span data-stu-id="ee7fe-144">Response</span></span>

<span data-ttu-id="ee7fe-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee7fe-146">示例</span><span class="sxs-lookup"><span data-stu-id="ee7fe-146">Example</span></span>
<span data-ttu-id="ee7fe-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee7fe-148">请求</span><span class="sxs-lookup"><span data-stu-id="ee7fe-148">Request</span></span>
<span data-ttu-id="ee7fe-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="ee7fe-150">响应</span><span class="sxs-lookup"><span data-stu-id="ee7fe-150">Response</span></span>
<span data-ttu-id="ee7fe-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-151">Here is an example of the response.</span></span> <span data-ttu-id="ee7fe-152">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee7fe-152">Note: The response object shown here might be shortened for readability.</span></span>
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


