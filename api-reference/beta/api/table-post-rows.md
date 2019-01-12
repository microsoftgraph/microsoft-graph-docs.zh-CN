---
title: 创建 TableRow
description: '向表末尾的行。 请注意 API 可以接受使用此 API 的多个行数据。 一次添加一个行可能导致性能下降。 建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。 为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。 试验要确定的理想要使用一个 API 调用中的行数的行数。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 7e5b44d5ef46dbbd534594aec16f1e6ac180c754
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918278"
---
# <a name="create-tablerow"></a><span data-ttu-id="71bda-108">创建 TableRow</span><span class="sxs-lookup"><span data-stu-id="71bda-108">Create TableRow</span></span>

> <span data-ttu-id="71bda-109">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="71bda-109">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71bda-110">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="71bda-110">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71bda-111">向表末尾的行。</span><span class="sxs-lookup"><span data-stu-id="71bda-111">Adds rows to the end of the table.</span></span> <span data-ttu-id="71bda-112">请注意 API 可以接受使用此 API 的多个行数据。</span><span class="sxs-lookup"><span data-stu-id="71bda-112">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="71bda-113">一次添加一个行可能导致性能下降。</span><span class="sxs-lookup"><span data-stu-id="71bda-113">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="71bda-114">建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。</span><span class="sxs-lookup"><span data-stu-id="71bda-114">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="71bda-115">为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。</span><span class="sxs-lookup"><span data-stu-id="71bda-115">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="71bda-116">试验要确定的理想要使用一个 API 调用中的行数的行数。</span><span class="sxs-lookup"><span data-stu-id="71bda-116">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="71bda-117">错误处理</span><span class="sxs-lookup"><span data-stu-id="71bda-117">Error Handling</span></span>

<span data-ttu-id="71bda-118">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="71bda-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="71bda-119">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="71bda-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="71bda-120">权限</span><span class="sxs-lookup"><span data-stu-id="71bda-120">Permissions</span></span>
<span data-ttu-id="71bda-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71bda-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71bda-123">权限类型</span><span class="sxs-lookup"><span data-stu-id="71bda-123">Permission type</span></span>      | <span data-ttu-id="71bda-124">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71bda-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71bda-125">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71bda-125">Delegated (work or school account)</span></span> | <span data-ttu-id="71bda-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71bda-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="71bda-127">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71bda-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71bda-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="71bda-128">Not supported.</span></span>    |
|<span data-ttu-id="71bda-129">应用程序</span><span class="sxs-lookup"><span data-stu-id="71bda-129">Application</span></span> | <span data-ttu-id="71bda-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="71bda-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71bda-131">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71bda-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="71bda-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="71bda-132">Request headers</span></span>
| <span data-ttu-id="71bda-133">名称</span><span class="sxs-lookup"><span data-stu-id="71bda-133">Name</span></span>       | <span data-ttu-id="71bda-134">说明</span><span class="sxs-lookup"><span data-stu-id="71bda-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71bda-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="71bda-135">Authorization</span></span>  | <span data-ttu-id="71bda-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71bda-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71bda-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71bda-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="71bda-p107">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="71bda-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71bda-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="71bda-141">Request body</span></span>
<span data-ttu-id="71bda-142">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="71bda-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="71bda-143">参数</span><span class="sxs-lookup"><span data-stu-id="71bda-143">Parameter</span></span>    | <span data-ttu-id="71bda-144">类型</span><span class="sxs-lookup"><span data-stu-id="71bda-144">Type</span></span>   |<span data-ttu-id="71bda-145">说明</span><span class="sxs-lookup"><span data-stu-id="71bda-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71bda-146">index</span><span class="sxs-lookup"><span data-stu-id="71bda-146">index</span></span>|<span data-ttu-id="71bda-147">number</span><span class="sxs-lookup"><span data-stu-id="71bda-147">number</span></span>|<span data-ttu-id="71bda-p108">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="71bda-p108">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="71bda-153">values</span><span class="sxs-lookup"><span data-stu-id="71bda-153">values</span></span>|<span data-ttu-id="71bda-154">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="71bda-154">(boolean or string or number)</span></span>|<span data-ttu-id="71bda-155">无格式的表格行值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="71bda-155">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="71bda-156">响应</span><span class="sxs-lookup"><span data-stu-id="71bda-156">Response</span></span>

<span data-ttu-id="71bda-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71bda-157">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71bda-158">示例</span><span class="sxs-lookup"><span data-stu-id="71bda-158">Example</span></span>
<span data-ttu-id="71bda-159">在此示例中的表的末尾插入两行数据。</span><span class="sxs-lookup"><span data-stu-id="71bda-159">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="71bda-160">请求</span><span class="sxs-lookup"><span data-stu-id="71bda-160">Request</span></span>
<span data-ttu-id="71bda-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71bda-161">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="71bda-162">响应</span><span class="sxs-lookup"><span data-stu-id="71bda-162">Response</span></span>
<span data-ttu-id="71bda-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71bda-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "tocPath": ""
}-->
