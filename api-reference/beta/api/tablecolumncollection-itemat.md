---
title: 'TableColumnCollection: ItemAt'
description: 根据其在集合中的位置获取列。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0cd2c587c8520fc7c76f98f07d540ab0cd934baf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836160"
---
# <a name="tablecolumncollection-itemat"></a><span data-ttu-id="2d49e-103">TableColumnCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="2d49e-103">TableColumnCollection: ItemAt</span></span>

> <span data-ttu-id="2d49e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2d49e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d49e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2d49e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d49e-106">根据其在集合中的位置获取列。</span><span class="sxs-lookup"><span data-stu-id="2d49e-106">Gets a column based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d49e-107">权限</span><span class="sxs-lookup"><span data-stu-id="2d49e-107">Permissions</span></span>
<span data-ttu-id="2d49e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d49e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d49e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d49e-110">Permission type</span></span>      | <span data-ttu-id="2d49e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d49e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d49e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d49e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2d49e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d49e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d49e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d49e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d49e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d49e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d49e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d49e-116">Application</span></span> | <span data-ttu-id="2d49e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d49e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d49e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d49e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/ItemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="2d49e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d49e-119">Request headers</span></span>
| <span data-ttu-id="2d49e-120">名称</span><span class="sxs-lookup"><span data-stu-id="2d49e-120">Name</span></span>       | <span data-ttu-id="2d49e-121">说明</span><span class="sxs-lookup"><span data-stu-id="2d49e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2d49e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d49e-122">Authorization</span></span>  | <span data-ttu-id="2d49e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d49e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2d49e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2d49e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2d49e-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2d49e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d49e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d49e-128">Request body</span></span>
<span data-ttu-id="2d49e-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2d49e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d49e-130">参数</span><span class="sxs-lookup"><span data-stu-id="2d49e-130">Parameter</span></span>    | <span data-ttu-id="2d49e-131">类型</span><span class="sxs-lookup"><span data-stu-id="2d49e-131">Type</span></span>   |<span data-ttu-id="2d49e-132">说明</span><span class="sxs-lookup"><span data-stu-id="2d49e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d49e-133">index</span><span class="sxs-lookup"><span data-stu-id="2d49e-133">index</span></span>|<span data-ttu-id="2d49e-134">number</span><span class="sxs-lookup"><span data-stu-id="2d49e-134">number</span></span>|<span data-ttu-id="2d49e-p105">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="2d49e-p105">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="2d49e-137">响应</span><span class="sxs-lookup"><span data-stu-id="2d49e-137">Response</span></span>

<span data-ttu-id="2d49e-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d49e-138">If successful, this method returns `200 OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d49e-139">示例</span><span class="sxs-lookup"><span data-stu-id="2d49e-139">Example</span></span>
<span data-ttu-id="2d49e-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2d49e-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d49e-141">请求</span><span class="sxs-lookup"><span data-stu-id="2d49e-141">Request</span></span>
<span data-ttu-id="2d49e-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d49e-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="2d49e-143">响应</span><span class="sxs-lookup"><span data-stu-id="2d49e-143">Response</span></span>
<span data-ttu-id="2d49e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d49e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumnCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
