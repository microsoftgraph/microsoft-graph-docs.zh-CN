---
title: 'Range: insert'
description: 将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 01bb7b3a756b9d97d2d849c49cade0ff285168a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508676"
---
# <a name="range-insert"></a><span data-ttu-id="892fe-104">Range: insert</span><span class="sxs-lookup"><span data-stu-id="892fe-104">Range: insert</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="892fe-p102">将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="892fe-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="892fe-107">权限</span><span class="sxs-lookup"><span data-stu-id="892fe-107">Permissions</span></span>
<span data-ttu-id="892fe-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="892fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="892fe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="892fe-110">Permission type</span></span>      | <span data-ttu-id="892fe-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="892fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="892fe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="892fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="892fe-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="892fe-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="892fe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="892fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="892fe-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="892fe-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="892fe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="892fe-116">Application</span></span> | <span data-ttu-id="892fe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="892fe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="892fe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="892fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="892fe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="892fe-119">Request headers</span></span>
| <span data-ttu-id="892fe-120">名称</span><span class="sxs-lookup"><span data-stu-id="892fe-120">Name</span></span>       | <span data-ttu-id="892fe-121">说明</span><span class="sxs-lookup"><span data-stu-id="892fe-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="892fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="892fe-122">Authorization</span></span>  | <span data-ttu-id="892fe-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="892fe-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="892fe-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="892fe-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="892fe-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="892fe-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="892fe-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="892fe-128">Request body</span></span>
<span data-ttu-id="892fe-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="892fe-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="892fe-130">参数</span><span class="sxs-lookup"><span data-stu-id="892fe-130">Parameter</span></span>    | <span data-ttu-id="892fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="892fe-131">Type</span></span>   |<span data-ttu-id="892fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="892fe-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="892fe-133">Shift</span><span class="sxs-lookup"><span data-stu-id="892fe-133">shift</span></span>|<span data-ttu-id="892fe-134">string</span><span class="sxs-lookup"><span data-stu-id="892fe-134">string</span></span>|<span data-ttu-id="892fe-p106">指定移动单元格的方式。可能的值是：`Down`、`Right`。</span><span class="sxs-lookup"><span data-stu-id="892fe-p106">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="892fe-137">响应</span><span class="sxs-lookup"><span data-stu-id="892fe-137">Response</span></span>

<span data-ttu-id="892fe-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="892fe-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="892fe-139">示例</span><span class="sxs-lookup"><span data-stu-id="892fe-139">Example</span></span>
<span data-ttu-id="892fe-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="892fe-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="892fe-141">请求</span><span class="sxs-lookup"><span data-stu-id="892fe-141">Request</span></span>
<span data-ttu-id="892fe-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="892fe-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="892fe-143">响应</span><span class="sxs-lookup"><span data-stu-id="892fe-143">Response</span></span>
<span data-ttu-id="892fe-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="892fe-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-insert.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
