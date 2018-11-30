---
title: 创建表
description: 使用此 API 创建新的表。
ms.openlocfilehash: a56091ca2ed5e3bad69b3d618fe760db5b350c9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046077"
---
# <a name="create-table"></a><span data-ttu-id="a26a9-103">创建表</span><span class="sxs-lookup"><span data-stu-id="a26a9-103">Create table</span></span>

> <span data-ttu-id="a26a9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a26a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a26a9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a26a9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a26a9-106">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="a26a9-106">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="a26a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="a26a9-107">Permissions</span></span>
<span data-ttu-id="a26a9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a26a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a26a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a26a9-110">Permission type</span></span>      | <span data-ttu-id="a26a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a26a9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a26a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a26a9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a26a9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a26a9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a26a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a26a9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a26a9-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a26a9-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a26a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a26a9-116">Application</span></span> | <span data-ttu-id="a26a9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a26a9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a26a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a26a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="a26a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a26a9-119">Request headers</span></span>
| <span data-ttu-id="a26a9-120">名称</span><span class="sxs-lookup"><span data-stu-id="a26a9-120">Name</span></span>       | <span data-ttu-id="a26a9-121">说明</span><span class="sxs-lookup"><span data-stu-id="a26a9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a26a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a26a9-122">Authorization</span></span>  | <span data-ttu-id="a26a9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a26a9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a26a9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a26a9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a26a9-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a26a9-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a26a9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a26a9-128">Request body</span></span>
<span data-ttu-id="a26a9-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a26a9-129">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="a26a9-130">参数</span><span class="sxs-lookup"><span data-stu-id="a26a9-130">Parameter</span></span>       | <span data-ttu-id="a26a9-131">类型</span><span class="sxs-lookup"><span data-stu-id="a26a9-131">Type</span></span>|<span data-ttu-id="a26a9-132">说明</span><span class="sxs-lookup"><span data-stu-id="a26a9-132">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="a26a9-133">Address</span><span class="sxs-lookup"><span data-stu-id="a26a9-133">Address</span></span>  | <span data-ttu-id="a26a9-134">string</span><span class="sxs-lookup"><span data-stu-id="a26a9-134">string</span></span>| <span data-ttu-id="a26a9-p105">区域地址。如果正在从“worksheets/{id</span><span class="sxs-lookup"><span data-stu-id="a26a9-p105">Range address. If you are calling this API off of \`worksheets/{id</span></span>|<span data-ttu-id="a26a9-137">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`) 调用此 API</span><span class="sxs-lookup"><span data-stu-id="a26a9-137">name}/tables/add` path, there is no need to support the sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4\`)</span></span>|
| <span data-ttu-id="a26a9-138">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="a26a9-138">hasHeaders</span></span>  | <span data-ttu-id="a26a9-139">boolean</span><span class="sxs-lookup"><span data-stu-id="a26a9-139">boolean</span></span>|<span data-ttu-id="a26a9-p106">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="a26a9-p106">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="a26a9-143">响应</span><span class="sxs-lookup"><span data-stu-id="a26a9-143">Response</span></span>

<span data-ttu-id="a26a9-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [Table](../resources/table.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a26a9-144">If successful, this method returns `201 Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a26a9-145">示例</span><span class="sxs-lookup"><span data-stu-id="a26a9-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a26a9-146">请求</span><span class="sxs-lookup"><span data-stu-id="a26a9-146">Request</span></span>
<span data-ttu-id="a26a9-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a26a9-147">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a26a9-148">响应</span><span class="sxs-lookup"><span data-stu-id="a26a9-148">Response</span></span>
<span data-ttu-id="a26a9-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a26a9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
