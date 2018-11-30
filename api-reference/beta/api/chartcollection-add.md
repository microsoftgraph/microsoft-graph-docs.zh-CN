---
title: 'ChartCollection: add'
description: 创建新图表。
ms.openlocfilehash: 85f6977ca3f9db267f3ec988286f0625baa20883
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046394"
---
# <a name="chartcollection-add"></a><span data-ttu-id="1e8b7-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="1e8b7-103">ChartCollection: add</span></span>

> <span data-ttu-id="1e8b7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e8b7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e8b7-106">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e8b7-107">权限</span><span class="sxs-lookup"><span data-stu-id="1e8b7-107">Permissions</span></span>
<span data-ttu-id="1e8b7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e8b7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e8b7-110">Permission type</span></span>      | <span data-ttu-id="1e8b7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e8b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e8b7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e8b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e8b7-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e8b7-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e8b7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e8b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e8b7-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e8b7-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1e8b7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e8b7-116">Application</span></span> | <span data-ttu-id="1e8b7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e8b7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e8b7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="1e8b7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e8b7-119">Request headers</span></span>
| <span data-ttu-id="1e8b7-120">名称</span><span class="sxs-lookup"><span data-stu-id="1e8b7-120">Name</span></span>       | <span data-ttu-id="1e8b7-121">说明</span><span class="sxs-lookup"><span data-stu-id="1e8b7-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e8b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e8b7-122">Authorization</span></span>  | <span data-ttu-id="1e8b7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e8b7-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1e8b7-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="1e8b7-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e8b7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e8b7-128">Request body</span></span>
<span data-ttu-id="1e8b7-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1e8b7-130">参数</span><span class="sxs-lookup"><span data-stu-id="1e8b7-130">Parameter</span></span>    | <span data-ttu-id="1e8b7-131">类型</span><span class="sxs-lookup"><span data-stu-id="1e8b7-131">Type</span></span>   |<span data-ttu-id="1e8b7-132">说明</span><span class="sxs-lookup"><span data-stu-id="1e8b7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e8b7-133">type</span><span class="sxs-lookup"><span data-stu-id="1e8b7-133">type</span></span>|<span data-ttu-id="1e8b7-134">string</span><span class="sxs-lookup"><span data-stu-id="1e8b7-134">string</span></span>|<span data-ttu-id="1e8b7-p105">表示图表的类型。可能的值是：`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.`。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="1e8b7-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="1e8b7-137">sourceData</span></span>|<span data-ttu-id="1e8b7-138">string</span><span class="sxs-lookup"><span data-stu-id="1e8b7-138">string</span></span>|<span data-ttu-id="1e8b7-139">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="1e8b7-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="1e8b7-140">seriesBy</span></span>|<span data-ttu-id="1e8b7-141">string</span><span class="sxs-lookup"><span data-stu-id="1e8b7-141">string</span></span>|<span data-ttu-id="1e8b7-p106">可选。指定列或行在图表上用作数据系列的方式。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="1e8b7-145">响应</span><span class="sxs-lookup"><span data-stu-id="1e8b7-145">Response</span></span>

<span data-ttu-id="1e8b7-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e8b7-147">示例</span><span class="sxs-lookup"><span data-stu-id="1e8b7-147">Example</span></span>
<span data-ttu-id="1e8b7-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e8b7-149">请求</span><span class="sxs-lookup"><span data-stu-id="1e8b7-149">Request</span></span>
<span data-ttu-id="1e8b7-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1e8b7-151">响应</span><span class="sxs-lookup"><span data-stu-id="1e8b7-151">Response</span></span>
<span data-ttu-id="1e8b7-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e8b7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
