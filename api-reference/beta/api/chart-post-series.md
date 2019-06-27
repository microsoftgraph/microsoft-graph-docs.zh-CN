---
title: 创建 ChartSeries
description: 使用此 API 创建新 ChartSeries。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8a30801e31f8940efd318095fe70d6e3a2685e20
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261969"
---
# <a name="create-chartseries"></a><span data-ttu-id="43edf-103">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="43edf-103">Create ChartSeries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43edf-104">使用此 API 创建新 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="43edf-104">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="43edf-105">权限</span><span class="sxs-lookup"><span data-stu-id="43edf-105">Permissions</span></span>
<span data-ttu-id="43edf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43edf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43edf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="43edf-108">Permission type</span></span>      | <span data-ttu-id="43edf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43edf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43edf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43edf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="43edf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43edf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="43edf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43edf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43edf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43edf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="43edf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="43edf-114">Application</span></span> | <span data-ttu-id="43edf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="43edf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43edf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43edf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="43edf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="43edf-117">Request headers</span></span>
| <span data-ttu-id="43edf-118">名称</span><span class="sxs-lookup"><span data-stu-id="43edf-118">Name</span></span>       | <span data-ttu-id="43edf-119">说明</span><span class="sxs-lookup"><span data-stu-id="43edf-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="43edf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="43edf-120">Authorization</span></span>  | <span data-ttu-id="43edf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="43edf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43edf-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="43edf-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="43edf-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="43edf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43edf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="43edf-126">Request body</span></span>
<span data-ttu-id="43edf-127">在请求正文中, 提供[workbookChartSeries](../resources/workbookchartseries.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43edf-127">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="43edf-128">响应</span><span class="sxs-lookup"><span data-stu-id="43edf-128">Response</span></span>

<span data-ttu-id="43edf-129">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[workbookChartSeries](../resources/workbookchartseries.md)对象。</span><span class="sxs-lookup"><span data-stu-id="43edf-129">If successful, this method returns `201 Created` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43edf-130">示例</span><span class="sxs-lookup"><span data-stu-id="43edf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43edf-131">请求</span><span class="sxs-lookup"><span data-stu-id="43edf-131">Request</span></span>
<span data-ttu-id="43edf-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43edf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chartseries_from_chart"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
<span data-ttu-id="43edf-133">在请求正文中, 提供[workbookChartSeries](../resources/workbookchartseries.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43edf-133">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="43edf-134">响应</span><span class="sxs-lookup"><span data-stu-id="43edf-134">Response</span></span>
<span data-ttu-id="43edf-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43edf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartSeries"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="43edf-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="43edf-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="43edf-139">C#</span><span class="sxs-lookup"><span data-stu-id="43edf-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chartseries_from_chart-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43edf-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="43edf-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chartseries_from_chart-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="43edf-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="43edf-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chartseries_from_chart-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-post-series.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chart-post-series.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chart-post-series.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
