---
title: 更新 chartlegend
description: 更新 chartlegend 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 14671f02929d4750f714cd870f4b76af969ca391
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574508"
---
# <a name="update-chartlegend"></a><span data-ttu-id="ebcab-103">更新 chartlegend</span><span class="sxs-lookup"><span data-stu-id="ebcab-103">Update chartlegend</span></span>

<span data-ttu-id="ebcab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebcab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebcab-105">更新 chartlegend 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ebcab-105">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebcab-106">权限</span><span class="sxs-lookup"><span data-stu-id="ebcab-106">Permissions</span></span>
<span data-ttu-id="ebcab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebcab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebcab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebcab-109">Permission type</span></span>      | <span data-ttu-id="ebcab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebcab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebcab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebcab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebcab-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebcab-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebcab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebcab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebcab-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebcab-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ebcab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebcab-115">Application</span></span> | <span data-ttu-id="ebcab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebcab-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebcab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebcab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="ebcab-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="ebcab-118">Optional request headers</span></span>
| <span data-ttu-id="ebcab-119">名称</span><span class="sxs-lookup"><span data-stu-id="ebcab-119">Name</span></span>       | <span data-ttu-id="ebcab-120">说明</span><span class="sxs-lookup"><span data-stu-id="ebcab-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ebcab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebcab-121">Authorization</span></span>  | <span data-ttu-id="ebcab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebcab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ebcab-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ebcab-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="ebcab-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ebcab-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebcab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebcab-127">Request body</span></span>
<span data-ttu-id="ebcab-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ebcab-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ebcab-131">属性</span><span class="sxs-lookup"><span data-stu-id="ebcab-131">Property</span></span>     | <span data-ttu-id="ebcab-132">类型</span><span class="sxs-lookup"><span data-stu-id="ebcab-132">Type</span></span>   |<span data-ttu-id="ebcab-133">说明</span><span class="sxs-lookup"><span data-stu-id="ebcab-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebcab-134">overlay</span><span class="sxs-lookup"><span data-stu-id="ebcab-134">overlay</span></span>|<span data-ttu-id="ebcab-135">布尔</span><span class="sxs-lookup"><span data-stu-id="ebcab-135">boolean</span></span>|<span data-ttu-id="ebcab-136">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ebcab-136">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="ebcab-137">position</span><span class="sxs-lookup"><span data-stu-id="ebcab-137">position</span></span>|<span data-ttu-id="ebcab-138">string</span><span class="sxs-lookup"><span data-stu-id="ebcab-138">string</span></span>|<span data-ttu-id="ebcab-p105">表示图例在图表上的位置。可能的值是：`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="ebcab-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="ebcab-141">visible</span><span class="sxs-lookup"><span data-stu-id="ebcab-141">visible</span></span>|<span data-ttu-id="ebcab-142">布尔</span><span class="sxs-lookup"><span data-stu-id="ebcab-142">boolean</span></span>|<span data-ttu-id="ebcab-143">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ebcab-143">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="ebcab-144">响应</span><span class="sxs-lookup"><span data-stu-id="ebcab-144">Response</span></span>

<span data-ttu-id="ebcab-145">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [workbookChartLegend](../resources/workbookchartlegend.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebcab-145">If successful, this method returns a `200 OK` response code and updated [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebcab-146">示例</span><span class="sxs-lookup"><span data-stu-id="ebcab-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebcab-147">请求</span><span class="sxs-lookup"><span data-stu-id="ebcab-147">Request</span></span>
<span data-ttu-id="ebcab-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebcab-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebcab-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebcab-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
# <a name="c"></a>[<span data-ttu-id="ebcab-150">C#</span><span class="sxs-lookup"><span data-stu-id="ebcab-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebcab-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebcab-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebcab-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebcab-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebcab-153">Java</span><span class="sxs-lookup"><span data-stu-id="ebcab-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chartlegend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ebcab-154">响应</span><span class="sxs-lookup"><span data-stu-id="ebcab-154">Response</span></span>
<span data-ttu-id="ebcab-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ebcab-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


