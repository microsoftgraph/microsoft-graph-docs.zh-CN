---
title: 创建 TableRow
description: '将行添加到表的末尾。 请注意, API 可以使用此 API 接受多行数据。 一次添加一行可能会导致性能下降。 建议的方法是将行在单个调用中进行批处理, 而不是执行单个行插入。 为获得最佳结果, 请收集要插入到应用程序中的行, 并执行单行添加操作。 试验行数, 以确定要在单个 API 调用中使用的理想行数。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 187a5e9028515a7e6450f4bc0e4930837d4be15f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458008"
---
# <a name="create-tablerow"></a><span data-ttu-id="96f88-108">创建 TableRow</span><span class="sxs-lookup"><span data-stu-id="96f88-108">Create TableRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96f88-109">将行添加到表的末尾。</span><span class="sxs-lookup"><span data-stu-id="96f88-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="96f88-110">请注意, API 可以使用此 API 接受多行数据。</span><span class="sxs-lookup"><span data-stu-id="96f88-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="96f88-111">一次添加一行可能会导致性能下降。</span><span class="sxs-lookup"><span data-stu-id="96f88-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="96f88-112">建议的方法是将行在单个调用中进行批处理, 而不是执行单个行插入。</span><span class="sxs-lookup"><span data-stu-id="96f88-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="96f88-113">为获得最佳结果, 请收集要插入到应用程序中的行, 并执行单行添加操作。</span><span class="sxs-lookup"><span data-stu-id="96f88-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="96f88-114">试验行数, 以确定要在单个 API 调用中使用的理想行数。</span><span class="sxs-lookup"><span data-stu-id="96f88-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="96f88-115">错误处理</span><span class="sxs-lookup"><span data-stu-id="96f88-115">Error Handling</span></span>

<span data-ttu-id="96f88-116">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="96f88-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="96f88-117">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="96f88-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="96f88-118">权限</span><span class="sxs-lookup"><span data-stu-id="96f88-118">Permissions</span></span>
<span data-ttu-id="96f88-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96f88-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96f88-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="96f88-121">Permission type</span></span>      | <span data-ttu-id="96f88-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96f88-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96f88-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96f88-123">Delegated (work or school account)</span></span> | <span data-ttu-id="96f88-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96f88-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="96f88-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96f88-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96f88-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="96f88-126">Not supported.</span></span>    |
|<span data-ttu-id="96f88-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="96f88-127">Application</span></span> | <span data-ttu-id="96f88-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="96f88-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96f88-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96f88-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="96f88-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="96f88-130">Request headers</span></span>
| <span data-ttu-id="96f88-131">名称</span><span class="sxs-lookup"><span data-stu-id="96f88-131">Name</span></span>       | <span data-ttu-id="96f88-132">说明</span><span class="sxs-lookup"><span data-stu-id="96f88-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96f88-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="96f88-133">Authorization</span></span>  | <span data-ttu-id="96f88-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96f88-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96f88-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96f88-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="96f88-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="96f88-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96f88-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="96f88-139">Request body</span></span>
<span data-ttu-id="96f88-140">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="96f88-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96f88-141">参数</span><span class="sxs-lookup"><span data-stu-id="96f88-141">Parameter</span></span>    | <span data-ttu-id="96f88-142">类型</span><span class="sxs-lookup"><span data-stu-id="96f88-142">Type</span></span>   |<span data-ttu-id="96f88-143">说明</span><span class="sxs-lookup"><span data-stu-id="96f88-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96f88-144">index</span><span class="sxs-lookup"><span data-stu-id="96f88-144">index</span></span>|<span data-ttu-id="96f88-145">number</span><span class="sxs-lookup"><span data-stu-id="96f88-145">number</span></span>|<span data-ttu-id="96f88-p107">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="96f88-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="96f88-151">值</span><span class="sxs-lookup"><span data-stu-id="96f88-151">values</span></span>|<span data-ttu-id="96f88-152">(布尔值或字符串或数字) 集合</span><span class="sxs-lookup"><span data-stu-id="96f88-152">(boolean or string or number) collection</span></span>|<span data-ttu-id="96f88-153">表格行无格式值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="96f88-153">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="96f88-154">响应</span><span class="sxs-lookup"><span data-stu-id="96f88-154">Response</span></span>

<span data-ttu-id="96f88-155">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[workbookTableRow](../resources/workbooktablerow.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96f88-155">If successful, this method returns `200 OK` response code and [workbookTableRow](../resources/workbooktablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f88-156">示例</span><span class="sxs-lookup"><span data-stu-id="96f88-156">Example</span></span>
<span data-ttu-id="96f88-157">在此示例中, 将两行数据插入到表的末尾。</span><span class="sxs-lookup"><span data-stu-id="96f88-157">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="96f88-158">请求</span><span class="sxs-lookup"><span data-stu-id="96f88-158">Request</span></span>
<span data-ttu-id="96f88-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96f88-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96f88-160">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="96f88-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96f88-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="96f88-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="96f88-162">响应</span><span class="sxs-lookup"><span data-stu-id="96f88-162">Response</span></span>
<span data-ttu-id="96f88-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96f88-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
