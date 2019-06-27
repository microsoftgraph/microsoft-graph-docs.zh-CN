---
title: 'Chart: setData'
description: 重置图表的源数据。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c7f95c83a2eeee77f66dd347b353a585fadbb16f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261948"
---
# <a name="chart-setdata"></a><span data-ttu-id="2b939-103">Chart: setData</span><span class="sxs-lookup"><span data-stu-id="2b939-103">Chart: setData</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b939-104">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="2b939-104">Resets the source data for the chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b939-105">权限</span><span class="sxs-lookup"><span data-stu-id="2b939-105">Permissions</span></span>
<span data-ttu-id="2b939-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b939-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b939-108">Permission type</span></span>      | <span data-ttu-id="2b939-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b939-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b939-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b939-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b939-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b939-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2b939-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b939-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b939-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b939-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2b939-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b939-114">Application</span></span> | <span data-ttu-id="2b939-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b939-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b939-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b939-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/setData

```
## <a name="request-headers"></a><span data-ttu-id="2b939-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b939-117">Request headers</span></span>
| <span data-ttu-id="2b939-118">名称</span><span class="sxs-lookup"><span data-stu-id="2b939-118">Name</span></span>       | <span data-ttu-id="2b939-119">说明</span><span class="sxs-lookup"><span data-stu-id="2b939-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b939-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b939-120">Authorization</span></span>  | <span data-ttu-id="2b939-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b939-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b939-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2b939-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2b939-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="2b939-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b939-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b939-126">Request body</span></span>
<span data-ttu-id="2b939-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2b939-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b939-128">参数</span><span class="sxs-lookup"><span data-stu-id="2b939-128">Parameter</span></span>    | <span data-ttu-id="2b939-129">类型</span><span class="sxs-lookup"><span data-stu-id="2b939-129">Type</span></span>   |<span data-ttu-id="2b939-130">说明</span><span class="sxs-lookup"><span data-stu-id="2b939-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b939-131">sourceData</span><span class="sxs-lookup"><span data-stu-id="2b939-131">sourceData</span></span>|<span data-ttu-id="2b939-132">string</span><span class="sxs-lookup"><span data-stu-id="2b939-132">string</span></span>|<span data-ttu-id="2b939-133">对应于源数据的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="2b939-133">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="2b939-134">seriesBy</span><span class="sxs-lookup"><span data-stu-id="2b939-134">seriesBy</span></span>|<span data-ttu-id="2b939-135">string</span><span class="sxs-lookup"><span data-stu-id="2b939-135">string</span></span>|<span data-ttu-id="2b939-p104">可选。指定列或行在图表上用作数据系列的方式。可以是下列值之一：自动（默认）、行、列。可能的值是：`Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="2b939-p104">Optional. Specifies the way columns or rows are used as data series on the chart. Can be one of the following: Auto (default), Rows, Columns.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="2b939-140">响应</span><span class="sxs-lookup"><span data-stu-id="2b939-140">Response</span></span>

<span data-ttu-id="2b939-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2b939-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b939-143">示例</span><span class="sxs-lookup"><span data-stu-id="2b939-143">Example</span></span>
<span data-ttu-id="2b939-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2b939-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2b939-145">请求</span><span class="sxs-lookup"><span data-stu-id="2b939-145">Request</span></span>
<span data-ttu-id="2b939-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b939-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="2b939-147">响应</span><span class="sxs-lookup"><span data-stu-id="2b939-147">Response</span></span>
<span data-ttu-id="2b939-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2b939-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2b939-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2b939-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2b939-150">C#</span><span class="sxs-lookup"><span data-stu-id="2b939-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chart_setdata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b939-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b939-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chart_setdata-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2b939-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="2b939-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/chart_setdata-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-setdata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
