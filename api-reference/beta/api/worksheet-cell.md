---
title: Worksheet:Cell
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4649a361ec46b9fb904cf959608fdee502f05c22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535980"
---
# <a name="worksheet-cell"></a><span data-ttu-id="2ed5e-104">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="2ed5e-104">Worksheet: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ed5e-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ed5e-107">权限</span><span class="sxs-lookup"><span data-stu-id="2ed5e-107">Permissions</span></span>
<span data-ttu-id="2ed5e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ed5e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ed5e-110">Permission type</span></span>      | <span data-ttu-id="2ed5e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ed5e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ed5e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed5e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ed5e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ed5e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ed5e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed5e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ed5e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ed5e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2ed5e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ed5e-116">Application</span></span> | <span data-ttu-id="2ed5e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ed5e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ed5e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="2ed5e-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="2ed5e-119">Function parameters</span></span>
<span data-ttu-id="2ed5e-120">在请求路径中, 提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="2ed5e-121">参数</span><span class="sxs-lookup"><span data-stu-id="2ed5e-121">Parameter</span></span>    | <span data-ttu-id="2ed5e-122">类型</span><span class="sxs-lookup"><span data-stu-id="2ed5e-122">Type</span></span>   |<span data-ttu-id="2ed5e-123">说明</span><span class="sxs-lookup"><span data-stu-id="2ed5e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ed5e-124">row</span><span class="sxs-lookup"><span data-stu-id="2ed5e-124">row</span></span>|<span data-ttu-id="2ed5e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2ed5e-125">Int32</span></span>|<span data-ttu-id="2ed5e-p104">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="2ed5e-128">column</span><span class="sxs-lookup"><span data-stu-id="2ed5e-128">column</span></span>|<span data-ttu-id="2ed5e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="2ed5e-129">Int32</span></span>|<span data-ttu-id="2ed5e-130">要检索的单元格的列号。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-130">Column number of the cell to be retrieved.</span></span> <span data-ttu-id="2ed5e-131">从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-131">Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2ed5e-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ed5e-132">Request headers</span></span>
| <span data-ttu-id="2ed5e-133">名称</span><span class="sxs-lookup"><span data-stu-id="2ed5e-133">Name</span></span>       | <span data-ttu-id="2ed5e-134">说明</span><span class="sxs-lookup"><span data-stu-id="2ed5e-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ed5e-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ed5e-135">Authorization</span></span>  | <span data-ttu-id="2ed5e-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ed5e-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2ed5e-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="2ed5e-p107">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ed5e-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ed5e-141">Request body</span></span>
<span data-ttu-id="2ed5e-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed5e-143">响应</span><span class="sxs-lookup"><span data-stu-id="2ed5e-143">Response</span></span>

<span data-ttu-id="2ed5e-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ed5e-145">示例</span><span class="sxs-lookup"><span data-stu-id="2ed5e-145">Example</span></span>
<span data-ttu-id="2ed5e-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2ed5e-147">请求</span><span class="sxs-lookup"><span data-stu-id="2ed5e-147">Request</span></span>
<span data-ttu-id="2ed5e-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="2ed5e-149">响应</span><span class="sxs-lookup"><span data-stu-id="2ed5e-149">Response</span></span>
<span data-ttu-id="2ed5e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ed5e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-cell.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
