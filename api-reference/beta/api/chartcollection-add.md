---
title: workbookChartCollection： add
description: 创建新的 workbookChart。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d81bdb08f5efa503e56961b2bb5fdba694c5aba4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047460"
---
# <a name="workbookchartcollection-add"></a><span data-ttu-id="5ceae-103">workbookChartCollection： add</span><span class="sxs-lookup"><span data-stu-id="5ceae-103">workbookChartCollection: add</span></span>

<span data-ttu-id="5ceae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ceae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ceae-105">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="5ceae-105">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ceae-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ceae-106">Permissions</span></span>
<span data-ttu-id="5ceae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ceae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ceae-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ceae-109">Permission type</span></span>      | <span data-ttu-id="5ceae-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ceae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ceae-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ceae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ceae-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ceae-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ceae-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ceae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ceae-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ceae-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5ceae-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ceae-115">Application</span></span> | <span data-ttu-id="5ceae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ceae-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ceae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ceae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="5ceae-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ceae-118">Request headers</span></span>
| <span data-ttu-id="5ceae-119">名称</span><span class="sxs-lookup"><span data-stu-id="5ceae-119">Name</span></span>       | <span data-ttu-id="5ceae-120">说明</span><span class="sxs-lookup"><span data-stu-id="5ceae-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5ceae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ceae-121">Authorization</span></span>  | <span data-ttu-id="5ceae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ceae-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ceae-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5ceae-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="5ceae-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5ceae-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ceae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ceae-127">Request body</span></span>
<span data-ttu-id="5ceae-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5ceae-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5ceae-129">参数</span><span class="sxs-lookup"><span data-stu-id="5ceae-129">Parameter</span></span>    | <span data-ttu-id="5ceae-130">类型</span><span class="sxs-lookup"><span data-stu-id="5ceae-130">Type</span></span>   |<span data-ttu-id="5ceae-131">说明</span><span class="sxs-lookup"><span data-stu-id="5ceae-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ceae-132">类型</span><span class="sxs-lookup"><span data-stu-id="5ceae-132">type</span></span>|<span data-ttu-id="5ceae-133">string</span><span class="sxs-lookup"><span data-stu-id="5ceae-133">string</span></span>|<span data-ttu-id="5ceae-134">表示图表的类型。</span><span class="sxs-lookup"><span data-stu-id="5ceae-134">Represents the type of a chart.</span></span>  <span data-ttu-id="5ceae-135">可能的值是 `ColumnClustered` `ColumnStacked` `ColumnStacked100` `BarClustered` `BarStacked` `BarStacked100` ：、、、、、、、。 `LineStacked` `LineStacked100` `LineMarkers` `LineMarkersStacked` `LineMarkersStacked100` `PieOfPie` `etc.`</span><span class="sxs-lookup"><span data-stu-id="5ceae-135">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="5ceae-136">sourceData</span><span class="sxs-lookup"><span data-stu-id="5ceae-136">sourceData</span></span>|<span data-ttu-id="5ceae-137">Json</span><span class="sxs-lookup"><span data-stu-id="5ceae-137">Json</span></span>|<span data-ttu-id="5ceae-138">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="5ceae-138">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="5ceae-139">seriesBy</span><span class="sxs-lookup"><span data-stu-id="5ceae-139">seriesBy</span></span>|<span data-ttu-id="5ceae-140">string</span><span class="sxs-lookup"><span data-stu-id="5ceae-140">string</span></span>|<span data-ttu-id="5ceae-141">可选。</span><span class="sxs-lookup"><span data-stu-id="5ceae-141">Optional.</span></span> <span data-ttu-id="5ceae-142">指定列或行在图表上用作数据系列的方式。</span><span class="sxs-lookup"><span data-stu-id="5ceae-142">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="5ceae-143">可能的值包括 `Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="5ceae-143">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="5ceae-144">响应</span><span class="sxs-lookup"><span data-stu-id="5ceae-144">Response</span></span>

<span data-ttu-id="5ceae-145">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [workbookChart](../resources/workbookchart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ceae-145">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ceae-146">示例</span><span class="sxs-lookup"><span data-stu-id="5ceae-146">Example</span></span>
<span data-ttu-id="5ceae-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5ceae-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5ceae-148">请求</span><span class="sxs-lookup"><span data-stu-id="5ceae-148">Request</span></span>
<span data-ttu-id="5ceae-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ceae-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ceae-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ceae-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ceae-151">C#</span><span class="sxs-lookup"><span data-stu-id="5ceae-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ceae-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ceae-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ceae-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ceae-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ceae-154">Java</span><span class="sxs-lookup"><span data-stu-id="5ceae-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ceae-155">响应</span><span class="sxs-lookup"><span data-stu-id="5ceae-155">Response</span></span>
<span data-ttu-id="5ceae-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ceae-156">Here is an example of the response.</span></span> <span data-ttu-id="5ceae-157">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5ceae-157">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


