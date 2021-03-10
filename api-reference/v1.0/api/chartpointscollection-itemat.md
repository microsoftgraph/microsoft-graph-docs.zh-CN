---
title: 'ChartPointsCollection: ItemAt'
description: 根据其在系列中的位置检索点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 300a561113abdae978531f080fe8ac8b2fb1f638
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575586"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="7bf38-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="7bf38-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="7bf38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bf38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bf38-105">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="7bf38-105">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="7bf38-106">权限</span><span class="sxs-lookup"><span data-stu-id="7bf38-106">Permissions</span></span>
<span data-ttu-id="7bf38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bf38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bf38-109">Permission type</span></span>      | <span data-ttu-id="7bf38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7bf38-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bf38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bf38-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7bf38-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bf38-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7bf38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bf38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bf38-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bf38-114">Not supported.</span></span>    |
|<span data-ttu-id="7bf38-115">Application</span><span class="sxs-lookup"><span data-stu-id="7bf38-115">Application</span></span> | <span data-ttu-id="7bf38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bf38-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bf38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bf38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="7bf38-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bf38-118">Request headers</span></span>
| <span data-ttu-id="7bf38-119">名称</span><span class="sxs-lookup"><span data-stu-id="7bf38-119">Name</span></span>       | <span data-ttu-id="7bf38-120">说明</span><span class="sxs-lookup"><span data-stu-id="7bf38-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7bf38-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bf38-121">Authorization</span></span>  | <span data-ttu-id="7bf38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7bf38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bf38-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7bf38-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7bf38-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7bf38-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bf38-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bf38-127">Request body</span></span>
<span data-ttu-id="7bf38-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7bf38-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7bf38-129">参数</span><span class="sxs-lookup"><span data-stu-id="7bf38-129">Parameter</span></span>    | <span data-ttu-id="7bf38-130">类型</span><span class="sxs-lookup"><span data-stu-id="7bf38-130">Type</span></span>   |<span data-ttu-id="7bf38-131">说明</span><span class="sxs-lookup"><span data-stu-id="7bf38-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bf38-132">index</span><span class="sxs-lookup"><span data-stu-id="7bf38-132">index</span></span>|<span data-ttu-id="7bf38-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7bf38-133">Int32</span></span>|<span data-ttu-id="7bf38-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="7bf38-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="7bf38-136">响应</span><span class="sxs-lookup"><span data-stu-id="7bf38-136">Response</span></span>

<span data-ttu-id="7bf38-137">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [WorkbookChartPoint](../resources/chartpoint.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bf38-137">If successful, this method returns `200 OK` response code and [WorkbookChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bf38-138">示例</span><span class="sxs-lookup"><span data-stu-id="7bf38-138">Example</span></span>
<span data-ttu-id="7bf38-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7bf38-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7bf38-140">请求</span><span class="sxs-lookup"><span data-stu-id="7bf38-140">Request</span></span>
<span data-ttu-id="7bf38-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bf38-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7bf38-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf38-142">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartpointscollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartpointscollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 8
}
```
# <a name="javascript"></a>[<span data-ttu-id="7bf38-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bf38-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartpointscollection-itemat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bf38-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bf38-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartpointscollection-itemat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7bf38-145">响应</span><span class="sxs-lookup"><span data-stu-id="7bf38-145">Response</span></span>
<span data-ttu-id="7bf38-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7bf38-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartPoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 20

{
  "value": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointsCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

