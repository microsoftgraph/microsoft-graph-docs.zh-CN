---
title: 更新 chartlegend
description: 更新 chartlegend 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: de47c95627a10b608e69f2be6b7b6c9e8d5b1b21
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418391"
---
# <a name="update-chartlegend"></a><span data-ttu-id="bc1ce-103">更新 chartlegend</span><span class="sxs-lookup"><span data-stu-id="bc1ce-103">Update chartlegend</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc1ce-104">更新 chartlegend 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc1ce-105">权限</span><span class="sxs-lookup"><span data-stu-id="bc1ce-105">Permissions</span></span>
<span data-ttu-id="bc1ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc1ce-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc1ce-108">Permission type</span></span>      | <span data-ttu-id="bc1ce-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc1ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc1ce-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc1ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc1ce-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc1ce-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc1ce-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc1ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc1ce-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc1ce-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc1ce-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc1ce-114">Application</span></span> | <span data-ttu-id="bc1ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc1ce-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc1ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="bc1ce-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="bc1ce-117">Optional request headers</span></span>
| <span data-ttu-id="bc1ce-118">名称</span><span class="sxs-lookup"><span data-stu-id="bc1ce-118">Name</span></span>       | <span data-ttu-id="bc1ce-119">说明</span><span class="sxs-lookup"><span data-stu-id="bc1ce-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bc1ce-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc1ce-120">Authorization</span></span>  | <span data-ttu-id="bc1ce-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc1ce-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc1ce-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc1ce-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc1ce-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc1ce-126">Request body</span></span>
<span data-ttu-id="bc1ce-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc1ce-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc1ce-130">Property</span></span>     | <span data-ttu-id="bc1ce-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc1ce-131">Type</span></span>   |<span data-ttu-id="bc1ce-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc1ce-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc1ce-133">overlay</span><span class="sxs-lookup"><span data-stu-id="bc1ce-133">overlay</span></span>|<span data-ttu-id="bc1ce-134">布尔</span><span class="sxs-lookup"><span data-stu-id="bc1ce-134">boolean</span></span>|<span data-ttu-id="bc1ce-135">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="bc1ce-136">position</span><span class="sxs-lookup"><span data-stu-id="bc1ce-136">position</span></span>|<span data-ttu-id="bc1ce-137">string</span><span class="sxs-lookup"><span data-stu-id="bc1ce-137">string</span></span>|<span data-ttu-id="bc1ce-p105">表示图例在图表上的位置。可能的值是：`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="bc1ce-140">visible</span><span class="sxs-lookup"><span data-stu-id="bc1ce-140">visible</span></span>|<span data-ttu-id="bc1ce-141">布尔</span><span class="sxs-lookup"><span data-stu-id="bc1ce-141">boolean</span></span>|<span data-ttu-id="bc1ce-142">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="bc1ce-143">响应</span><span class="sxs-lookup"><span data-stu-id="bc1ce-143">Response</span></span>

<span data-ttu-id="bc1ce-144">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[workbookChartLegend](../resources/workbookchartlegend.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-144">If successful, this method returns a `200 OK` response code and updated [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc1ce-145">示例</span><span class="sxs-lookup"><span data-stu-id="bc1ce-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc1ce-146">请求</span><span class="sxs-lookup"><span data-stu-id="bc1ce-146">Request</span></span>
<span data-ttu-id="bc1ce-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bc1ce-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bc1ce-148">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc1ce-149">C#</span><span class="sxs-lookup"><span data-stu-id="bc1ce-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chartlegend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc1ce-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc1ce-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chartlegend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc1ce-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="bc1ce-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chartlegend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc1ce-152">响应</span><span class="sxs-lookup"><span data-stu-id="bc1ce-152">Response</span></span>
<span data-ttu-id="bc1ce-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc1ce-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
