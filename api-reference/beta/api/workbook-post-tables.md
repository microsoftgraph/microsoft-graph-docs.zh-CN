---
title: 创建表
description: 使用此 API 创建新的表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 67f34a0310fcfd0ba6641eeecbbb8c3e6fc2a05f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643634"
---
# <a name="create-table"></a><span data-ttu-id="0e8be-103">创建表</span><span class="sxs-lookup"><span data-stu-id="0e8be-103">Create table</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e8be-104">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="0e8be-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e8be-105">权限</span><span class="sxs-lookup"><span data-stu-id="0e8be-105">Permissions</span></span>
<span data-ttu-id="0e8be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e8be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e8be-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e8be-108">Permission type</span></span>      | <span data-ttu-id="0e8be-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e8be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e8be-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e8be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e8be-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e8be-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e8be-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e8be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e8be-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e8be-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e8be-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e8be-114">Application</span></span> | <span data-ttu-id="0e8be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e8be-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e8be-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e8be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="0e8be-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e8be-117">Request headers</span></span>
| <span data-ttu-id="0e8be-118">名称</span><span class="sxs-lookup"><span data-stu-id="0e8be-118">Name</span></span>       | <span data-ttu-id="0e8be-119">说明</span><span class="sxs-lookup"><span data-stu-id="0e8be-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e8be-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e8be-120">Authorization</span></span>  | <span data-ttu-id="0e8be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e8be-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e8be-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e8be-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e8be-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0e8be-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e8be-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e8be-126">Request body</span></span>
<span data-ttu-id="0e8be-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0e8be-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e8be-128">参数</span><span class="sxs-lookup"><span data-stu-id="0e8be-128">Parameter</span></span>           | <span data-ttu-id="0e8be-129">类型</span><span class="sxs-lookup"><span data-stu-id="0e8be-129">Type</span></span>      |<span data-ttu-id="0e8be-130">说明</span><span class="sxs-lookup"><span data-stu-id="0e8be-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="0e8be-131">Address</span><span class="sxs-lookup"><span data-stu-id="0e8be-131">Address</span></span>  | <span data-ttu-id="0e8be-132">string</span><span class="sxs-lookup"><span data-stu-id="0e8be-132">string</span></span>| <span data-ttu-id="0e8be-p104">区域地址。若要从 `worksheets/{id or name}/tables/add` 路径调用此 API，地址中无需有工作表名称前缀。不过，若要从 `workbook/tables/add` 路径调用此 API，请提供需要在其中创建表的工作表名称（例如：`sheet1!A1:D4`）</span><span class="sxs-lookup"><span data-stu-id="0e8be-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="0e8be-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="0e8be-136">hasHeaders</span></span>  | <span data-ttu-id="0e8be-137">boolean</span><span class="sxs-lookup"><span data-stu-id="0e8be-137">boolean</span></span>|<span data-ttu-id="0e8be-p105">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="0e8be-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="0e8be-141">响应</span><span class="sxs-lookup"><span data-stu-id="0e8be-141">Response</span></span>

<span data-ttu-id="0e8be-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Table](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e8be-142">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e8be-143">示例</span><span class="sxs-lookup"><span data-stu-id="0e8be-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e8be-144">请求</span><span class="sxs-lookup"><span data-stu-id="0e8be-144">Request</span></span>
<span data-ttu-id="0e8be-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e8be-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="0e8be-146">响应</span><span class="sxs-lookup"><span data-stu-id="0e8be-146">Response</span></span>
<span data-ttu-id="0e8be-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e8be-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/workbook-post-tables.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
