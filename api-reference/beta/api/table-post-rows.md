---
title: 创建 TableRow
description: '向表末尾的行。 请注意 API 可以接受使用此 API 的多个行数据。 一次添加一个行可能导致性能下降。 建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。 为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。 试验要确定的理想要使用一个 API 调用中的行数的行数。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 88fd78516528f62925b18c1c45d9452404be6881
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529507"
---
# <a name="create-tablerow"></a><span data-ttu-id="6b340-108">创建 TableRow</span><span class="sxs-lookup"><span data-stu-id="6b340-108">Create TableRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b340-109">向表末尾的行。</span><span class="sxs-lookup"><span data-stu-id="6b340-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="6b340-110">请注意 API 可以接受使用此 API 的多个行数据。</span><span class="sxs-lookup"><span data-stu-id="6b340-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="6b340-111">一次添加一个行可能导致性能下降。</span><span class="sxs-lookup"><span data-stu-id="6b340-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="6b340-112">建议的方法是批处理一起中单个呼叫，而不是以单个行插入行。</span><span class="sxs-lookup"><span data-stu-id="6b340-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="6b340-113">为了获得最佳结果，收集要插入的应用程序一侧，并执行单个行的行添加操作。</span><span class="sxs-lookup"><span data-stu-id="6b340-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="6b340-114">试验要确定的理想要使用一个 API 调用中的行数的行数。</span><span class="sxs-lookup"><span data-stu-id="6b340-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="6b340-115">错误处理</span><span class="sxs-lookup"><span data-stu-id="6b340-115">Error Handling</span></span>

<span data-ttu-id="6b340-116">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="6b340-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="6b340-117">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="6b340-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b340-118">权限</span><span class="sxs-lookup"><span data-stu-id="6b340-118">Permissions</span></span>
<span data-ttu-id="6b340-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b340-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b340-121">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b340-121">Permission type</span></span>      | <span data-ttu-id="6b340-122">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b340-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b340-123">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b340-123">Delegated (work or school account)</span></span> | <span data-ttu-id="6b340-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b340-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6b340-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b340-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b340-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b340-126">Not supported.</span></span>    |
|<span data-ttu-id="6b340-127">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b340-127">Application</span></span> | <span data-ttu-id="6b340-128">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b340-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b340-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b340-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="6b340-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b340-130">Request headers</span></span>
| <span data-ttu-id="6b340-131">名称</span><span class="sxs-lookup"><span data-stu-id="6b340-131">Name</span></span>       | <span data-ttu-id="6b340-132">说明</span><span class="sxs-lookup"><span data-stu-id="6b340-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6b340-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b340-133">Authorization</span></span>  | <span data-ttu-id="6b340-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b340-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6b340-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6b340-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="6b340-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6b340-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b340-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b340-139">Request body</span></span>
<span data-ttu-id="6b340-140">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6b340-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b340-141">参数</span><span class="sxs-lookup"><span data-stu-id="6b340-141">Parameter</span></span>    | <span data-ttu-id="6b340-142">类型</span><span class="sxs-lookup"><span data-stu-id="6b340-142">Type</span></span>   |<span data-ttu-id="6b340-143">说明</span><span class="sxs-lookup"><span data-stu-id="6b340-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b340-144">index</span><span class="sxs-lookup"><span data-stu-id="6b340-144">index</span></span>|<span data-ttu-id="6b340-145">number</span><span class="sxs-lookup"><span data-stu-id="6b340-145">number</span></span>|<span data-ttu-id="6b340-p107">可选。指定新行的相对位置。如果为空，将在末尾进行添加。插入的行下方的任何行将向下移动。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="6b340-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="6b340-151">values</span><span class="sxs-lookup"><span data-stu-id="6b340-151">values</span></span>|<span data-ttu-id="6b340-152">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="6b340-152">(boolean or string or number)</span></span>|<span data-ttu-id="6b340-153">无格式的表格行值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="6b340-153">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="6b340-154">响应</span><span class="sxs-lookup"><span data-stu-id="6b340-154">Response</span></span>

<span data-ttu-id="6b340-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b340-155">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b340-156">示例</span><span class="sxs-lookup"><span data-stu-id="6b340-156">Example</span></span>
<span data-ttu-id="6b340-157">在此示例中的表的末尾插入两行数据。</span><span class="sxs-lookup"><span data-stu-id="6b340-157">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="6b340-158">请求</span><span class="sxs-lookup"><span data-stu-id="6b340-158">Request</span></span>
<span data-ttu-id="6b340-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b340-159">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6b340-160">响应</span><span class="sxs-lookup"><span data-stu-id="6b340-160">Response</span></span>
<span data-ttu-id="6b340-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b340-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-post-rows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
