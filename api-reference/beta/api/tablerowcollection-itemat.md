---
title: 'TableRowCollection: ItemAt'
description: 根据其在集合中的位置获取行。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 01b0d1e5ba480479752ca3ac9469697ca49ca5c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834179"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="95ae3-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="95ae3-103">TableRowCollection: ItemAt</span></span>

> <span data-ttu-id="95ae3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="95ae3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95ae3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="95ae3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95ae3-106">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="95ae3-106">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="95ae3-107">权限</span><span class="sxs-lookup"><span data-stu-id="95ae3-107">Permissions</span></span>
<span data-ttu-id="95ae3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95ae3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95ae3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95ae3-110">Permission type</span></span>      | <span data-ttu-id="95ae3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="95ae3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95ae3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95ae3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="95ae3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95ae3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="95ae3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95ae3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95ae3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95ae3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="95ae3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="95ae3-116">Application</span></span> | <span data-ttu-id="95ae3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="95ae3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95ae3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95ae3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="95ae3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95ae3-119">Request headers</span></span>
| <span data-ttu-id="95ae3-120">名称</span><span class="sxs-lookup"><span data-stu-id="95ae3-120">Name</span></span>       | <span data-ttu-id="95ae3-121">说明</span><span class="sxs-lookup"><span data-stu-id="95ae3-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="95ae3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95ae3-122">Authorization</span></span>  | <span data-ttu-id="95ae3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="95ae3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="95ae3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="95ae3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="95ae3-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="95ae3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="95ae3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="95ae3-128">Request body</span></span>
<span data-ttu-id="95ae3-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="95ae3-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="95ae3-130">参数</span><span class="sxs-lookup"><span data-stu-id="95ae3-130">Parameter</span></span>    | <span data-ttu-id="95ae3-131">类型</span><span class="sxs-lookup"><span data-stu-id="95ae3-131">Type</span></span>   |<span data-ttu-id="95ae3-132">说明</span><span class="sxs-lookup"><span data-stu-id="95ae3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95ae3-133">index</span><span class="sxs-lookup"><span data-stu-id="95ae3-133">index</span></span>|<span data-ttu-id="95ae3-134">number</span><span class="sxs-lookup"><span data-stu-id="95ae3-134">number</span></span>|<span data-ttu-id="95ae3-p105">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="95ae3-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="95ae3-137">响应</span><span class="sxs-lookup"><span data-stu-id="95ae3-137">Response</span></span>

<span data-ttu-id="95ae3-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95ae3-138">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95ae3-139">示例</span><span class="sxs-lookup"><span data-stu-id="95ae3-139">Example</span></span>
<span data-ttu-id="95ae3-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="95ae3-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="95ae3-141">请求</span><span class="sxs-lookup"><span data-stu-id="95ae3-141">Request</span></span>
<span data-ttu-id="95ae3-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95ae3-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="95ae3-143">响应</span><span class="sxs-lookup"><span data-stu-id="95ae3-143">Response</span></span>
<span data-ttu-id="95ae3-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95ae3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
