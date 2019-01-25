---
title: 'TableColumnCollection: add'
description: 向表中添加新列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1f3e2b5cacb3bb7ab462cc127b9cbc2e3b85019f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529108"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="39741-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="39741-103">TableColumnCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39741-104">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="39741-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="39741-105">权限</span><span class="sxs-lookup"><span data-stu-id="39741-105">Permissions</span></span>
<span data-ttu-id="39741-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39741-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="39741-108">Permission type</span></span>      | <span data-ttu-id="39741-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39741-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39741-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39741-110">Delegated (work or school account)</span></span> | <span data-ttu-id="39741-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39741-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39741-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39741-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39741-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39741-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39741-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="39741-114">Application</span></span> | <span data-ttu-id="39741-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="39741-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39741-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39741-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="39741-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="39741-117">Request headers</span></span>
| <span data-ttu-id="39741-118">名称</span><span class="sxs-lookup"><span data-stu-id="39741-118">Name</span></span>       | <span data-ttu-id="39741-119">说明</span><span class="sxs-lookup"><span data-stu-id="39741-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39741-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="39741-120">Authorization</span></span>  | <span data-ttu-id="39741-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39741-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39741-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="39741-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="39741-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="39741-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39741-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="39741-126">Request body</span></span>
<span data-ttu-id="39741-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="39741-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="39741-128">参数</span><span class="sxs-lookup"><span data-stu-id="39741-128">Parameter</span></span>    | <span data-ttu-id="39741-129">类型</span><span class="sxs-lookup"><span data-stu-id="39741-129">Type</span></span>   |<span data-ttu-id="39741-130">说明</span><span class="sxs-lookup"><span data-stu-id="39741-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39741-131">index</span><span class="sxs-lookup"><span data-stu-id="39741-131">index</span></span>|<span data-ttu-id="39741-132">number</span><span class="sxs-lookup"><span data-stu-id="39741-132">number</span></span>|<span data-ttu-id="39741-p104">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="39741-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="39741-137">values</span><span class="sxs-lookup"><span data-stu-id="39741-137">values</span></span>|<span data-ttu-id="39741-138">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="39741-138">(boolean or string or number)</span></span>|<span data-ttu-id="39741-p105">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="39741-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="39741-141">响应</span><span class="sxs-lookup"><span data-stu-id="39741-141">Response</span></span>

<span data-ttu-id="39741-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39741-142">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39741-143">示例</span><span class="sxs-lookup"><span data-stu-id="39741-143">Example</span></span>
<span data-ttu-id="39741-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="39741-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="39741-145">请求</span><span class="sxs-lookup"><span data-stu-id="39741-145">Request</span></span>
<span data-ttu-id="39741-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39741-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="39741-147">响应</span><span class="sxs-lookup"><span data-stu-id="39741-147">Response</span></span>
<span data-ttu-id="39741-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39741-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tablecolumncollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
