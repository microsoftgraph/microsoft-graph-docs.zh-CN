---
title: 更新图表
description: 更新 chart 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c8e7f25b04869ec80ecad8fc27eff24a6117b621
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958946"
---
# <a name="update-chart"></a><span data-ttu-id="03043-103">更新图表</span><span class="sxs-lookup"><span data-stu-id="03043-103">Update chart</span></span>

<span data-ttu-id="03043-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03043-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03043-105">更新 chart 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03043-105">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="03043-106">权限</span><span class="sxs-lookup"><span data-stu-id="03043-106">Permissions</span></span>
<span data-ttu-id="03043-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03043-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="03043-109">Permission type</span></span>      | <span data-ttu-id="03043-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03043-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03043-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03043-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03043-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03043-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03043-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03043-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03043-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03043-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03043-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="03043-115">Application</span></span> | <span data-ttu-id="03043-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03043-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03043-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03043-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="03043-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="03043-118">Optional request headers</span></span>
| <span data-ttu-id="03043-119">名称</span><span class="sxs-lookup"><span data-stu-id="03043-119">Name</span></span>       | <span data-ttu-id="03043-120">说明</span><span class="sxs-lookup"><span data-stu-id="03043-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="03043-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03043-121">Authorization</span></span>  | <span data-ttu-id="03043-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03043-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03043-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03043-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="03043-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="03043-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03043-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03043-127">Request body</span></span>
<span data-ttu-id="03043-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="03043-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="03043-131">属性</span><span class="sxs-lookup"><span data-stu-id="03043-131">Property</span></span>     | <span data-ttu-id="03043-132">类型</span><span class="sxs-lookup"><span data-stu-id="03043-132">Type</span></span>   |<span data-ttu-id="03043-133">说明</span><span class="sxs-lookup"><span data-stu-id="03043-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03043-134">高度</span><span class="sxs-lookup"><span data-stu-id="03043-134">height</span></span>|<span data-ttu-id="03043-135">double</span><span class="sxs-lookup"><span data-stu-id="03043-135">double</span></span>|<span data-ttu-id="03043-136">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="03043-136">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="03043-137">left</span><span class="sxs-lookup"><span data-stu-id="03043-137">left</span></span>|<span data-ttu-id="03043-138">double</span><span class="sxs-lookup"><span data-stu-id="03043-138">double</span></span>|<span data-ttu-id="03043-139">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="03043-139">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="03043-140">name</span><span class="sxs-lookup"><span data-stu-id="03043-140">name</span></span>|<span data-ttu-id="03043-141">string</span><span class="sxs-lookup"><span data-stu-id="03043-141">string</span></span>|<span data-ttu-id="03043-142">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="03043-142">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="03043-143">top</span><span class="sxs-lookup"><span data-stu-id="03043-143">top</span></span>|<span data-ttu-id="03043-144">double</span><span class="sxs-lookup"><span data-stu-id="03043-144">double</span></span>|<span data-ttu-id="03043-145">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="03043-145">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="03043-146">width</span><span class="sxs-lookup"><span data-stu-id="03043-146">width</span></span>|<span data-ttu-id="03043-147">double</span><span class="sxs-lookup"><span data-stu-id="03043-147">double</span></span>|<span data-ttu-id="03043-148">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="03043-148">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="03043-149">响应</span><span class="sxs-lookup"><span data-stu-id="03043-149">Response</span></span>

<span data-ttu-id="03043-150">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [workbookChart](../resources/workbookchart.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03043-150">If successful, this method returns a `200 OK` response code and updated [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03043-151">示例</span><span class="sxs-lookup"><span data-stu-id="03043-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03043-152">请求</span><span class="sxs-lookup"><span data-stu-id="03043-152">Request</span></span>
<span data-ttu-id="03043-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03043-153">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03043-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="03043-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03043-155">C#</span><span class="sxs-lookup"><span data-stu-id="03043-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03043-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03043-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03043-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03043-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03043-158">Java</span><span class="sxs-lookup"><span data-stu-id="03043-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="03043-159">响应</span><span class="sxs-lookup"><span data-stu-id="03043-159">Response</span></span>
<span data-ttu-id="03043-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03043-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


