---
title: 'workbookChartCollection: 添加'
description: 创建新的 workbookChart。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 44b2ad6ae9e67beced215eba9a130da0d418e5a3
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635699"
---
# <a name="workbookchartcollection-add"></a><span data-ttu-id="3507c-103">workbookChartCollection: 添加</span><span class="sxs-lookup"><span data-stu-id="3507c-103">workbookChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3507c-104">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="3507c-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="3507c-105">权限</span><span class="sxs-lookup"><span data-stu-id="3507c-105">Permissions</span></span>
<span data-ttu-id="3507c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3507c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3507c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3507c-108">Permission type</span></span>      | <span data-ttu-id="3507c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3507c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3507c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3507c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3507c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3507c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3507c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3507c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3507c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3507c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3507c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3507c-114">Application</span></span> | <span data-ttu-id="3507c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3507c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3507c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3507c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="3507c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3507c-117">Request headers</span></span>
| <span data-ttu-id="3507c-118">名称</span><span class="sxs-lookup"><span data-stu-id="3507c-118">Name</span></span>       | <span data-ttu-id="3507c-119">说明</span><span class="sxs-lookup"><span data-stu-id="3507c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3507c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3507c-120">Authorization</span></span>  | <span data-ttu-id="3507c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3507c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3507c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3507c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="3507c-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3507c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3507c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3507c-126">Request body</span></span>
<span data-ttu-id="3507c-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3507c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3507c-128">参数</span><span class="sxs-lookup"><span data-stu-id="3507c-128">Parameter</span></span>    | <span data-ttu-id="3507c-129">类型</span><span class="sxs-lookup"><span data-stu-id="3507c-129">Type</span></span>   |<span data-ttu-id="3507c-130">说明</span><span class="sxs-lookup"><span data-stu-id="3507c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3507c-131">类型</span><span class="sxs-lookup"><span data-stu-id="3507c-131">type</span></span>|<span data-ttu-id="3507c-132">string</span><span class="sxs-lookup"><span data-stu-id="3507c-132">string</span></span>|<span data-ttu-id="3507c-133">表示图表的类型。</span><span class="sxs-lookup"><span data-stu-id="3507c-133">Represents the type of a chart.</span></span>  <span data-ttu-id="3507c-134">可能的值为: `ColumnClustered`、 `ColumnStacked`、 `ColumnStacked100` `BarClustered` `BarStacked` `BarStacked100` `LineStacked` `PieOfPie` `etc.`、、、、、、、、、、。 `LineStacked100` `LineMarkers` `LineMarkersStacked` `LineMarkersStacked100`</span><span class="sxs-lookup"><span data-stu-id="3507c-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="3507c-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="3507c-135">sourceData</span></span>|<span data-ttu-id="3507c-136">Json</span><span class="sxs-lookup"><span data-stu-id="3507c-136">Json</span></span>|<span data-ttu-id="3507c-137">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="3507c-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="3507c-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="3507c-138">seriesBy</span></span>|<span data-ttu-id="3507c-139">字符串</span><span class="sxs-lookup"><span data-stu-id="3507c-139">string</span></span>|<span data-ttu-id="3507c-140">可选。</span><span class="sxs-lookup"><span data-stu-id="3507c-140">Optional.</span></span> <span data-ttu-id="3507c-141">指定列或行在图表上用作数据系列的方式。</span><span class="sxs-lookup"><span data-stu-id="3507c-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="3507c-142">可能的值包括 `Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="3507c-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="3507c-143">响应</span><span class="sxs-lookup"><span data-stu-id="3507c-143">Response</span></span>

<span data-ttu-id="3507c-144">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[workbookChart](../resources/workbookchart.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3507c-144">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3507c-145">示例</span><span class="sxs-lookup"><span data-stu-id="3507c-145">Example</span></span>
<span data-ttu-id="3507c-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3507c-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3507c-147">请求</span><span class="sxs-lookup"><span data-stu-id="3507c-147">Request</span></span>
<span data-ttu-id="3507c-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3507c-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3507c-149">响应</span><span class="sxs-lookup"><span data-stu-id="3507c-149">Response</span></span>
<span data-ttu-id="3507c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3507c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3507c-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3507c-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3507c-154">语言</span><span class="sxs-lookup"><span data-stu-id="3507c-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chartcollection_add-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3507c-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="3507c-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartcollection_add-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
