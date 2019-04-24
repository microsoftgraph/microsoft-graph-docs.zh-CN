---
title: 'ChartCollection: add'
description: 创建新图表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cdb3ff01b0741f0f1a4a0bff22e3a8e3dc32335c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456589"
---
# <a name="chartcollection-add"></a><span data-ttu-id="4d869-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="4d869-103">ChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d869-104">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="4d869-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d869-105">权限</span><span class="sxs-lookup"><span data-stu-id="4d869-105">Permissions</span></span>
<span data-ttu-id="4d869-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d869-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d869-108">Permission type</span></span>      | <span data-ttu-id="4d869-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d869-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d869-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d869-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d869-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d869-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d869-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d869-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d869-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d869-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d869-114">Application</span><span class="sxs-lookup"><span data-stu-id="4d869-114">Application</span></span> | <span data-ttu-id="4d869-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d869-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d869-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d869-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="4d869-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d869-117">Request headers</span></span>
| <span data-ttu-id="4d869-118">名称</span><span class="sxs-lookup"><span data-stu-id="4d869-118">Name</span></span>       | <span data-ttu-id="4d869-119">说明</span><span class="sxs-lookup"><span data-stu-id="4d869-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4d869-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d869-120">Authorization</span></span>  | <span data-ttu-id="4d869-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d869-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d869-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4d869-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4d869-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="4d869-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d869-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d869-126">Request body</span></span>
<span data-ttu-id="4d869-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4d869-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d869-128">参数</span><span class="sxs-lookup"><span data-stu-id="4d869-128">Parameter</span></span>    | <span data-ttu-id="4d869-129">类型</span><span class="sxs-lookup"><span data-stu-id="4d869-129">Type</span></span>   |<span data-ttu-id="4d869-130">描述</span><span class="sxs-lookup"><span data-stu-id="4d869-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d869-131">类型</span><span class="sxs-lookup"><span data-stu-id="4d869-131">type</span></span>|<span data-ttu-id="4d869-132">string</span><span class="sxs-lookup"><span data-stu-id="4d869-132">string</span></span>|<span data-ttu-id="4d869-p104">表示图表的类型。可能的值是：`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.`。</span><span class="sxs-lookup"><span data-stu-id="4d869-p104">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="4d869-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="4d869-135">sourceData</span></span>|<span data-ttu-id="4d869-136">string</span><span class="sxs-lookup"><span data-stu-id="4d869-136">string</span></span>|<span data-ttu-id="4d869-137">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="4d869-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="4d869-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="4d869-138">seriesBy</span></span>|<span data-ttu-id="4d869-139">string</span><span class="sxs-lookup"><span data-stu-id="4d869-139">string</span></span>|<span data-ttu-id="4d869-p105">可选。指定列或行在图表上用作数据系列的方式。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="4d869-p105">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="4d869-143">响应</span><span class="sxs-lookup"><span data-stu-id="4d869-143">Response</span></span>

<span data-ttu-id="4d869-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d869-144">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d869-145">示例</span><span class="sxs-lookup"><span data-stu-id="4d869-145">Example</span></span>
<span data-ttu-id="4d869-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4d869-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4d869-147">请求</span><span class="sxs-lookup"><span data-stu-id="4d869-147">Request</span></span>
<span data-ttu-id="4d869-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d869-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4d869-149">响应</span><span class="sxs-lookup"><span data-stu-id="4d869-149">Response</span></span>
<span data-ttu-id="4d869-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d869-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
