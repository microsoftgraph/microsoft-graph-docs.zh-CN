---
title: 更新 RangeBorder
description: 更新 rangeborder 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 0c6f6d53cddacc5e54031aaa9830f15b1573814d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454640"
---
# <a name="update-rangeborder"></a><span data-ttu-id="c51b6-103">更新 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="c51b6-103">Update rangeborder</span></span>

<span data-ttu-id="c51b6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c51b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c51b6-105">更新 rangeborder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c51b6-105">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c51b6-106">权限</span><span class="sxs-lookup"><span data-stu-id="c51b6-106">Permissions</span></span>
<span data-ttu-id="c51b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c51b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c51b6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c51b6-109">Permission type</span></span>      | <span data-ttu-id="c51b6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c51b6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c51b6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c51b6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c51b6-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c51b6-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c51b6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c51b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c51b6-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c51b6-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c51b6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c51b6-115">Application</span></span> | <span data-ttu-id="c51b6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c51b6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c51b6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c51b6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="c51b6-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c51b6-118">Optional request headers</span></span>
| <span data-ttu-id="c51b6-119">名称</span><span class="sxs-lookup"><span data-stu-id="c51b6-119">Name</span></span>       | <span data-ttu-id="c51b6-120">说明</span><span class="sxs-lookup"><span data-stu-id="c51b6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c51b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c51b6-121">Authorization</span></span>  | <span data-ttu-id="c51b6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c51b6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c51b6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c51b6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c51b6-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c51b6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c51b6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c51b6-127">Request body</span></span>
<span data-ttu-id="c51b6-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c51b6-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c51b6-131">属性</span><span class="sxs-lookup"><span data-stu-id="c51b6-131">Property</span></span>     | <span data-ttu-id="c51b6-132">类型</span><span class="sxs-lookup"><span data-stu-id="c51b6-132">Type</span></span>   |<span data-ttu-id="c51b6-133">说明</span><span class="sxs-lookup"><span data-stu-id="c51b6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c51b6-134">color</span><span class="sxs-lookup"><span data-stu-id="c51b6-134">color</span></span>|<span data-ttu-id="c51b6-135">字符串</span><span class="sxs-lookup"><span data-stu-id="c51b6-135">string</span></span>|<span data-ttu-id="c51b6-136">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="c51b6-136">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="c51b6-137">style</span><span class="sxs-lookup"><span data-stu-id="c51b6-137">style</span></span>|<span data-ttu-id="c51b6-138">string</span><span class="sxs-lookup"><span data-stu-id="c51b6-138">string</span></span>|<span data-ttu-id="c51b6-p105">线条样式的常量之一，指定边框的线条样式。可能的值是：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="c51b6-p105">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="c51b6-141">weight</span><span class="sxs-lookup"><span data-stu-id="c51b6-141">weight</span></span>|<span data-ttu-id="c51b6-142">string</span><span class="sxs-lookup"><span data-stu-id="c51b6-142">string</span></span>|<span data-ttu-id="c51b6-p106">指定区域周围边框的权重。可能的值是：`Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="c51b6-p106">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="c51b6-145">响应</span><span class="sxs-lookup"><span data-stu-id="c51b6-145">Response</span></span>

<span data-ttu-id="c51b6-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[workbookRangeBorder](../resources/workbookrangeborder.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c51b6-146">If successful, this method returns a `200 OK` response code and updated [workbookRangeBorder](../resources/workbookrangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c51b6-147">示例</span><span class="sxs-lookup"><span data-stu-id="c51b6-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c51b6-148">请求</span><span class="sxs-lookup"><span data-stu-id="c51b6-148">Request</span></span>
<span data-ttu-id="c51b6-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c51b6-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c51b6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="c51b6-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
# <a name="c"></a>[<span data-ttu-id="c51b6-151">C#</span><span class="sxs-lookup"><span data-stu-id="c51b6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-rangeborder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c51b6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c51b6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-rangeborder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c51b6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c51b6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-rangeborder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c51b6-154">响应</span><span class="sxs-lookup"><span data-stu-id="c51b6-154">Response</span></span>
<span data-ttu-id="c51b6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c51b6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
