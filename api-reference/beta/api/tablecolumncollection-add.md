---
title: 'TableColumnCollection: add'
description: 向表中添加新列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 96b228b9e5f5b0aeeedaa87abdc18f8f2d94120a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027501"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="53f59-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="53f59-103">TableColumnCollection: add</span></span>

<span data-ttu-id="53f59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53f59-105">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="53f59-105">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="53f59-106">权限</span><span class="sxs-lookup"><span data-stu-id="53f59-106">Permissions</span></span>
<span data-ttu-id="53f59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53f59-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53f59-109">Permission type</span></span>      | <span data-ttu-id="53f59-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53f59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53f59-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53f59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53f59-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53f59-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53f59-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53f59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53f59-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53f59-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53f59-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53f59-115">Application</span></span> | <span data-ttu-id="53f59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53f59-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53f59-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53f59-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="53f59-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="53f59-118">Request headers</span></span>
| <span data-ttu-id="53f59-119">名称</span><span class="sxs-lookup"><span data-stu-id="53f59-119">Name</span></span>       | <span data-ttu-id="53f59-120">说明</span><span class="sxs-lookup"><span data-stu-id="53f59-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53f59-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53f59-121">Authorization</span></span>  | <span data-ttu-id="53f59-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53f59-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53f59-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53f59-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="53f59-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="53f59-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53f59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53f59-127">Request body</span></span>
<span data-ttu-id="53f59-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="53f59-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53f59-129">参数</span><span class="sxs-lookup"><span data-stu-id="53f59-129">Parameter</span></span>    | <span data-ttu-id="53f59-130">类型</span><span class="sxs-lookup"><span data-stu-id="53f59-130">Type</span></span>   |<span data-ttu-id="53f59-131">说明</span><span class="sxs-lookup"><span data-stu-id="53f59-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53f59-132">index</span><span class="sxs-lookup"><span data-stu-id="53f59-132">index</span></span>|<span data-ttu-id="53f59-133">number</span><span class="sxs-lookup"><span data-stu-id="53f59-133">number</span></span>|<span data-ttu-id="53f59-p104">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="53f59-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="53f59-138">值</span><span class="sxs-lookup"><span data-stu-id="53f59-138">values</span></span>|<span data-ttu-id="53f59-139"> () 集合中的布尔值或字符串或数字</span><span class="sxs-lookup"><span data-stu-id="53f59-139">(boolean or string or number) collection</span></span>|<span data-ttu-id="53f59-p105">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="53f59-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="53f59-142">响应</span><span class="sxs-lookup"><span data-stu-id="53f59-142">Response</span></span>

<span data-ttu-id="53f59-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookTableColumn](../resources/workbooktablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53f59-143">If successful, this method returns `200 OK` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53f59-144">示例</span><span class="sxs-lookup"><span data-stu-id="53f59-144">Example</span></span>
<span data-ttu-id="53f59-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="53f59-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53f59-146">请求</span><span class="sxs-lookup"><span data-stu-id="53f59-146">Request</span></span>
<span data-ttu-id="53f59-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53f59-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53f59-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="53f59-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="53f59-149">C#</span><span class="sxs-lookup"><span data-stu-id="53f59-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53f59-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53f59-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53f59-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53f59-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53f59-152">响应</span><span class="sxs-lookup"><span data-stu-id="53f59-152">Response</span></span>
<span data-ttu-id="53f59-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53f59-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


