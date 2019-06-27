---
title: 更新 chartlineformat
description: 更新 chartlineformat 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e3da69e44fb8736543e46696099928cbe71cb62c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264706"
---
# <a name="update-chartlineformat"></a><span data-ttu-id="27eee-103">更新 chartlineformat</span><span class="sxs-lookup"><span data-stu-id="27eee-103">Update chartlineformat</span></span>

<span data-ttu-id="27eee-104">更新 chartlineformat 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27eee-104">Update the properties of chartlineformat object.</span></span>
## <a name="permissions"></a><span data-ttu-id="27eee-105">权限</span><span class="sxs-lookup"><span data-stu-id="27eee-105">Permissions</span></span>
<span data-ttu-id="27eee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27eee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27eee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="27eee-108">Permission type</span></span>      | <span data-ttu-id="27eee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27eee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27eee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27eee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27eee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27eee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="27eee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27eee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27eee-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="27eee-113">Not supported.</span></span>    |
|<span data-ttu-id="27eee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="27eee-114">Application</span></span> | <span data-ttu-id="27eee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27eee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27eee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27eee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line
PATCH /workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/majorgridlines/format/line
```
## <a name="optional-request-headers"></a><span data-ttu-id="27eee-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="27eee-117">Optional request headers</span></span>
| <span data-ttu-id="27eee-118">名称</span><span class="sxs-lookup"><span data-stu-id="27eee-118">Name</span></span>       | <span data-ttu-id="27eee-119">说明</span><span class="sxs-lookup"><span data-stu-id="27eee-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="27eee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="27eee-120">Authorization</span></span>  | <span data-ttu-id="27eee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27eee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27eee-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="27eee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="27eee-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="27eee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27eee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="27eee-126">Request body</span></span>
<span data-ttu-id="27eee-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="27eee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="27eee-130">属性</span><span class="sxs-lookup"><span data-stu-id="27eee-130">Property</span></span>     | <span data-ttu-id="27eee-131">类型</span><span class="sxs-lookup"><span data-stu-id="27eee-131">Type</span></span>   |<span data-ttu-id="27eee-132">说明</span><span class="sxs-lookup"><span data-stu-id="27eee-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27eee-133">color</span><span class="sxs-lookup"><span data-stu-id="27eee-133">color</span></span>|<span data-ttu-id="27eee-134">string</span><span class="sxs-lookup"><span data-stu-id="27eee-134">string</span></span>|<span data-ttu-id="27eee-135">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="27eee-135">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="response"></a><span data-ttu-id="27eee-136">响应</span><span class="sxs-lookup"><span data-stu-id="27eee-136">Response</span></span>

<span data-ttu-id="27eee-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookChartLineFormat](../resources/chartlineformat.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27eee-137">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLineFormat](../resources/chartlineformat.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="27eee-138">示例</span><span class="sxs-lookup"><span data-stu-id="27eee-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27eee-139">请求</span><span class="sxs-lookup"><span data-stu-id="27eee-139">Request</span></span>
<span data-ttu-id="27eee-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27eee-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlineformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="27eee-141">响应</span><span class="sxs-lookup"><span data-stu-id="27eee-141">Response</span></span>
<span data-ttu-id="27eee-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27eee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="27eee-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="27eee-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="27eee-146">C#</span><span class="sxs-lookup"><span data-stu-id="27eee-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_chartlineformat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27eee-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="27eee-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_chartlineformat-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="27eee-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="27eee-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_chartlineformat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlineformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/chartlineformat-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/chartlineformat-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/chartlineformat-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
