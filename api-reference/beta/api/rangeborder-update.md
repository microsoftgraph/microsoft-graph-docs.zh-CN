---
title: 更新 RangeBorder
description: 更新 rangeborder 对象的属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 99db19208242ae25c94c081b4e43f9f8caa47e67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877054"
---
# <a name="update-rangeborder"></a><span data-ttu-id="a72a3-103">更新 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="a72a3-103">Update rangeborder</span></span>

> <span data-ttu-id="a72a3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a72a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a72a3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a72a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a72a3-106">更新 rangeborder 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a72a3-106">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a72a3-107">权限</span><span class="sxs-lookup"><span data-stu-id="a72a3-107">Permissions</span></span>
<span data-ttu-id="a72a3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a72a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a72a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a72a3-110">Permission type</span></span>      | <span data-ttu-id="a72a3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a72a3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a72a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a72a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a72a3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a72a3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a72a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a72a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a72a3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a72a3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a72a3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a72a3-116">Application</span></span> | <span data-ttu-id="a72a3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a72a3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a72a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a72a3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="a72a3-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a72a3-119">Optional request headers</span></span>
| <span data-ttu-id="a72a3-120">名称</span><span class="sxs-lookup"><span data-stu-id="a72a3-120">Name</span></span>       | <span data-ttu-id="a72a3-121">说明</span><span class="sxs-lookup"><span data-stu-id="a72a3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a72a3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a72a3-122">Authorization</span></span>  | <span data-ttu-id="a72a3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a72a3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a72a3-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a72a3-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a72a3-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a72a3-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a72a3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a72a3-128">Request body</span></span>
<span data-ttu-id="a72a3-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a72a3-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a72a3-132">属性</span><span class="sxs-lookup"><span data-stu-id="a72a3-132">Property</span></span>     | <span data-ttu-id="a72a3-133">类型</span><span class="sxs-lookup"><span data-stu-id="a72a3-133">Type</span></span>   |<span data-ttu-id="a72a3-134">说明</span><span class="sxs-lookup"><span data-stu-id="a72a3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a72a3-135">color</span><span class="sxs-lookup"><span data-stu-id="a72a3-135">color</span></span>|<span data-ttu-id="a72a3-136">string</span><span class="sxs-lookup"><span data-stu-id="a72a3-136">string</span></span>|<span data-ttu-id="a72a3-137">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="a72a3-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="a72a3-138">style</span><span class="sxs-lookup"><span data-stu-id="a72a3-138">style</span></span>|<span data-ttu-id="a72a3-139">string</span><span class="sxs-lookup"><span data-stu-id="a72a3-139">string</span></span>|<span data-ttu-id="a72a3-p106">线条样式的常量之一，指定边框的线条样式。可能的值是：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="a72a3-p106">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="a72a3-142">weight</span><span class="sxs-lookup"><span data-stu-id="a72a3-142">weight</span></span>|<span data-ttu-id="a72a3-143">string</span><span class="sxs-lookup"><span data-stu-id="a72a3-143">string</span></span>|<span data-ttu-id="a72a3-p107">指定区域周围边框的权重。可能的值是：`Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="a72a3-p107">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="a72a3-146">响应</span><span class="sxs-lookup"><span data-stu-id="a72a3-146">Response</span></span>

<span data-ttu-id="a72a3-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [RangeBorder](../resources/rangeborder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a72a3-147">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a72a3-148">示例</span><span class="sxs-lookup"><span data-stu-id="a72a3-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a72a3-149">请求</span><span class="sxs-lookup"><span data-stu-id="a72a3-149">Request</span></span>
<span data-ttu-id="a72a3-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a72a3-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="a72a3-151">响应</span><span class="sxs-lookup"><span data-stu-id="a72a3-151">Response</span></span>
<span data-ttu-id="a72a3-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a72a3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
