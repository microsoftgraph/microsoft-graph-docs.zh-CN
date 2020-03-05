---
title: Worksheet:Cell
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d0cf070f9e6b4a7df176eb68e616f339ae36a125
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451226"
---
# <a name="worksheet-cell"></a><span data-ttu-id="d7c2a-104">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="d7c2a-104">Worksheet: Cell</span></span>

<span data-ttu-id="d7c2a-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d7c2a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7c2a-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7c2a-108">权限</span><span class="sxs-lookup"><span data-stu-id="d7c2a-108">Permissions</span></span>
<span data-ttu-id="d7c2a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7c2a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7c2a-111">Permission type</span></span>      | <span data-ttu-id="d7c2a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7c2a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7c2a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7c2a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d7c2a-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7c2a-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7c2a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7c2a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7c2a-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7c2a-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7c2a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7c2a-117">Application</span></span> | <span data-ttu-id="d7c2a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7c2a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7c2a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="d7c2a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="d7c2a-120">Function parameters</span></span>
<span data-ttu-id="d7c2a-121">在请求路径中，提供以下参数。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-121">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="d7c2a-122">参数</span><span class="sxs-lookup"><span data-stu-id="d7c2a-122">Parameter</span></span>    | <span data-ttu-id="d7c2a-123">类型</span><span class="sxs-lookup"><span data-stu-id="d7c2a-123">Type</span></span>   |<span data-ttu-id="d7c2a-124">说明</span><span class="sxs-lookup"><span data-stu-id="d7c2a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7c2a-125">row</span><span class="sxs-lookup"><span data-stu-id="d7c2a-125">row</span></span>|<span data-ttu-id="d7c2a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c2a-126">Int32</span></span>|<span data-ttu-id="d7c2a-p104">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="d7c2a-129">column</span><span class="sxs-lookup"><span data-stu-id="d7c2a-129">column</span></span>|<span data-ttu-id="d7c2a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d7c2a-130">Int32</span></span>|<span data-ttu-id="d7c2a-131">要检索的单元格的列号。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-131">Column number of the cell to be retrieved.</span></span> <span data-ttu-id="d7c2a-132">从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-132">Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d7c2a-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7c2a-133">Request headers</span></span>
| <span data-ttu-id="d7c2a-134">名称</span><span class="sxs-lookup"><span data-stu-id="d7c2a-134">Name</span></span>       | <span data-ttu-id="d7c2a-135">说明</span><span class="sxs-lookup"><span data-stu-id="d7c2a-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7c2a-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7c2a-136">Authorization</span></span>  | <span data-ttu-id="d7c2a-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d7c2a-139">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d7c2a-139">Workbook-Session-Id</span></span>  | <span data-ttu-id="d7c2a-p107">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7c2a-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7c2a-142">Request body</span></span>
<span data-ttu-id="d7c2a-143">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7c2a-144">响应</span><span class="sxs-lookup"><span data-stu-id="d7c2a-144">Response</span></span>

<span data-ttu-id="d7c2a-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-145">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c2a-146">示例</span><span class="sxs-lookup"><span data-stu-id="d7c2a-146">Example</span></span>
<span data-ttu-id="d7c2a-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d7c2a-148">请求</span><span class="sxs-lookup"><span data-stu-id="d7c2a-148">Request</span></span>
<span data-ttu-id="d7c2a-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="d7c2a-150">响应</span><span class="sxs-lookup"><span data-stu-id="d7c2a-150">Response</span></span>
<span data-ttu-id="d7c2a-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7c2a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
