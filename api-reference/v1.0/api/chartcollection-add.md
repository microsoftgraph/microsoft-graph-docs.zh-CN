---
title: 'ChartCollection: add'
description: 创建新图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1e4813ee72f7cccb109369ef12b884efe24e9563
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916402"
---
# <a name="chartcollection-add"></a><span data-ttu-id="bfb29-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="bfb29-103">ChartCollection: add</span></span>

<span data-ttu-id="bfb29-104">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="bfb29-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="bfb29-105">权限</span><span class="sxs-lookup"><span data-stu-id="bfb29-105">Permissions</span></span>
<span data-ttu-id="bfb29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfb29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfb29-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfb29-108">Permission type</span></span>      | <span data-ttu-id="bfb29-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfb29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfb29-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb29-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfb29-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfb29-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bfb29-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfb29-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfb29-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfb29-113">Not supported.</span></span>    |
|<span data-ttu-id="bfb29-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfb29-114">Application</span></span> | <span data-ttu-id="bfb29-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfb29-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfb29-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfb29-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="bfb29-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfb29-117">Request headers</span></span>
| <span data-ttu-id="bfb29-118">名称</span><span class="sxs-lookup"><span data-stu-id="bfb29-118">Name</span></span>       | <span data-ttu-id="bfb29-119">说明</span><span class="sxs-lookup"><span data-stu-id="bfb29-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bfb29-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfb29-120">Authorization</span></span>  | <span data-ttu-id="bfb29-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfb29-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bfb29-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bfb29-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bfb29-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="bfb29-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfb29-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfb29-126">Request body</span></span>
<span data-ttu-id="bfb29-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="bfb29-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bfb29-128">参数</span><span class="sxs-lookup"><span data-stu-id="bfb29-128">Parameter</span></span>    | <span data-ttu-id="bfb29-129">类型</span><span class="sxs-lookup"><span data-stu-id="bfb29-129">Type</span></span>   |<span data-ttu-id="bfb29-130">说明</span><span class="sxs-lookup"><span data-stu-id="bfb29-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfb29-131">type</span><span class="sxs-lookup"><span data-stu-id="bfb29-131">type</span></span>|<span data-ttu-id="bfb29-132">string</span><span class="sxs-lookup"><span data-stu-id="bfb29-132">string</span></span>|<span data-ttu-id="bfb29-133">代表图表的类型。</span><span class="sxs-lookup"><span data-stu-id="bfb29-133">Represents the type of a chart.</span></span>  <span data-ttu-id="bfb29-134">可能的值为： `ColumnClustered`， `ColumnStacked`， `ColumnStacked100`， `BarClustered`， `BarStacked`， `BarStacked100`， `LineStacked`， `LineStacked100`， `LineMarkers`， `LineMarkersStacked`， `LineMarkersStacked100`， `PieOfPie`， `etc.`。</span><span class="sxs-lookup"><span data-stu-id="bfb29-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="bfb29-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="bfb29-135">sourceData</span></span>|<span data-ttu-id="bfb29-136">Json</span><span class="sxs-lookup"><span data-stu-id="bfb29-136">Json</span></span>|<span data-ttu-id="bfb29-137">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="bfb29-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="bfb29-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="bfb29-138">seriesBy</span></span>|<span data-ttu-id="bfb29-139">string</span><span class="sxs-lookup"><span data-stu-id="bfb29-139">string</span></span>|<span data-ttu-id="bfb29-140">可选。</span><span class="sxs-lookup"><span data-stu-id="bfb29-140">Optional.</span></span> <span data-ttu-id="bfb29-141">指定的方式列或行用作图表上的数据系列。</span><span class="sxs-lookup"><span data-stu-id="bfb29-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="bfb29-142">可能的值为： `Auto`， `Columns`， `Rows`。</span><span class="sxs-lookup"><span data-stu-id="bfb29-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="bfb29-143">响应</span><span class="sxs-lookup"><span data-stu-id="bfb29-143">Response</span></span>

<span data-ttu-id="bfb29-144">如果成功，此方法返回`200 OK`响应代码和[WorkbookChart](../resources/chart.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="bfb29-144">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfb29-145">示例</span><span class="sxs-lookup"><span data-stu-id="bfb29-145">Example</span></span>
<span data-ttu-id="bfb29-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="bfb29-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bfb29-147">请求</span><span class="sxs-lookup"><span data-stu-id="bfb29-147">Request</span></span>
<span data-ttu-id="bfb29-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bfb29-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="bfb29-149">响应</span><span class="sxs-lookup"><span data-stu-id="bfb29-149">Response</span></span>
<span data-ttu-id="bfb29-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bfb29-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
