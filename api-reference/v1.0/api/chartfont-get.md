---
title: 获取 ChartFont
description: 检索 chartfont 对象的属性和关系。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4e6a71955891147f311f50cd35f0ba25df91fa88
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272476"
---
# <a name="get-chartfont"></a><span data-ttu-id="41adf-103">获取 ChartFont</span><span class="sxs-lookup"><span data-stu-id="41adf-103">Get ChartFont</span></span>

<span data-ttu-id="41adf-104">检索 chartfont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41adf-104">Retrieve the properties and relationships of chartfont object.</span></span>
## <a name="permissions"></a><span data-ttu-id="41adf-105">权限</span><span class="sxs-lookup"><span data-stu-id="41adf-105">Permissions</span></span>
<span data-ttu-id="41adf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41adf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="41adf-108">Permission type</span></span>      | <span data-ttu-id="41adf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41adf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41adf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41adf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41adf-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41adf-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="41adf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41adf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41adf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="41adf-113">Not supported.</span></span>    |
|<span data-ttu-id="41adf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="41adf-114">Application</span></span> | <span data-ttu-id="41adf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41adf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41adf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41adf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/font
GET /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/font
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41adf-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41adf-117">Optional query parameters</span></span>
<span data-ttu-id="41adf-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41adf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41adf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41adf-119">Request headers</span></span>
| <span data-ttu-id="41adf-120">名称</span><span class="sxs-lookup"><span data-stu-id="41adf-120">Name</span></span>      |<span data-ttu-id="41adf-121">说明</span><span class="sxs-lookup"><span data-stu-id="41adf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41adf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41adf-122">Authorization</span></span>  | <span data-ttu-id="41adf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41adf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="41adf-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="41adf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="41adf-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="41adf-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="41adf-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="41adf-128">Request body</span></span>
<span data-ttu-id="41adf-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41adf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41adf-130">响应</span><span class="sxs-lookup"><span data-stu-id="41adf-130">Response</span></span>

<span data-ttu-id="41adf-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[WorkbookChartFont](../resources/chartfont.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41adf-131">If successful, this method returns a `200 OK` response code and [WorkbookChartFont](../resources/chartfont.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41adf-132">示例</span><span class="sxs-lookup"><span data-stu-id="41adf-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41adf-133">请求</span><span class="sxs-lookup"><span data-stu-id="41adf-133">Request</span></span>
<span data-ttu-id="41adf-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41adf-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_chartfont"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font
```
##### <a name="response"></a><span data-ttu-id="41adf-135">响应</span><span class="sxs-lookup"><span data-stu-id="41adf-135">Response</span></span>
<span data-ttu-id="41adf-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41adf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartFont"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "bold": true,
  "color": "color-value",
  "italic": true,
  "name": "name-value",
  "size": 99,
  "underline": "underline-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="41adf-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="41adf-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="41adf-140">C#</span><span class="sxs-lookup"><span data-stu-id="41adf-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_chartfont-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41adf-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="41adf-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_chartfont-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="41adf-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="41adf-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_chartfont-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get ChartFont",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartfont-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartfont-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartfont-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
