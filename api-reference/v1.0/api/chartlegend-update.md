---
title: 更新 chartlegend
description: 更新 chartlegend 对象的属性。
ms.openlocfilehash: c9c3d39bda04e178a892c94f2ea533460a7bfad8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011737"
---
# <a name="update-chartlegend"></a><span data-ttu-id="d4574-103">更新 chartlegend</span><span class="sxs-lookup"><span data-stu-id="d4574-103">Update chartlegend</span></span>

<span data-ttu-id="d4574-104">更新 chartlegend 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d4574-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d4574-105">权限</span><span class="sxs-lookup"><span data-stu-id="d4574-105">Permissions</span></span>
<span data-ttu-id="d4574-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4574-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4574-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4574-108">Permission type</span></span>      | <span data-ttu-id="d4574-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4574-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4574-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4574-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4574-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d4574-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d4574-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4574-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4574-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4574-113">Not supported.</span></span>    |
|<span data-ttu-id="d4574-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4574-114">Application</span></span> | <span data-ttu-id="d4574-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4574-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4574-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4574-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="d4574-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d4574-117">Optional request headers</span></span>
| <span data-ttu-id="d4574-118">名称</span><span class="sxs-lookup"><span data-stu-id="d4574-118">Name</span></span>       | <span data-ttu-id="d4574-119">说明</span><span class="sxs-lookup"><span data-stu-id="d4574-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d4574-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4574-120">Authorization</span></span>  | <span data-ttu-id="d4574-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4574-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4574-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d4574-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d4574-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d4574-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4574-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4574-126">Request body</span></span>
<span data-ttu-id="d4574-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d4574-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d4574-130">属性</span><span class="sxs-lookup"><span data-stu-id="d4574-130">Property</span></span>     | <span data-ttu-id="d4574-131">类型</span><span class="sxs-lookup"><span data-stu-id="d4574-131">Type</span></span>   |<span data-ttu-id="d4574-132">说明</span><span class="sxs-lookup"><span data-stu-id="d4574-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4574-133">overlay</span><span class="sxs-lookup"><span data-stu-id="d4574-133">overlay</span></span>|<span data-ttu-id="d4574-134">boolean</span><span class="sxs-lookup"><span data-stu-id="d4574-134">boolean</span></span>|<span data-ttu-id="d4574-135">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d4574-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="d4574-136">position</span><span class="sxs-lookup"><span data-stu-id="d4574-136">position</span></span>|<span data-ttu-id="d4574-137">string</span><span class="sxs-lookup"><span data-stu-id="d4574-137">string</span></span>|<span data-ttu-id="d4574-138">代表图表上图例的位置。</span><span class="sxs-lookup"><span data-stu-id="d4574-138">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="d4574-139">可能的值为： `Top`， `Bottom`， `Left`， `Right`， `Corner`， `Custom`。</span><span class="sxs-lookup"><span data-stu-id="d4574-139">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="d4574-140">visible</span><span class="sxs-lookup"><span data-stu-id="d4574-140">visible</span></span>|<span data-ttu-id="d4574-141">boolean</span><span class="sxs-lookup"><span data-stu-id="d4574-141">boolean</span></span>|<span data-ttu-id="d4574-142">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d4574-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="d4574-143">响应</span><span class="sxs-lookup"><span data-stu-id="d4574-143">Response</span></span>

<span data-ttu-id="d4574-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[WorkbookChartLegend](../resources/chartlegend.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d4574-144">If successful, this method returns a `200 OK` response code and updated [WorkbookChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4574-145">示例</span><span class="sxs-lookup"><span data-stu-id="d4574-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4574-146">请求</span><span class="sxs-lookup"><span data-stu-id="d4574-146">Request</span></span>
<span data-ttu-id="d4574-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4574-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="d4574-148">响应</span><span class="sxs-lookup"><span data-stu-id="d4574-148">Response</span></span>
<span data-ttu-id="d4574-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4574-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->