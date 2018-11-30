---
title: 'TableRowCollection: add'
description: '向表末尾的行。 请注意 API 可以接受使用此 API 的多个行数据。 一次添加一个行可能导致性能下降。 建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。 为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。 试验要确定的理想要使用一个 API 调用中的行数的行数。 '
ms.openlocfilehash: fc2b89a25ade4b9d85844716370d95d52689de9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009149"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="a8c41-108">TableRowCollection: add</span><span class="sxs-lookup"><span data-stu-id="a8c41-108">TableRowCollection: add</span></span>

<span data-ttu-id="a8c41-109">向表末尾的行。</span><span class="sxs-lookup"><span data-stu-id="a8c41-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="a8c41-110">请注意 API 可以接受使用此 API 的多个行数据。</span><span class="sxs-lookup"><span data-stu-id="a8c41-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="a8c41-111">一次添加一个行可能导致性能下降。</span><span class="sxs-lookup"><span data-stu-id="a8c41-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="a8c41-112">建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。</span><span class="sxs-lookup"><span data-stu-id="a8c41-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="a8c41-113">为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。</span><span class="sxs-lookup"><span data-stu-id="a8c41-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="a8c41-114">试验要确定的理想要使用一个 API 调用中的行数的行数。</span><span class="sxs-lookup"><span data-stu-id="a8c41-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="a8c41-115">错误处理</span><span class="sxs-lookup"><span data-stu-id="a8c41-115">Error Handling</span></span>

<span data-ttu-id="a8c41-116">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="a8c41-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="a8c41-117">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="a8c41-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8c41-118">权限</span><span class="sxs-lookup"><span data-stu-id="a8c41-118">Permissions</span></span>
<span data-ttu-id="a8c41-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8c41-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8c41-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8c41-121">Permission type</span></span>      | <span data-ttu-id="a8c41-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8c41-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8c41-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8c41-123">Delegated (work or school account)</span></span> | <span data-ttu-id="a8c41-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8c41-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a8c41-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8c41-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8c41-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8c41-126">Not supported.</span></span>    |
|<span data-ttu-id="a8c41-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8c41-127">Application</span></span> | <span data-ttu-id="a8c41-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8c41-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8c41-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8c41-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="a8c41-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8c41-130">Request headers</span></span>
| <span data-ttu-id="a8c41-131">名称</span><span class="sxs-lookup"><span data-stu-id="a8c41-131">Name</span></span>       | <span data-ttu-id="a8c41-132">说明</span><span class="sxs-lookup"><span data-stu-id="a8c41-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8c41-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8c41-133">Authorization</span></span>  | <span data-ttu-id="a8c41-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8c41-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8c41-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a8c41-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="a8c41-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a8c41-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8c41-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8c41-139">Request body</span></span>
<span data-ttu-id="a8c41-140">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a8c41-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8c41-141">参数</span><span class="sxs-lookup"><span data-stu-id="a8c41-141">Parameter</span></span>    | <span data-ttu-id="a8c41-142">类型</span><span class="sxs-lookup"><span data-stu-id="a8c41-142">Type</span></span>   |<span data-ttu-id="a8c41-143">说明</span><span class="sxs-lookup"><span data-stu-id="a8c41-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8c41-144">index</span><span class="sxs-lookup"><span data-stu-id="a8c41-144">index</span></span>|<span data-ttu-id="a8c41-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a8c41-145">Int32</span></span>|<span data-ttu-id="a8c41-p107">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="a8c41-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="a8c41-151">values</span><span class="sxs-lookup"><span data-stu-id="a8c41-151">values</span></span>|<span data-ttu-id="a8c41-152">Json</span><span class="sxs-lookup"><span data-stu-id="a8c41-152">Json</span></span>|<span data-ttu-id="a8c41-p108">可选。未设置格式的表行值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="a8c41-p108">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="a8c41-155">响应</span><span class="sxs-lookup"><span data-stu-id="a8c41-155">Response</span></span>

<span data-ttu-id="a8c41-156">如果成功，此方法返回`200 OK`响应代码和[WorkbookTableRow](../resources/tablerow.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="a8c41-156">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8c41-157">示例</span><span class="sxs-lookup"><span data-stu-id="a8c41-157">Example</span></span>
<span data-ttu-id="a8c41-158">在此示例中的表的末尾插入两行数据。</span><span class="sxs-lookup"><span data-stu-id="a8c41-158">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="a8c41-159">请求</span><span class="sxs-lookup"><span data-stu-id="a8c41-159">Request</span></span>
<span data-ttu-id="a8c41-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8c41-160">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="a8c41-161">响应</span><span class="sxs-lookup"><span data-stu-id="a8c41-161">Response</span></span>
<span data-ttu-id="a8c41-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8c41-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
