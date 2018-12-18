---
title: 'ChartCollection: add'
description: 创建新图表。
author: lumine2008
ms.openlocfilehash: 704afc9890e3921c69cdd7b746c0e362c4627511
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325548"
---
# <a name="chartcollection-add"></a><span data-ttu-id="7c0d4-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="7c0d4-103">ChartCollection: add</span></span>

> <span data-ttu-id="7c0d4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c0d4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c0d4-106">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="7c0d4-107">权限</span><span class="sxs-lookup"><span data-stu-id="7c0d4-107">Permissions</span></span>
<span data-ttu-id="7c0d4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c0d4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c0d4-110">Permission type</span></span>      | <span data-ttu-id="7c0d4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c0d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c0d4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c0d4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7c0d4-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c0d4-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c0d4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c0d4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c0d4-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c0d4-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7c0d4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c0d4-116">Application</span></span> | <span data-ttu-id="7c0d4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c0d4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c0d4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="7c0d4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c0d4-119">Request headers</span></span>
| <span data-ttu-id="7c0d4-120">Name</span><span class="sxs-lookup"><span data-stu-id="7c0d4-120">Name</span></span>       | <span data-ttu-id="7c0d4-121">说明</span><span class="sxs-lookup"><span data-stu-id="7c0d4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7c0d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c0d4-122">Authorization</span></span>  | <span data-ttu-id="7c0d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c0d4-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7c0d4-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7c0d4-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c0d4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c0d4-128">Request body</span></span>
<span data-ttu-id="7c0d4-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7c0d4-130">参数</span><span class="sxs-lookup"><span data-stu-id="7c0d4-130">Parameter</span></span>    | <span data-ttu-id="7c0d4-131">Type</span><span class="sxs-lookup"><span data-stu-id="7c0d4-131">Type</span></span>   |<span data-ttu-id="7c0d4-132">说明</span><span class="sxs-lookup"><span data-stu-id="7c0d4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c0d4-133">type</span><span class="sxs-lookup"><span data-stu-id="7c0d4-133">type</span></span>|<span data-ttu-id="7c0d4-134">string</span><span class="sxs-lookup"><span data-stu-id="7c0d4-134">string</span></span>|<span data-ttu-id="7c0d4-p105">表示图表的类型。可能的值是：`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.`。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="7c0d4-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="7c0d4-137">sourceData</span></span>|<span data-ttu-id="7c0d4-138">string</span><span class="sxs-lookup"><span data-stu-id="7c0d4-138">string</span></span>|<span data-ttu-id="7c0d4-139">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="7c0d4-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="7c0d4-140">seriesBy</span></span>|<span data-ttu-id="7c0d4-141">string</span><span class="sxs-lookup"><span data-stu-id="7c0d4-141">string</span></span>|<span data-ttu-id="7c0d4-p106">可选。指定列或行在图表上用作数据系列的方式。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="7c0d4-145">响应</span><span class="sxs-lookup"><span data-stu-id="7c0d4-145">Response</span></span>

<span data-ttu-id="7c0d4-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c0d4-147">示例</span><span class="sxs-lookup"><span data-stu-id="7c0d4-147">Example</span></span>
<span data-ttu-id="7c0d4-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c0d4-149">请求</span><span class="sxs-lookup"><span data-stu-id="7c0d4-149">Request</span></span>
<span data-ttu-id="7c0d4-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```

##### <a name="response"></a><span data-ttu-id="7c0d4-151">响应</span><span class="sxs-lookup"><span data-stu-id="7c0d4-151">Response</span></span>
<span data-ttu-id="7c0d4-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c0d4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
