---
title: 更新图表
description: 更新 chart 对象的属性。
author: lumine2008
ms.openlocfilehash: 086d4a2ea0ce823ace141df0d5576af732bf8c0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328180"
---
# <a name="update-chart"></a><span data-ttu-id="765e0-103">更新图表</span><span class="sxs-lookup"><span data-stu-id="765e0-103">Update chart</span></span>

> <span data-ttu-id="765e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="765e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="765e0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="765e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="765e0-106">更新 chart 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="765e0-106">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="765e0-107">权限</span><span class="sxs-lookup"><span data-stu-id="765e0-107">Permissions</span></span>
<span data-ttu-id="765e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="765e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="765e0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="765e0-110">Permission type</span></span>      | <span data-ttu-id="765e0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="765e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="765e0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="765e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="765e0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="765e0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="765e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="765e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="765e0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="765e0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="765e0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="765e0-116">Application</span></span> | <span data-ttu-id="765e0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="765e0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="765e0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="765e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="765e0-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="765e0-119">Optional request headers</span></span>
| <span data-ttu-id="765e0-120">Name</span><span class="sxs-lookup"><span data-stu-id="765e0-120">Name</span></span>       | <span data-ttu-id="765e0-121">说明</span><span class="sxs-lookup"><span data-stu-id="765e0-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="765e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="765e0-122">Authorization</span></span>  | <span data-ttu-id="765e0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="765e0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="765e0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="765e0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="765e0-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="765e0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="765e0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="765e0-128">Request body</span></span>
<span data-ttu-id="765e0-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="765e0-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="765e0-132">属性</span><span class="sxs-lookup"><span data-stu-id="765e0-132">Property</span></span>     | <span data-ttu-id="765e0-133">类型</span><span class="sxs-lookup"><span data-stu-id="765e0-133">Type</span></span>   |<span data-ttu-id="765e0-134">说明</span><span class="sxs-lookup"><span data-stu-id="765e0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="765e0-135">height</span><span class="sxs-lookup"><span data-stu-id="765e0-135">height</span></span>|<span data-ttu-id="765e0-136">double</span><span class="sxs-lookup"><span data-stu-id="765e0-136">double</span></span>|<span data-ttu-id="765e0-137">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="765e0-137">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="765e0-138">left</span><span class="sxs-lookup"><span data-stu-id="765e0-138">left</span></span>|<span data-ttu-id="765e0-139">double</span><span class="sxs-lookup"><span data-stu-id="765e0-139">double</span></span>|<span data-ttu-id="765e0-140">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="765e0-140">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="765e0-141">name</span><span class="sxs-lookup"><span data-stu-id="765e0-141">name</span></span>|<span data-ttu-id="765e0-142">string</span><span class="sxs-lookup"><span data-stu-id="765e0-142">string</span></span>|<span data-ttu-id="765e0-143">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="765e0-143">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="765e0-144">top</span><span class="sxs-lookup"><span data-stu-id="765e0-144">top</span></span>|<span data-ttu-id="765e0-145">double</span><span class="sxs-lookup"><span data-stu-id="765e0-145">double</span></span>|<span data-ttu-id="765e0-146">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="765e0-146">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="765e0-147">width</span><span class="sxs-lookup"><span data-stu-id="765e0-147">width</span></span>|<span data-ttu-id="765e0-148">double</span><span class="sxs-lookup"><span data-stu-id="765e0-148">double</span></span>|<span data-ttu-id="765e0-149">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="765e0-149">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="765e0-150">响应</span><span class="sxs-lookup"><span data-stu-id="765e0-150">Response</span></span>

<span data-ttu-id="765e0-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Chart](../resources/chart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="765e0-151">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="765e0-152">示例</span><span class="sxs-lookup"><span data-stu-id="765e0-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="765e0-153">请求</span><span class="sxs-lookup"><span data-stu-id="765e0-153">Request</span></span>
<span data-ttu-id="765e0-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="765e0-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="765e0-155">响应</span><span class="sxs-lookup"><span data-stu-id="765e0-155">Response</span></span>
<span data-ttu-id="765e0-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="765e0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->