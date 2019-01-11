---
title: 'TableColumnCollection: add'
description: 向表中添加新列。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: bd3c1a2b1cbfcb8d0e47f9d7ec93b0695e9854c3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870236"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="8b92c-103">TableColumnCollection: add</span><span class="sxs-lookup"><span data-stu-id="8b92c-103">TableColumnCollection: add</span></span>

> <span data-ttu-id="8b92c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8b92c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b92c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b92c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b92c-106">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="8b92c-106">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b92c-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b92c-107">Permissions</span></span>
<span data-ttu-id="8b92c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b92c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b92c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b92c-110">Permission type</span></span>      | <span data-ttu-id="8b92c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b92c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b92c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b92c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b92c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b92c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b92c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b92c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b92c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b92c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b92c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b92c-116">Application</span></span> | <span data-ttu-id="8b92c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b92c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b92c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b92c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="8b92c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b92c-119">Request headers</span></span>
| <span data-ttu-id="8b92c-120">名称</span><span class="sxs-lookup"><span data-stu-id="8b92c-120">Name</span></span>       | <span data-ttu-id="8b92c-121">说明</span><span class="sxs-lookup"><span data-stu-id="8b92c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b92c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b92c-122">Authorization</span></span>  | <span data-ttu-id="8b92c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b92c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b92c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8b92c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b92c-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8b92c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b92c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b92c-128">Request body</span></span>
<span data-ttu-id="8b92c-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8b92c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8b92c-130">参数</span><span class="sxs-lookup"><span data-stu-id="8b92c-130">Parameter</span></span>    | <span data-ttu-id="8b92c-131">类型</span><span class="sxs-lookup"><span data-stu-id="8b92c-131">Type</span></span>   |<span data-ttu-id="8b92c-132">说明</span><span class="sxs-lookup"><span data-stu-id="8b92c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b92c-133">index</span><span class="sxs-lookup"><span data-stu-id="8b92c-133">index</span></span>|<span data-ttu-id="8b92c-134">number</span><span class="sxs-lookup"><span data-stu-id="8b92c-134">number</span></span>|<span data-ttu-id="8b92c-p105">指定新列的相对位置。之前位于此位置的列向右移动。索引值应等于或小于最后一列的索引值，因此不能用于在表末尾附加列。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="8b92c-p105">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="8b92c-139">values</span><span class="sxs-lookup"><span data-stu-id="8b92c-139">values</span></span>|<span data-ttu-id="8b92c-140">（布尔值、字符串或数字）</span><span class="sxs-lookup"><span data-stu-id="8b92c-140">(boolean or string or number)</span></span>|<span data-ttu-id="8b92c-p106">可选。未设置格式的表列值的二维数组。</span><span class="sxs-lookup"><span data-stu-id="8b92c-p106">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="8b92c-143">响应</span><span class="sxs-lookup"><span data-stu-id="8b92c-143">Response</span></span>

<span data-ttu-id="8b92c-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b92c-144">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b92c-145">示例</span><span class="sxs-lookup"><span data-stu-id="8b92c-145">Example</span></span>
<span data-ttu-id="8b92c-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8b92c-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8b92c-147">请求</span><span class="sxs-lookup"><span data-stu-id="8b92c-147">Request</span></span>
<span data-ttu-id="8b92c-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b92c-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="8b92c-149">响应</span><span class="sxs-lookup"><span data-stu-id="8b92c-149">Response</span></span>
<span data-ttu-id="8b92c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8b92c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
