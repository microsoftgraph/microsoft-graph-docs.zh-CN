---
title: 更新图表
description: 更新 chart 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: feb89c9b1cf94c0c1cfeebe3aebec187a5d59406
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047495"
---
# <a name="update-chart"></a><span data-ttu-id="3b5ff-103">更新图表</span><span class="sxs-lookup"><span data-stu-id="3b5ff-103">Update chart</span></span>

<span data-ttu-id="3b5ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b5ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b5ff-105">更新 chart 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-105">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b5ff-106">权限</span><span class="sxs-lookup"><span data-stu-id="3b5ff-106">Permissions</span></span>
<span data-ttu-id="3b5ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b5ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b5ff-109">Permission type</span></span>      | <span data-ttu-id="3b5ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b5ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b5ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b5ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3b5ff-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b5ff-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b5ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b5ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b5ff-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b5ff-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b5ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b5ff-115">Application</span></span> | <span data-ttu-id="3b5ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b5ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b5ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3b5ff-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="3b5ff-118">Optional request headers</span></span>
| <span data-ttu-id="3b5ff-119">名称</span><span class="sxs-lookup"><span data-stu-id="3b5ff-119">Name</span></span>       | <span data-ttu-id="3b5ff-120">说明</span><span class="sxs-lookup"><span data-stu-id="3b5ff-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3b5ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b5ff-121">Authorization</span></span>  | <span data-ttu-id="3b5ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b5ff-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3b5ff-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="3b5ff-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b5ff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b5ff-127">Request body</span></span>
<span data-ttu-id="3b5ff-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3b5ff-131">属性</span><span class="sxs-lookup"><span data-stu-id="3b5ff-131">Property</span></span>     | <span data-ttu-id="3b5ff-132">类型</span><span class="sxs-lookup"><span data-stu-id="3b5ff-132">Type</span></span>   |<span data-ttu-id="3b5ff-133">说明</span><span class="sxs-lookup"><span data-stu-id="3b5ff-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b5ff-134">高度</span><span class="sxs-lookup"><span data-stu-id="3b5ff-134">height</span></span>|<span data-ttu-id="3b5ff-135">double</span><span class="sxs-lookup"><span data-stu-id="3b5ff-135">double</span></span>|<span data-ttu-id="3b5ff-136">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-136">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="3b5ff-137">left</span><span class="sxs-lookup"><span data-stu-id="3b5ff-137">left</span></span>|<span data-ttu-id="3b5ff-138">double</span><span class="sxs-lookup"><span data-stu-id="3b5ff-138">double</span></span>|<span data-ttu-id="3b5ff-139">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-139">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="3b5ff-140">name</span><span class="sxs-lookup"><span data-stu-id="3b5ff-140">name</span></span>|<span data-ttu-id="3b5ff-141">string</span><span class="sxs-lookup"><span data-stu-id="3b5ff-141">string</span></span>|<span data-ttu-id="3b5ff-142">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-142">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="3b5ff-143">top</span><span class="sxs-lookup"><span data-stu-id="3b5ff-143">top</span></span>|<span data-ttu-id="3b5ff-144">double</span><span class="sxs-lookup"><span data-stu-id="3b5ff-144">double</span></span>|<span data-ttu-id="3b5ff-145">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-145">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="3b5ff-146">width</span><span class="sxs-lookup"><span data-stu-id="3b5ff-146">width</span></span>|<span data-ttu-id="3b5ff-147">double</span><span class="sxs-lookup"><span data-stu-id="3b5ff-147">double</span></span>|<span data-ttu-id="3b5ff-148">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-148">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="3b5ff-149">响应</span><span class="sxs-lookup"><span data-stu-id="3b5ff-149">Response</span></span>

<span data-ttu-id="3b5ff-150">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [workbookChart](../resources/workbookchart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-150">If successful, this method returns a `200 OK` response code and updated [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b5ff-151">示例</span><span class="sxs-lookup"><span data-stu-id="3b5ff-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b5ff-152">请求</span><span class="sxs-lookup"><span data-stu-id="3b5ff-152">Request</span></span>
<span data-ttu-id="3b5ff-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b5ff-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b5ff-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3b5ff-155">C#</span><span class="sxs-lookup"><span data-stu-id="3b5ff-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b5ff-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b5ff-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b5ff-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b5ff-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b5ff-158">Java</span><span class="sxs-lookup"><span data-stu-id="3b5ff-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3b5ff-159">响应</span><span class="sxs-lookup"><span data-stu-id="3b5ff-159">Response</span></span>
<span data-ttu-id="3b5ff-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-160">Here is an example of the response.</span></span> <span data-ttu-id="3b5ff-161">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3b5ff-161">Note: The response object shown here might be shortened for readability.</span></span>
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


