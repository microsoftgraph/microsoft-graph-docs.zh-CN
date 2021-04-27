---
title: 'TableRowCollection: add'
description: '将行添加到表的末尾。 请注意，API 可以使用此 API 接受多行数据。 一次添加一行可能会导致性能下降。 建议的方法是在单个调用中一起批处理行，而不是执行单行插入。 为了获得最佳结果，请收集应用程序端要插入的行并执行单行添加操作。 试验行数以确定在单个 API 调用中要使用的理想行数。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 55b34694abea4200c9801acd60ca5efed77b7935
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054789"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="f152f-108">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="f152f-108">TableRowCollection: add</span></span>

<span data-ttu-id="f152f-109">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f152f-109">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f152f-110">将行添加到表的末尾。</span><span class="sxs-lookup"><span data-stu-id="f152f-110">Adds rows to the end of the table.</span></span> <span data-ttu-id="f152f-111">请注意，API 可以使用此 API 接受多行数据。</span><span class="sxs-lookup"><span data-stu-id="f152f-111">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="f152f-112">一次添加一行可能会导致性能下降。</span><span class="sxs-lookup"><span data-stu-id="f152f-112">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="f152f-113">建议的方法是在单个调用中一起批处理行，而不是执行单行插入。</span><span class="sxs-lookup"><span data-stu-id="f152f-113">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="f152f-114">为了获得最佳结果，请收集应用程序端要插入的行并执行单行添加操作。</span><span class="sxs-lookup"><span data-stu-id="f152f-114">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="f152f-115">试验行数以确定在单个 API 调用中要使用的理想行数。</span><span class="sxs-lookup"><span data-stu-id="f152f-115">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="f152f-116">错误处理</span><span class="sxs-lookup"><span data-stu-id="f152f-116">Error Handling</span></span>

<span data-ttu-id="f152f-117">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="f152f-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="f152f-118">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="f152f-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="f152f-119">权限</span><span class="sxs-lookup"><span data-stu-id="f152f-119">Permissions</span></span>
<span data-ttu-id="f152f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f152f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f152f-122">权限类型</span><span class="sxs-lookup"><span data-stu-id="f152f-122">Permission type</span></span>      | <span data-ttu-id="f152f-123">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f152f-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f152f-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f152f-124">Delegated (work or school account)</span></span> | <span data-ttu-id="f152f-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f152f-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f152f-126">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f152f-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f152f-127">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f152f-127">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f152f-128">应用程序</span><span class="sxs-lookup"><span data-stu-id="f152f-128">Application</span></span> | <span data-ttu-id="f152f-129">不支持。</span><span class="sxs-lookup"><span data-stu-id="f152f-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f152f-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f152f-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/rows/add
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/rows/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="f152f-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="f152f-131">Request headers</span></span>
| <span data-ttu-id="f152f-132">名称</span><span class="sxs-lookup"><span data-stu-id="f152f-132">Name</span></span>       | <span data-ttu-id="f152f-133">说明</span><span class="sxs-lookup"><span data-stu-id="f152f-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f152f-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f152f-134">Authorization</span></span>  | <span data-ttu-id="f152f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f152f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f152f-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f152f-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="f152f-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f152f-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f152f-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="f152f-140">Request body</span></span>
<span data-ttu-id="f152f-141">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f152f-141">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f152f-142">参数</span><span class="sxs-lookup"><span data-stu-id="f152f-142">Parameter</span></span>    | <span data-ttu-id="f152f-143">类型</span><span class="sxs-lookup"><span data-stu-id="f152f-143">Type</span></span>   |<span data-ttu-id="f152f-144">说明</span><span class="sxs-lookup"><span data-stu-id="f152f-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f152f-145">index</span><span class="sxs-lookup"><span data-stu-id="f152f-145">index</span></span>|<span data-ttu-id="f152f-146">number</span><span class="sxs-lookup"><span data-stu-id="f152f-146">number</span></span>|<span data-ttu-id="f152f-p107">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="f152f-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="f152f-152">值</span><span class="sxs-lookup"><span data-stu-id="f152f-152">values</span></span>|<span data-ttu-id="f152f-153"> (布尔值、字符串或数字) 集合</span><span class="sxs-lookup"><span data-stu-id="f152f-153">(boolean or string or number) collection</span></span>|<span data-ttu-id="f152f-154">可选。</span><span class="sxs-lookup"><span data-stu-id="f152f-154">Optional.</span></span> <span data-ttu-id="f152f-155">表格行的无格式值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="f152f-155">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="f152f-156">响应</span><span class="sxs-lookup"><span data-stu-id="f152f-156">Response</span></span>

<span data-ttu-id="f152f-157">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [workbookTableRow](../resources/workbooktablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f152f-157">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f152f-158">示例</span><span class="sxs-lookup"><span data-stu-id="f152f-158">Example</span></span>
<span data-ttu-id="f152f-159">本示例在表格末尾插入两行数据。</span><span class="sxs-lookup"><span data-stu-id="f152f-159">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="f152f-160">请求</span><span class="sxs-lookup"><span data-stu-id="f152f-160">Request</span></span>
<span data-ttu-id="f152f-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f152f-161">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f152f-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="f152f-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add_2"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": null,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="f152f-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f152f-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f152f-164">C#</span><span class="sxs-lookup"><span data-stu-id="f152f-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerowcollection-add-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f152f-165">响应</span><span class="sxs-lookup"><span data-stu-id="f152f-165">Response</span></span>
<span data-ttu-id="f152f-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f152f-166">Here is an example of the response.</span></span> <span data-ttu-id="f152f-167">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f152f-167">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


