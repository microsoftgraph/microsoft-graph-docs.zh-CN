---
title: 更新图表
description: 更新 chart 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 7e733fbf1f9612bfdaf1d98cdc8d1aca049353cf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418584"
---
# <a name="update-chart"></a><span data-ttu-id="8f4ba-103">更新图表</span><span class="sxs-lookup"><span data-stu-id="8f4ba-103">Update chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f4ba-104">更新 chart 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f4ba-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f4ba-105">Permissions</span></span>
<span data-ttu-id="8f4ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f4ba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f4ba-108">Permission type</span></span>      | <span data-ttu-id="8f4ba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f4ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f4ba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f4ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f4ba-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ba-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f4ba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f4ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f4ba-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f4ba-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8f4ba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f4ba-114">Application</span></span> | <span data-ttu-id="8f4ba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f4ba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f4ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8f4ba-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="8f4ba-117">Optional request headers</span></span>
| <span data-ttu-id="8f4ba-118">名称</span><span class="sxs-lookup"><span data-stu-id="8f4ba-118">Name</span></span>       | <span data-ttu-id="8f4ba-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f4ba-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8f4ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f4ba-120">Authorization</span></span>  | <span data-ttu-id="8f4ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f4ba-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8f4ba-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8f4ba-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f4ba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f4ba-126">Request body</span></span>
<span data-ttu-id="8f4ba-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8f4ba-130">属性</span><span class="sxs-lookup"><span data-stu-id="8f4ba-130">Property</span></span>     | <span data-ttu-id="8f4ba-131">类型</span><span class="sxs-lookup"><span data-stu-id="8f4ba-131">Type</span></span>   |<span data-ttu-id="8f4ba-132">说明</span><span class="sxs-lookup"><span data-stu-id="8f4ba-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f4ba-133">高度</span><span class="sxs-lookup"><span data-stu-id="8f4ba-133">height</span></span>|<span data-ttu-id="8f4ba-134">double</span><span class="sxs-lookup"><span data-stu-id="8f4ba-134">double</span></span>|<span data-ttu-id="8f4ba-135">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="8f4ba-136">left</span><span class="sxs-lookup"><span data-stu-id="8f4ba-136">left</span></span>|<span data-ttu-id="8f4ba-137">double</span><span class="sxs-lookup"><span data-stu-id="8f4ba-137">double</span></span>|<span data-ttu-id="8f4ba-138">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="8f4ba-139">name</span><span class="sxs-lookup"><span data-stu-id="8f4ba-139">name</span></span>|<span data-ttu-id="8f4ba-140">string</span><span class="sxs-lookup"><span data-stu-id="8f4ba-140">string</span></span>|<span data-ttu-id="8f4ba-141">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="8f4ba-142">top</span><span class="sxs-lookup"><span data-stu-id="8f4ba-142">top</span></span>|<span data-ttu-id="8f4ba-143">double</span><span class="sxs-lookup"><span data-stu-id="8f4ba-143">double</span></span>|<span data-ttu-id="8f4ba-144">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="8f4ba-145">width</span><span class="sxs-lookup"><span data-stu-id="8f4ba-145">width</span></span>|<span data-ttu-id="8f4ba-146">double</span><span class="sxs-lookup"><span data-stu-id="8f4ba-146">double</span></span>|<span data-ttu-id="8f4ba-147">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="8f4ba-148">响应</span><span class="sxs-lookup"><span data-stu-id="8f4ba-148">Response</span></span>

<span data-ttu-id="8f4ba-149">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookChart](../resources/workbookchart.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-149">If successful, this method returns a `200 OK` response code and updated [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8f4ba-150">示例</span><span class="sxs-lookup"><span data-stu-id="8f4ba-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f4ba-151">请求</span><span class="sxs-lookup"><span data-stu-id="8f4ba-151">Request</span></span>
<span data-ttu-id="8f4ba-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-152">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8f4ba-153">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8f4ba-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f4ba-154">C#</span><span class="sxs-lookup"><span data-stu-id="8f4ba-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f4ba-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f4ba-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f4ba-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="8f4ba-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8f4ba-157">响应</span><span class="sxs-lookup"><span data-stu-id="8f4ba-157">Response</span></span>
<span data-ttu-id="8f4ba-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f4ba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
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
<!--
{
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
