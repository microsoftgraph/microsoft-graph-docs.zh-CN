---
title: 创建表
description: 使用此 API 创建新的表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f4bb3dfd7433a5bced3e105ac63b7865984c52a5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977247"
---
# <a name="create-table"></a><span data-ttu-id="67687-103">创建表</span><span class="sxs-lookup"><span data-stu-id="67687-103">Create table</span></span>

<span data-ttu-id="67687-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67687-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67687-105">使用此 API 创建新的表。</span><span class="sxs-lookup"><span data-stu-id="67687-105">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="67687-106">权限</span><span class="sxs-lookup"><span data-stu-id="67687-106">Permissions</span></span>
<span data-ttu-id="67687-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67687-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="67687-109">Permission type</span></span>      | <span data-ttu-id="67687-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67687-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67687-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67687-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67687-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67687-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67687-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67687-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67687-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67687-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="67687-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="67687-115">Application</span></span> | <span data-ttu-id="67687-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67687-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67687-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67687-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="67687-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="67687-118">Request headers</span></span>
| <span data-ttu-id="67687-119">名称</span><span class="sxs-lookup"><span data-stu-id="67687-119">Name</span></span>       | <span data-ttu-id="67687-120">说明</span><span class="sxs-lookup"><span data-stu-id="67687-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67687-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67687-121">Authorization</span></span>  | <span data-ttu-id="67687-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67687-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67687-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="67687-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="67687-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="67687-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67687-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="67687-127">Request body</span></span>
<span data-ttu-id="67687-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="67687-128">In the request body, provide a JSON object with the following parameters.</span></span> 

| <span data-ttu-id="67687-129">参数</span><span class="sxs-lookup"><span data-stu-id="67687-129">Parameter</span></span>       | <span data-ttu-id="67687-130">类型</span><span class="sxs-lookup"><span data-stu-id="67687-130">Type</span></span>|<span data-ttu-id="67687-131">说明</span><span class="sxs-lookup"><span data-stu-id="67687-131">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="67687-132">Address</span><span class="sxs-lookup"><span data-stu-id="67687-132">Address</span></span>  | <span data-ttu-id="67687-133">string</span><span class="sxs-lookup"><span data-stu-id="67687-133">string</span></span>| <span data-ttu-id="67687-134">区域地址。</span><span class="sxs-lookup"><span data-stu-id="67687-134">Range address.</span></span> <span data-ttu-id="67687-135">如果要从路径调用此 API `worksheets/{id|name}/tables/add` ，则无需支持地址中的工作表名称前缀。</span><span class="sxs-lookup"><span data-stu-id="67687-135">If you are calling this API off of `worksheets/{id|name}/tables/add` path, there is no need to support the sheet name prefix in the address.</span></span> <span data-ttu-id="67687-136">但是，如果要调用此 `workbook/tables/add` 路径 off，请提供需要在其上创建表的工作表名称 (例如： `sheet1!A1:D4`) </span><span class="sxs-lookup"><span data-stu-id="67687-136">However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="67687-137">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="67687-137">hasHeaders</span></span>  | <span data-ttu-id="67687-138">布尔</span><span class="sxs-lookup"><span data-stu-id="67687-138">boolean</span></span>|<span data-ttu-id="67687-p105">指示区域是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="67687-p105">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="67687-142">响应</span><span class="sxs-lookup"><span data-stu-id="67687-142">Response</span></span>

<span data-ttu-id="67687-143">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [workbookTable](../resources/workbooktable.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67687-143">If successful, this method returns `201 Created` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67687-144">示例</span><span class="sxs-lookup"><span data-stu-id="67687-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67687-145">请求</span><span class="sxs-lookup"><span data-stu-id="67687-145">Request</span></span>
<span data-ttu-id="67687-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67687-146">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67687-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="67687-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="67687-148">C#</span><span class="sxs-lookup"><span data-stu-id="67687-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-table-from-worksheet-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67687-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67687-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-table-from-worksheet-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67687-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67687-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-table-from-worksheet-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67687-151">Java</span><span class="sxs-lookup"><span data-stu-id="67687-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-table-from-worksheet-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67687-152">响应</span><span class="sxs-lookup"><span data-stu-id="67687-152">Response</span></span>
<span data-ttu-id="67687-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67687-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


