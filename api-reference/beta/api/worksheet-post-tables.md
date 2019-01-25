---
title: 创建表
description: 使用此 API 创建新的表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 649fb5848a7c30908a87d8ea643aefa19ca5623e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516369"
---
# <a name="create-table"></a><span data-ttu-id="77369-103">创建表</span><span class="sxs-lookup"><span data-stu-id="77369-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77369-104">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="77369-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="77369-105">权限</span><span class="sxs-lookup"><span data-stu-id="77369-105">Permissions</span></span>
<span data-ttu-id="77369-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77369-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77369-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77369-108">Permission type</span></span>      | <span data-ttu-id="77369-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77369-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77369-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77369-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77369-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77369-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77369-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77369-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77369-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77369-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="77369-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77369-114">Application</span></span> | <span data-ttu-id="77369-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77369-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77369-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77369-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="77369-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="77369-117">Request headers</span></span>
| <span data-ttu-id="77369-118">名称</span><span class="sxs-lookup"><span data-stu-id="77369-118">Name</span></span>       | <span data-ttu-id="77369-119">说明</span><span class="sxs-lookup"><span data-stu-id="77369-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77369-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77369-120">Authorization</span></span>  | <span data-ttu-id="77369-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77369-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77369-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="77369-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="77369-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="77369-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77369-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="77369-126">Request body</span></span>
<span data-ttu-id="77369-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="77369-127">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="77369-128">参数</span><span class="sxs-lookup"><span data-stu-id="77369-128">Parameter</span></span>       | <span data-ttu-id="77369-129">类型</span><span class="sxs-lookup"><span data-stu-id="77369-129">Type</span></span>|<span data-ttu-id="77369-130">说明</span><span class="sxs-lookup"><span data-stu-id="77369-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="77369-131">Address</span><span class="sxs-lookup"><span data-stu-id="77369-131">Address</span></span>  | <span data-ttu-id="77369-132">string</span><span class="sxs-lookup"><span data-stu-id="77369-132">string</span></span>| <span data-ttu-id="77369-p104">区域地址。如果正在从“worksheets/{id</span><span class="sxs-lookup"><span data-stu-id="77369-p104">Range address. If you are calling this API off of \`worksheets/{id</span></span>|<span data-ttu-id="77369-135">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`) 调用此 API</span><span class="sxs-lookup"><span data-stu-id="77369-135">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span></span>|
| <span data-ttu-id="77369-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="77369-136">hasHeaders</span></span>  | <span data-ttu-id="77369-137">布尔</span><span class="sxs-lookup"><span data-stu-id="77369-137">boolean</span></span>|<span data-ttu-id="77369-p105">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="77369-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="77369-141">响应</span><span class="sxs-lookup"><span data-stu-id="77369-141">Response</span></span>

<span data-ttu-id="77369-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Table](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77369-142">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77369-143">示例</span><span class="sxs-lookup"><span data-stu-id="77369-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77369-144">请求</span><span class="sxs-lookup"><span data-stu-id="77369-144">Request</span></span>
<span data-ttu-id="77369-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77369-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="77369-146">响应</span><span class="sxs-lookup"><span data-stu-id="77369-146">Response</span></span>
<span data-ttu-id="77369-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77369-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-post-tables.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
