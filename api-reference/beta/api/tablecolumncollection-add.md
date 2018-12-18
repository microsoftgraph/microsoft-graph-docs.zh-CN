---
title: 'TableColumnCollection: add'
description: 向表中添加新列。
author: lumine2008
ms.openlocfilehash: a0897dc4eff387d14643b0a067ef92ad79755614
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350020"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="1c4fe-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="1c4fe-103">TableColumnCollection: add</span></span>

> <span data-ttu-id="1c4fe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c4fe-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c4fe-106">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-106">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c4fe-107">权限</span><span class="sxs-lookup"><span data-stu-id="1c4fe-107">Permissions</span></span>
<span data-ttu-id="1c4fe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c4fe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c4fe-110">Permission type</span></span>      | <span data-ttu-id="1c4fe-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c4fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c4fe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c4fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1c4fe-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c4fe-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c4fe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c4fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c4fe-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c4fe-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c4fe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c4fe-116">Application</span></span> | <span data-ttu-id="1c4fe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c4fe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c4fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="1c4fe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c4fe-119">Request headers</span></span>
| <span data-ttu-id="1c4fe-120">Name</span><span class="sxs-lookup"><span data-stu-id="1c4fe-120">Name</span></span>       | <span data-ttu-id="1c4fe-121">说明</span><span class="sxs-lookup"><span data-stu-id="1c4fe-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1c4fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c4fe-122">Authorization</span></span>  | <span data-ttu-id="1c4fe-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c4fe-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1c4fe-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c4fe-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c4fe-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c4fe-128">Request body</span></span>
<span data-ttu-id="1c4fe-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c4fe-130">参数</span><span class="sxs-lookup"><span data-stu-id="1c4fe-130">Parameter</span></span>    | <span data-ttu-id="1c4fe-131">Type</span><span class="sxs-lookup"><span data-stu-id="1c4fe-131">Type</span></span>   |<span data-ttu-id="1c4fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="1c4fe-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c4fe-133">index</span><span class="sxs-lookup"><span data-stu-id="1c4fe-133">index</span></span>|<span data-ttu-id="1c4fe-134">number</span><span class="sxs-lookup"><span data-stu-id="1c4fe-134">number</span></span>|<span data-ttu-id="1c4fe-p105">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-p105">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="1c4fe-139">values</span><span class="sxs-lookup"><span data-stu-id="1c4fe-139">values</span></span>|<span data-ttu-id="1c4fe-140">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="1c4fe-140">(boolean or string or number)</span></span>|<span data-ttu-id="1c4fe-p106">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-p106">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="1c4fe-143">响应</span><span class="sxs-lookup"><span data-stu-id="1c4fe-143">Response</span></span>

<span data-ttu-id="1c4fe-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-144">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c4fe-145">示例</span><span class="sxs-lookup"><span data-stu-id="1c4fe-145">Example</span></span>
<span data-ttu-id="1c4fe-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c4fe-147">请求</span><span class="sxs-lookup"><span data-stu-id="1c4fe-147">Request</span></span>
<span data-ttu-id="1c4fe-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1c4fe-149">响应</span><span class="sxs-lookup"><span data-stu-id="1c4fe-149">Response</span></span>
<span data-ttu-id="1c4fe-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c4fe-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
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
  "tocPath": ""
}-->