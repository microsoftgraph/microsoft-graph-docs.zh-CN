---
title: 创建表
description: 使用此 API 创建新的表。
ms.openlocfilehash: 49c0beac13fc40f10eb5c2b44f405d23885bcb38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008770"
---
# <a name="create-table"></a><span data-ttu-id="3ec13-103">创建表</span><span class="sxs-lookup"><span data-stu-id="3ec13-103">Create table</span></span>

<span data-ttu-id="3ec13-104">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="3ec13-104">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ec13-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ec13-105">Permissions</span></span>
<span data-ttu-id="3ec13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ec13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ec13-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ec13-108">Permission type</span></span>      | <span data-ttu-id="3ec13-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ec13-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ec13-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec13-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ec13-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ec13-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3ec13-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ec13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ec13-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec13-113">Not supported.</span></span>    |
|<span data-ttu-id="3ec13-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ec13-114">Application</span></span> | <span data-ttu-id="3ec13-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ec13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ec13-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ec13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="3ec13-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ec13-117">Request headers</span></span>
| <span data-ttu-id="3ec13-118">名称</span><span class="sxs-lookup"><span data-stu-id="3ec13-118">Name</span></span>       | <span data-ttu-id="3ec13-119">说明</span><span class="sxs-lookup"><span data-stu-id="3ec13-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3ec13-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ec13-120">Authorization</span></span>  | <span data-ttu-id="3ec13-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ec13-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ec13-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3ec13-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3ec13-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3ec13-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ec13-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ec13-126">Request body</span></span>
<span data-ttu-id="3ec13-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3ec13-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ec13-128">参数</span><span class="sxs-lookup"><span data-stu-id="3ec13-128">Parameter</span></span>           | <span data-ttu-id="3ec13-129">类型</span><span class="sxs-lookup"><span data-stu-id="3ec13-129">Type</span></span>      |<span data-ttu-id="3ec13-130">说明</span><span class="sxs-lookup"><span data-stu-id="3ec13-130">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="3ec13-131">Address</span><span class="sxs-lookup"><span data-stu-id="3ec13-131">Address</span></span>  | <span data-ttu-id="3ec13-132">string</span><span class="sxs-lookup"><span data-stu-id="3ec13-132">string</span></span>| <span data-ttu-id="3ec13-p104">区域地址。若要从 `worksheets/{id or name}/tables/add` 路径调用此 API，地址中无需有工作表名称前缀。不过，若要从 `workbook/tables/add` 路径调用此 API，请提供需要在其中创建表的工作表名称（例如：`sheet1!A1:D4`）</span><span class="sxs-lookup"><span data-stu-id="3ec13-p104">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="3ec13-136">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="3ec13-136">hasHeaders</span></span>  | <span data-ttu-id="3ec13-137">boolean</span><span class="sxs-lookup"><span data-stu-id="3ec13-137">boolean</span></span>|<span data-ttu-id="3ec13-p105">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="3ec13-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="3ec13-141">响应</span><span class="sxs-lookup"><span data-stu-id="3ec13-141">Response</span></span>

<span data-ttu-id="3ec13-142">如果成功，此方法返回`201 Created`响应代码和[WorkbookTable](../resources/table.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="3ec13-142">If successful, this method returns `201 Created` response code and [WorkbookTable](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ec13-143">示例</span><span class="sxs-lookup"><span data-stu-id="3ec13-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ec13-144">请求</span><span class="sxs-lookup"><span data-stu-id="3ec13-144">Request</span></span>
<span data-ttu-id="3ec13-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ec13-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id}/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="3ec13-146">响应</span><span class="sxs-lookup"><span data-stu-id="3ec13-146">Response</span></span>
<span data-ttu-id="3ec13-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ec13-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
