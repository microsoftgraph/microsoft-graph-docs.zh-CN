---
title: 获取 ChartSeries
description: 检索 chartseries 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 39d82bb06de903d8c175ff9202ccaca6821d55f3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261626"
---
# <a name="get-chartseries"></a><span data-ttu-id="5dbf9-103">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="5dbf9-103">Get ChartSeries</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dbf9-104">检索 chartseries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-104">Retrieve the properties and relationships of chartseries object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5dbf9-105">权限</span><span class="sxs-lookup"><span data-stu-id="5dbf9-105">Permissions</span></span>
<span data-ttu-id="5dbf9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dbf9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dbf9-108">Permission type</span></span>      | <span data-ttu-id="5dbf9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dbf9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dbf9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dbf9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5dbf9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dbf9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5dbf9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dbf9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dbf9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5dbf9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5dbf9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dbf9-114">Application</span></span> | <span data-ttu-id="5dbf9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dbf9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dbf9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5dbf9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5dbf9-117">Optional query parameters</span></span>
<span data-ttu-id="5dbf9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dbf9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dbf9-119">Request headers</span></span>
| <span data-ttu-id="5dbf9-120">名称</span><span class="sxs-lookup"><span data-stu-id="5dbf9-120">Name</span></span>      |<span data-ttu-id="5dbf9-121">说明</span><span class="sxs-lookup"><span data-stu-id="5dbf9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5dbf9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dbf9-122">Authorization</span></span>  | <span data-ttu-id="5dbf9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5dbf9-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5dbf9-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="5dbf9-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dbf9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dbf9-128">Request body</span></span>
<span data-ttu-id="5dbf9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dbf9-130">响应</span><span class="sxs-lookup"><span data-stu-id="5dbf9-130">Response</span></span>

<span data-ttu-id="5dbf9-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookChartSeries](../resources/workbookchartseries.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-131">If successful, this method returns a `200 OK` response code and [workbookChartSeries](../resources/workbookchartseries.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5dbf9-132">示例</span><span class="sxs-lookup"><span data-stu-id="5dbf9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5dbf9-133">请求</span><span class="sxs-lookup"><span data-stu-id="5dbf9-133">Request</span></span>
<span data-ttu-id="5dbf9-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartseries"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}
```
##### <a name="response"></a><span data-ttu-id="5dbf9-135">响应</span><span class="sxs-lookup"><span data-stu-id="5dbf9-135">Response</span></span>
<span data-ttu-id="5dbf9-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5dbf9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5dbf9-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="5dbf9-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5dbf9-140">C#</span><span class="sxs-lookup"><span data-stu-id="5dbf9-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chartseries-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dbf9-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="5dbf9-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chartseries-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5dbf9-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="5dbf9-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chartseries-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get ChartSeries",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartseries-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chartseries-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartseries-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
