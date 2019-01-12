---
title: Worksheet:Cell
description: 根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 96069c11d8e520b64854eb7a2a72dc9d5f6de25b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967299"
---
# <a name="worksheet-cell"></a><span data-ttu-id="ab56c-104">Worksheet:Cell</span><span class="sxs-lookup"><span data-stu-id="ab56c-104">Worksheet: Cell</span></span>

<span data-ttu-id="ab56c-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="ab56c-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab56c-107">权限</span><span class="sxs-lookup"><span data-stu-id="ab56c-107">Permissions</span></span>
<span data-ttu-id="ab56c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ab56c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab56c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab56c-110">Permission type</span></span>      | <span data-ttu-id="ab56c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ab56c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab56c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab56c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab56c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab56c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ab56c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab56c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab56c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab56c-115">Not supported.</span></span>    |
|<span data-ttu-id="ab56c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab56c-116">Application</span></span> | <span data-ttu-id="ab56c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab56c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab56c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab56c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="ab56c-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="ab56c-119">Function parameters</span></span>
<span data-ttu-id="ab56c-120">在请求路径中，提供了以下参数。</span><span class="sxs-lookup"><span data-stu-id="ab56c-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="ab56c-121">参数</span><span class="sxs-lookup"><span data-stu-id="ab56c-121">Parameter</span></span>    | <span data-ttu-id="ab56c-122">类型</span><span class="sxs-lookup"><span data-stu-id="ab56c-122">Type</span></span>   |<span data-ttu-id="ab56c-123">说明</span><span class="sxs-lookup"><span data-stu-id="ab56c-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab56c-124">row</span><span class="sxs-lookup"><span data-stu-id="ab56c-124">row</span></span>|<span data-ttu-id="ab56c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ab56c-125">Int32</span></span>|<span data-ttu-id="ab56c-p104">要检索的单元格的行号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="ab56c-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="ab56c-128">column</span><span class="sxs-lookup"><span data-stu-id="ab56c-128">column</span></span>|<span data-ttu-id="ab56c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ab56c-129">Int32</span></span>|<span data-ttu-id="ab56c-p105">要检索的单元格的列号。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="ab56c-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ab56c-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab56c-132">Request headers</span></span>
| <span data-ttu-id="ab56c-133">名称</span><span class="sxs-lookup"><span data-stu-id="ab56c-133">Name</span></span>       | <span data-ttu-id="ab56c-134">说明</span><span class="sxs-lookup"><span data-stu-id="ab56c-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab56c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab56c-135">Authorization</span></span>  | <span data-ttu-id="ab56c-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ab56c-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab56c-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ab56c-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="ab56c-p107">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ab56c-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab56c-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab56c-141">Request body</span></span>
<span data-ttu-id="ab56c-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ab56c-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab56c-143">响应</span><span class="sxs-lookup"><span data-stu-id="ab56c-143">Response</span></span>

<span data-ttu-id="ab56c-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ab56c-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab56c-145">示例</span><span class="sxs-lookup"><span data-stu-id="ab56c-145">Example</span></span>
<span data-ttu-id="ab56c-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ab56c-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ab56c-147">请求</span><span class="sxs-lookup"><span data-stu-id="ab56c-147">Request</span></span>
<span data-ttu-id="ab56c-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab56c-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="ab56c-149">响应</span><span class="sxs-lookup"><span data-stu-id="ab56c-149">Response</span></span>
<span data-ttu-id="ab56c-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab56c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
