---
title: 'TableRowCollection: ItemAt'
description: 根据其在集合中的位置获取行。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 017618e37be33e7f64ce01082e8fe16b23c03f13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880709"
---
# <a name="tablerowcollection-itemat"></a><span data-ttu-id="8ae12-103">TableRowCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="8ae12-103">TableRowCollection: ItemAt</span></span>

<span data-ttu-id="8ae12-104">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="8ae12-104">Gets a row based on its position in the collection.</span></span>
## <a name="permissions"></a><span data-ttu-id="8ae12-105">权限</span><span class="sxs-lookup"><span data-stu-id="8ae12-105">Permissions</span></span>
<span data-ttu-id="8ae12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ae12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae12-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ae12-108">Permission type</span></span>      | <span data-ttu-id="8ae12-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ae12-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ae12-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ae12-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ae12-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ae12-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8ae12-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ae12-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ae12-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ae12-113">Not supported.</span></span>    |
|<span data-ttu-id="8ae12-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ae12-114">Application</span></span> | <span data-ttu-id="8ae12-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ae12-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ae12-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ae12-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/itemAt
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="8ae12-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ae12-117">Request headers</span></span>
| <span data-ttu-id="8ae12-118">名称</span><span class="sxs-lookup"><span data-stu-id="8ae12-118">Name</span></span>       | <span data-ttu-id="8ae12-119">说明</span><span class="sxs-lookup"><span data-stu-id="8ae12-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ae12-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae12-120">Authorization</span></span>  | <span data-ttu-id="8ae12-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ae12-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8ae12-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8ae12-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8ae12-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8ae12-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae12-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ae12-126">Request body</span></span>
<span data-ttu-id="8ae12-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8ae12-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8ae12-128">参数</span><span class="sxs-lookup"><span data-stu-id="8ae12-128">Parameter</span></span>    | <span data-ttu-id="8ae12-129">类型</span><span class="sxs-lookup"><span data-stu-id="8ae12-129">Type</span></span>   |<span data-ttu-id="8ae12-130">说明</span><span class="sxs-lookup"><span data-stu-id="8ae12-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ae12-131">index</span><span class="sxs-lookup"><span data-stu-id="8ae12-131">index</span></span>|<span data-ttu-id="8ae12-132">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae12-132">Int32</span></span>|<span data-ttu-id="8ae12-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="8ae12-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="8ae12-135">响应</span><span class="sxs-lookup"><span data-stu-id="8ae12-135">Response</span></span>

<span data-ttu-id="8ae12-136">如果成功，此方法返回`200 OK`响应代码和[WorkbookTableRow](../resources/tablerow.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="8ae12-136">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae12-137">示例</span><span class="sxs-lookup"><span data-stu-id="8ae12-137">Example</span></span>
<span data-ttu-id="8ae12-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8ae12-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8ae12-139">请求</span><span class="sxs-lookup"><span data-stu-id="8ae12-139">Request</span></span>
<span data-ttu-id="8ae12-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ae12-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerowcollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.tablerowcollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 4
}
```

##### <a name="response"></a><span data-ttu-id="8ae12-141">响应</span><span class="sxs-lookup"><span data-stu-id="8ae12-141">Response</span></span>
<span data-ttu-id="8ae12-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ae12-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRowCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
