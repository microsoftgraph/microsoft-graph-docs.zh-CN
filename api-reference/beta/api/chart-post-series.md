---
title: 创建 ChartSeries
description: 使用此 API 创建新 ChartSeries。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 2a528321a9b6cb1ffd40065d28122e44ae4a73a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983185"
---
# <a name="create-chartseries"></a><span data-ttu-id="9c94b-103">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="9c94b-103">Create ChartSeries</span></span>

<span data-ttu-id="9c94b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c94b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c94b-105">使用此 API 创建新 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="9c94b-105">Use this API to create a new ChartSeries.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c94b-106">权限</span><span class="sxs-lookup"><span data-stu-id="9c94b-106">Permissions</span></span>
<span data-ttu-id="9c94b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c94b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c94b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c94b-109">Permission type</span></span>      | <span data-ttu-id="9c94b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c94b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c94b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c94b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c94b-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c94b-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c94b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c94b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c94b-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c94b-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c94b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c94b-115">Application</span></span> | <span data-ttu-id="9c94b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c94b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c94b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c94b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/series

```
## <a name="request-headers"></a><span data-ttu-id="9c94b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c94b-118">Request headers</span></span>
| <span data-ttu-id="9c94b-119">名称</span><span class="sxs-lookup"><span data-stu-id="9c94b-119">Name</span></span>       | <span data-ttu-id="9c94b-120">说明</span><span class="sxs-lookup"><span data-stu-id="9c94b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9c94b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c94b-121">Authorization</span></span>  | <span data-ttu-id="9c94b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c94b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c94b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9c94b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9c94b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9c94b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c94b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c94b-127">Request body</span></span>
<span data-ttu-id="9c94b-128">在请求正文中，提供 [workbookChartSeries](../resources/workbookchartseries.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c94b-128">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9c94b-129">响应</span><span class="sxs-lookup"><span data-stu-id="9c94b-129">Response</span></span>

<span data-ttu-id="9c94b-130">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [workbookChartSeries](../resources/workbookchartseries.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c94b-130">If successful, this method returns `201 Created` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c94b-131">示例</span><span class="sxs-lookup"><span data-stu-id="9c94b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c94b-132">请求</span><span class="sxs-lookup"><span data-stu-id="9c94b-132">Request</span></span>
<span data-ttu-id="9c94b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c94b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c94b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c94b-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9c94b-135">C#</span><span class="sxs-lookup"><span data-stu-id="9c94b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chartseries-from-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c94b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c94b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chartseries-from-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c94b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c94b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chartseries-from-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9c94b-138">在请求正文中，提供 [workbookChartSeries](../resources/workbookchartseries.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c94b-138">In the request body, supply a JSON representation of [workbookChartSeries](../resources/workbookchartseries.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9c94b-139">响应</span><span class="sxs-lookup"><span data-stu-id="9c94b-139">Response</span></span>
<span data-ttu-id="9c94b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c94b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->


