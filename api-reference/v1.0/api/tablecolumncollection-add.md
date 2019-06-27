---
title: 'TableColumnCollection: add'
description: 向表中添加新列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2eced50021770194ff80518632f686faf502099f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278804"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="fd2ae-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="fd2ae-103">TableColumnCollection: add</span></span>

<span data-ttu-id="fd2ae-104">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd2ae-105">权限</span><span class="sxs-lookup"><span data-stu-id="fd2ae-105">Permissions</span></span>
<span data-ttu-id="fd2ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd2ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd2ae-108">Permission type</span></span>      | <span data-ttu-id="fd2ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd2ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd2ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd2ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd2ae-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd2ae-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fd2ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd2ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd2ae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-113">Not supported.</span></span>    |
|<span data-ttu-id="fd2ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd2ae-114">Application</span></span> | <span data-ttu-id="fd2ae-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd2ae-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd2ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="fd2ae-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd2ae-117">Request headers</span></span>
| <span data-ttu-id="fd2ae-118">名称</span><span class="sxs-lookup"><span data-stu-id="fd2ae-118">Name</span></span>       | <span data-ttu-id="fd2ae-119">说明</span><span class="sxs-lookup"><span data-stu-id="fd2ae-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd2ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd2ae-120">Authorization</span></span>  | <span data-ttu-id="fd2ae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd2ae-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fd2ae-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="fd2ae-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd2ae-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd2ae-126">Request body</span></span>
<span data-ttu-id="fd2ae-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fd2ae-128">参数</span><span class="sxs-lookup"><span data-stu-id="fd2ae-128">Parameter</span></span>    | <span data-ttu-id="fd2ae-129">类型</span><span class="sxs-lookup"><span data-stu-id="fd2ae-129">Type</span></span>   |<span data-ttu-id="fd2ae-130">说明</span><span class="sxs-lookup"><span data-stu-id="fd2ae-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd2ae-131">index</span><span class="sxs-lookup"><span data-stu-id="fd2ae-131">index</span></span>|<span data-ttu-id="fd2ae-132">Int32</span><span class="sxs-lookup"><span data-stu-id="fd2ae-132">Int32</span></span>|<span data-ttu-id="fd2ae-p104">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="fd2ae-137">values</span><span class="sxs-lookup"><span data-stu-id="fd2ae-137">values</span></span>|<span data-ttu-id="fd2ae-138">Json</span><span class="sxs-lookup"><span data-stu-id="fd2ae-138">Json</span></span>|<span data-ttu-id="fd2ae-p105">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="fd2ae-141">name</span><span class="sxs-lookup"><span data-stu-id="fd2ae-141">name</span></span>|<span data-ttu-id="fd2ae-142">string</span><span class="sxs-lookup"><span data-stu-id="fd2ae-142">string</span></span>|<span data-ttu-id="fd2ae-143">name</span><span class="sxs-lookup"><span data-stu-id="fd2ae-143">name</span></span>
## <a name="response"></a><span data-ttu-id="fd2ae-144">响应</span><span class="sxs-lookup"><span data-stu-id="fd2ae-144">Response</span></span>

<span data-ttu-id="fd2ae-145">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[WorkbookTableColumn](../resources/tablecolumn.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-145">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd2ae-146">示例</span><span class="sxs-lookup"><span data-stu-id="fd2ae-146">Example</span></span>
<span data-ttu-id="fd2ae-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd2ae-148">请求</span><span class="sxs-lookup"><span data-stu-id="fd2ae-148">Request</span></span>
<span data-ttu-id="fd2ae-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-149">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="fd2ae-150">响应</span><span class="sxs-lookup"><span data-stu-id="fd2ae-150">Response</span></span>
<span data-ttu-id="fd2ae-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd2ae-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd2ae-154">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fd2ae-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd2ae-155">C#</span><span class="sxs-lookup"><span data-stu-id="fd2ae-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd2ae-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="fd2ae-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fd2ae-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="fd2ae-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/tablecolumncollection_add-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Warning: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
