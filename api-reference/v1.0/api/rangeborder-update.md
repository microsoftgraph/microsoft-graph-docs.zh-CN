---
title: 更新 RangeBorder
description: 更新 rangeborder 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a850d4db197906b7c1c5f7986166a85143ddf544
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607999"
---
# <a name="update-rangeborder"></a><span data-ttu-id="da5cb-103">更新 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="da5cb-103">Update rangeborder</span></span>

<span data-ttu-id="da5cb-104">更新 rangeborder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da5cb-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="da5cb-105">权限</span><span class="sxs-lookup"><span data-stu-id="da5cb-105">Permissions</span></span>
<span data-ttu-id="da5cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da5cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da5cb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="da5cb-108">Permission type</span></span>      | <span data-ttu-id="da5cb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da5cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da5cb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da5cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da5cb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da5cb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da5cb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da5cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da5cb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="da5cb-113">Not supported.</span></span>    |
|<span data-ttu-id="da5cb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="da5cb-114">Application</span></span> | <span data-ttu-id="da5cb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da5cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da5cb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da5cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="da5cb-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="da5cb-117">Optional request headers</span></span>
| <span data-ttu-id="da5cb-118">名称</span><span class="sxs-lookup"><span data-stu-id="da5cb-118">Name</span></span>       | <span data-ttu-id="da5cb-119">说明</span><span class="sxs-lookup"><span data-stu-id="da5cb-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="da5cb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="da5cb-120">Authorization</span></span>  | <span data-ttu-id="da5cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da5cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da5cb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da5cb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="da5cb-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="da5cb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da5cb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da5cb-126">Request body</span></span>
<span data-ttu-id="da5cb-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="da5cb-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da5cb-130">属性</span><span class="sxs-lookup"><span data-stu-id="da5cb-130">Property</span></span>     | <span data-ttu-id="da5cb-131">类型</span><span class="sxs-lookup"><span data-stu-id="da5cb-131">Type</span></span>   |<span data-ttu-id="da5cb-132">说明</span><span class="sxs-lookup"><span data-stu-id="da5cb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da5cb-133">color</span><span class="sxs-lookup"><span data-stu-id="da5cb-133">color</span></span>|<span data-ttu-id="da5cb-134">字符串</span><span class="sxs-lookup"><span data-stu-id="da5cb-134">string</span></span>|<span data-ttu-id="da5cb-135">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="da5cb-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="da5cb-136">style</span><span class="sxs-lookup"><span data-stu-id="da5cb-136">style</span></span>|<span data-ttu-id="da5cb-137">string</span><span class="sxs-lookup"><span data-stu-id="da5cb-137">string</span></span>|<span data-ttu-id="da5cb-138">线条样式的常量之一，指定边框的线条样式。</span><span class="sxs-lookup"><span data-stu-id="da5cb-138">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="da5cb-139">可能的值为: `None`、 `Continuous`、 `Dash` `DashDot` `DashDotDot` `Dot` `Double`、、、、 `SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="da5cb-139">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="da5cb-140">weight</span><span class="sxs-lookup"><span data-stu-id="da5cb-140">weight</span></span>|<span data-ttu-id="da5cb-141">string</span><span class="sxs-lookup"><span data-stu-id="da5cb-141">string</span></span>|<span data-ttu-id="da5cb-142">指定区域周围的边框的粗细。</span><span class="sxs-lookup"><span data-stu-id="da5cb-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="da5cb-143">可能的值包括 `Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="da5cb-143">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="da5cb-144">响应</span><span class="sxs-lookup"><span data-stu-id="da5cb-144">Response</span></span>

<span data-ttu-id="da5cb-145">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[WorkbookRangeBorder](../resources/rangeborder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da5cb-145">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da5cb-146">示例</span><span class="sxs-lookup"><span data-stu-id="da5cb-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da5cb-147">请求</span><span class="sxs-lookup"><span data-stu-id="da5cb-147">Request</span></span>
<span data-ttu-id="da5cb-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da5cb-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="da5cb-149">响应</span><span class="sxs-lookup"><span data-stu-id="da5cb-149">Response</span></span>
<span data-ttu-id="da5cb-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da5cb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="da5cb-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="da5cb-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="da5cb-154">语言</span><span class="sxs-lookup"><span data-stu-id="da5cb-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_rangeborder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da5cb-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="da5cb-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_rangeborder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/rangeborder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/rangeborder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
