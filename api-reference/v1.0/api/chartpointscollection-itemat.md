---
title: 'ChartPointsCollection: ItemAt'
description: 根据其在系列中的位置检索点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 91537f67a050d17484c7425eff342049df205df0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463500"
---
# <a name="chartpointscollection-itemat"></a><span data-ttu-id="333a5-103">ChartPointsCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="333a5-103">ChartPointsCollection: ItemAt</span></span>

<span data-ttu-id="333a5-104">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="333a5-104">Retrieve a point based on its position within the series.</span></span>
## <a name="permissions"></a><span data-ttu-id="333a5-105">权限</span><span class="sxs-lookup"><span data-stu-id="333a5-105">Permissions</span></span>
<span data-ttu-id="333a5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="333a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="333a5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="333a5-108">Permission type</span></span>      | <span data-ttu-id="333a5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="333a5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="333a5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="333a5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="333a5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="333a5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="333a5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="333a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="333a5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="333a5-113">Not supported.</span></span>    |
|<span data-ttu-id="333a5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="333a5-114">Application</span></span> | <span data-ttu-id="333a5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="333a5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="333a5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="333a5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="333a5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="333a5-117">Request headers</span></span>
| <span data-ttu-id="333a5-118">名称</span><span class="sxs-lookup"><span data-stu-id="333a5-118">Name</span></span>       | <span data-ttu-id="333a5-119">说明</span><span class="sxs-lookup"><span data-stu-id="333a5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="333a5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="333a5-120">Authorization</span></span>  | <span data-ttu-id="333a5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="333a5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="333a5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="333a5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="333a5-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="333a5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="333a5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="333a5-126">Request body</span></span>
<span data-ttu-id="333a5-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="333a5-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="333a5-128">参数</span><span class="sxs-lookup"><span data-stu-id="333a5-128">Parameter</span></span>    | <span data-ttu-id="333a5-129">类型</span><span class="sxs-lookup"><span data-stu-id="333a5-129">Type</span></span>   |<span data-ttu-id="333a5-130">说明</span><span class="sxs-lookup"><span data-stu-id="333a5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="333a5-131">index</span><span class="sxs-lookup"><span data-stu-id="333a5-131">index</span></span>|<span data-ttu-id="333a5-132">Int32</span><span class="sxs-lookup"><span data-stu-id="333a5-132">Int32</span></span>|<span data-ttu-id="333a5-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="333a5-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="333a5-135">响应</span><span class="sxs-lookup"><span data-stu-id="333a5-135">Response</span></span>

<span data-ttu-id="333a5-136">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[WorkbookChartPoint](../resources/chartpoint.md)对象。</span><span class="sxs-lookup"><span data-stu-id="333a5-136">If successful, this method returns `200 OK` response code and [WorkbookChartPoint](../resources/chartpoint.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="333a5-137">示例</span><span class="sxs-lookup"><span data-stu-id="333a5-137">Example</span></span>
<span data-ttu-id="333a5-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="333a5-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="333a5-139">请求</span><span class="sxs-lookup"><span data-stu-id="333a5-139">Request</span></span>
<span data-ttu-id="333a5-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="333a5-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="333a5-141">响应</span><span class="sxs-lookup"><span data-stu-id="333a5-141">Response</span></span>
<span data-ttu-id="333a5-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="333a5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
