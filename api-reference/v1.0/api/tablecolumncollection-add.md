---
title: 'TableColumnCollection: add'
description: 向表中添加新列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 09312b06c0ba3be49e5f26b1346345017cd05095
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575894"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="3cd61-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="3cd61-103">TableColumnCollection: add</span></span>

<span data-ttu-id="3cd61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cd61-105">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="3cd61-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3cd61-106">权限</span><span class="sxs-lookup"><span data-stu-id="3cd61-106">Permissions</span></span>
<span data-ttu-id="3cd61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cd61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd61-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cd61-109">Permission type</span></span>      | <span data-ttu-id="3cd61-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cd61-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cd61-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cd61-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3cd61-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cd61-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3cd61-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cd61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cd61-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cd61-114">Not supported.</span></span>    |
|<span data-ttu-id="3cd61-115">Application</span><span class="sxs-lookup"><span data-stu-id="3cd61-115">Application</span></span> | <span data-ttu-id="3cd61-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cd61-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cd61-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cd61-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="3cd61-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cd61-118">Request headers</span></span>
| <span data-ttu-id="3cd61-119">名称</span><span class="sxs-lookup"><span data-stu-id="3cd61-119">Name</span></span>       | <span data-ttu-id="3cd61-120">说明</span><span class="sxs-lookup"><span data-stu-id="3cd61-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3cd61-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cd61-121">Authorization</span></span>  | <span data-ttu-id="3cd61-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cd61-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3cd61-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3cd61-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3cd61-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3cd61-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd61-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cd61-127">Request body</span></span>
<span data-ttu-id="3cd61-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3cd61-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3cd61-129">参数</span><span class="sxs-lookup"><span data-stu-id="3cd61-129">Parameter</span></span>    | <span data-ttu-id="3cd61-130">类型</span><span class="sxs-lookup"><span data-stu-id="3cd61-130">Type</span></span>   |<span data-ttu-id="3cd61-131">说明</span><span class="sxs-lookup"><span data-stu-id="3cd61-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cd61-132">index</span><span class="sxs-lookup"><span data-stu-id="3cd61-132">index</span></span>|<span data-ttu-id="3cd61-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3cd61-133">Int32</span></span>|<span data-ttu-id="3cd61-p104">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="3cd61-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="3cd61-138">values</span><span class="sxs-lookup"><span data-stu-id="3cd61-138">values</span></span>|<span data-ttu-id="3cd61-139">Json</span><span class="sxs-lookup"><span data-stu-id="3cd61-139">Json</span></span>|<span data-ttu-id="3cd61-p105">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="3cd61-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="3cd61-142">name</span><span class="sxs-lookup"><span data-stu-id="3cd61-142">name</span></span>|<span data-ttu-id="3cd61-143">string</span><span class="sxs-lookup"><span data-stu-id="3cd61-143">string</span></span>|<span data-ttu-id="3cd61-144">name</span><span class="sxs-lookup"><span data-stu-id="3cd61-144">name</span></span>
## <a name="response"></a><span data-ttu-id="3cd61-145">响应</span><span class="sxs-lookup"><span data-stu-id="3cd61-145">Response</span></span>

<span data-ttu-id="3cd61-146">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [WorkbookTableColumn](../resources/workbooktablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cd61-146">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd61-147">示例</span><span class="sxs-lookup"><span data-stu-id="3cd61-147">Example</span></span>
<span data-ttu-id="3cd61-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3cd61-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3cd61-149">请求</span><span class="sxs-lookup"><span data-stu-id="3cd61-149">Request</span></span>
<span data-ttu-id="3cd61-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3cd61-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cd61-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd61-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="3cd61-152">C#</span><span class="sxs-lookup"><span data-stu-id="3cd61-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cd61-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cd61-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cd61-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cd61-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cd61-155">Java</span><span class="sxs-lookup"><span data-stu-id="3cd61-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cd61-156">响应</span><span class="sxs-lookup"><span data-stu-id="3cd61-156">Response</span></span>
<span data-ttu-id="3cd61-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cd61-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": "99",
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->

