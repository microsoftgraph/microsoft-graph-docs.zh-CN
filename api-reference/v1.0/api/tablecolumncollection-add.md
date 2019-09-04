---
title: 'TableColumnCollection: add'
description: 向表中添加新列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 6632ba9b8809500612b312cf792907586a6c6bd7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729110"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="2a0a9-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="2a0a9-103">TableColumnCollection: add</span></span>

<span data-ttu-id="2a0a9-104">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="2a0a9-105">权限</span><span class="sxs-lookup"><span data-stu-id="2a0a9-105">Permissions</span></span>
<span data-ttu-id="2a0a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a0a9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a0a9-108">Permission type</span></span>      | <span data-ttu-id="2a0a9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a0a9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a0a9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a0a9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2a0a9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a0a9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2a0a9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a0a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a0a9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-113">Not supported.</span></span>    |
|<span data-ttu-id="2a0a9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a0a9-114">Application</span></span> | <span data-ttu-id="2a0a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a0a9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a0a9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="2a0a9-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a0a9-117">Request headers</span></span>
| <span data-ttu-id="2a0a9-118">名称</span><span class="sxs-lookup"><span data-stu-id="2a0a9-118">Name</span></span>       | <span data-ttu-id="2a0a9-119">说明</span><span class="sxs-lookup"><span data-stu-id="2a0a9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2a0a9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a0a9-120">Authorization</span></span>  | <span data-ttu-id="2a0a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a0a9-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2a0a9-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2a0a9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a0a9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a0a9-126">Request body</span></span>
<span data-ttu-id="2a0a9-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a0a9-128">参数</span><span class="sxs-lookup"><span data-stu-id="2a0a9-128">Parameter</span></span>    | <span data-ttu-id="2a0a9-129">类型</span><span class="sxs-lookup"><span data-stu-id="2a0a9-129">Type</span></span>   |<span data-ttu-id="2a0a9-130">说明</span><span class="sxs-lookup"><span data-stu-id="2a0a9-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a0a9-131">index</span><span class="sxs-lookup"><span data-stu-id="2a0a9-131">index</span></span>|<span data-ttu-id="2a0a9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="2a0a9-132">Int32</span></span>|<span data-ttu-id="2a0a9-p104">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="2a0a9-137">values</span><span class="sxs-lookup"><span data-stu-id="2a0a9-137">values</span></span>|<span data-ttu-id="2a0a9-138">Json</span><span class="sxs-lookup"><span data-stu-id="2a0a9-138">Json</span></span>|<span data-ttu-id="2a0a9-p105">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="2a0a9-141">name</span><span class="sxs-lookup"><span data-stu-id="2a0a9-141">name</span></span>|<span data-ttu-id="2a0a9-142">string</span><span class="sxs-lookup"><span data-stu-id="2a0a9-142">string</span></span>|<span data-ttu-id="2a0a9-143">name</span><span class="sxs-lookup"><span data-stu-id="2a0a9-143">name</span></span>
## <a name="response"></a><span data-ttu-id="2a0a9-144">响应</span><span class="sxs-lookup"><span data-stu-id="2a0a9-144">Response</span></span>

<span data-ttu-id="2a0a9-145">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[WorkbookTableColumn](../resources/workbooktablecolumn.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-145">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a0a9-146">示例</span><span class="sxs-lookup"><span data-stu-id="2a0a9-146">Example</span></span>
<span data-ttu-id="2a0a9-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2a0a9-148">请求</span><span class="sxs-lookup"><span data-stu-id="2a0a9-148">Request</span></span>
<span data-ttu-id="2a0a9-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2a0a9-150">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2a0a9-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a0a9-151">C#</span><span class="sxs-lookup"><span data-stu-id="2a0a9-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a0a9-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a0a9-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a0a9-153">目标-C</span><span class="sxs-lookup"><span data-stu-id="2a0a9-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2a0a9-154">Java</span><span class="sxs-lookup"><span data-stu-id="2a0a9-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablecolumncollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a0a9-155">响应</span><span class="sxs-lookup"><span data-stu-id="2a0a9-155">Response</span></span>
<span data-ttu-id="2a0a9-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a0a9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": 99,
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
