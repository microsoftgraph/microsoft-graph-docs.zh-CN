---
title: 'ChartSeriesCollection: ItemAt'
description: 根据其在集合中的位置检索系列
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6d6d9cc9b8625d5303843d7427d3eb3e23cec82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912762"
---
# <a name="chartseriescollection-itemat"></a><span data-ttu-id="5f22f-103">ChartSeriesCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="5f22f-103">ChartSeriesCollection: ItemAt</span></span>

<span data-ttu-id="5f22f-104">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="5f22f-104">Retrieves a series based on its position in the collection</span></span>
## <a name="permissions"></a><span data-ttu-id="5f22f-105">权限</span><span class="sxs-lookup"><span data-stu-id="5f22f-105">Permissions</span></span>
<span data-ttu-id="5f22f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f22f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f22f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f22f-108">Permission type</span></span>      | <span data-ttu-id="5f22f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f22f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f22f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f22f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f22f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f22f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5f22f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f22f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f22f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f22f-113">Not supported.</span></span>    |
|<span data-ttu-id="5f22f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f22f-114">Application</span></span> | <span data-ttu-id="5f22f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f22f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f22f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f22f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series/itemAt

```
## <a name="request-headers"></a><span data-ttu-id="5f22f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f22f-117">Request headers</span></span>
| <span data-ttu-id="5f22f-118">名称</span><span class="sxs-lookup"><span data-stu-id="5f22f-118">Name</span></span>       | <span data-ttu-id="5f22f-119">说明</span><span class="sxs-lookup"><span data-stu-id="5f22f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5f22f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f22f-120">Authorization</span></span>  | <span data-ttu-id="5f22f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f22f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f22f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5f22f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="5f22f-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5f22f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f22f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f22f-126">Request body</span></span>
<span data-ttu-id="5f22f-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5f22f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f22f-128">参数</span><span class="sxs-lookup"><span data-stu-id="5f22f-128">Parameter</span></span>    | <span data-ttu-id="5f22f-129">类型</span><span class="sxs-lookup"><span data-stu-id="5f22f-129">Type</span></span>   |<span data-ttu-id="5f22f-130">说明</span><span class="sxs-lookup"><span data-stu-id="5f22f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f22f-131">index</span><span class="sxs-lookup"><span data-stu-id="5f22f-131">index</span></span>|<span data-ttu-id="5f22f-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5f22f-132">Int32</span></span>|<span data-ttu-id="5f22f-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="5f22f-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="5f22f-135">响应</span><span class="sxs-lookup"><span data-stu-id="5f22f-135">Response</span></span>

<span data-ttu-id="5f22f-136">如果成功，此方法返回`200 OK`响应代码和[WorkbookChartSeries](../resources/chartseries.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="5f22f-136">If successful, this method returns `200 OK` response code and [WorkbookChartSeries](../resources/chartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f22f-137">示例</span><span class="sxs-lookup"><span data-stu-id="5f22f-137">Example</span></span>
<span data-ttu-id="5f22f-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5f22f-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5f22f-139">请求</span><span class="sxs-lookup"><span data-stu-id="5f22f-139">Request</span></span>
<span data-ttu-id="5f22f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f22f-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "chartseriescollection_itemat",
  "idempotent": true,
  "@type": "requestBodyResourceFor.chartseriescollection_itemat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt
Content-type: application/json
Content-length: 20

{
  "index": 2
}
```

##### <a name="response"></a><span data-ttu-id="5f22f-141">响应</span><span class="sxs-lookup"><span data-stu-id="5f22f-141">Response</span></span>
<span data-ttu-id="5f22f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f22f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
