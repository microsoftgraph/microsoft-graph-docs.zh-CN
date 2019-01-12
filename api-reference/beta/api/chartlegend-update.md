---
title: 更新 chartlegend
description: 更新 chartlegend 对象的属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 03bcd9ce5d5c15f624dd0eaa231f8965137c210e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946628"
---
# <a name="update-chartlegend"></a><span data-ttu-id="0ce1c-103">更新 chartlegend</span><span class="sxs-lookup"><span data-stu-id="0ce1c-103">Update chartlegend</span></span>

> <span data-ttu-id="0ce1c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ce1c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ce1c-106">更新 chartlegend 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-106">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ce1c-107">权限</span><span class="sxs-lookup"><span data-stu-id="0ce1c-107">Permissions</span></span>
<span data-ttu-id="0ce1c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ce1c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ce1c-110">Permission type</span></span>      | <span data-ttu-id="0ce1c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ce1c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ce1c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce1c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ce1c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ce1c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ce1c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce1c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ce1c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0ce1c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ce1c-116">Application</span></span> | <span data-ttu-id="0ce1c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ce1c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ce1c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="0ce1c-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0ce1c-119">Optional request headers</span></span>
| <span data-ttu-id="0ce1c-120">名称</span><span class="sxs-lookup"><span data-stu-id="0ce1c-120">Name</span></span>       | <span data-ttu-id="0ce1c-121">说明</span><span class="sxs-lookup"><span data-stu-id="0ce1c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0ce1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ce1c-122">Authorization</span></span>  | <span data-ttu-id="0ce1c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ce1c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ce1c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ce1c-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ce1c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ce1c-128">Request body</span></span>
<span data-ttu-id="0ce1c-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0ce1c-132">属性</span><span class="sxs-lookup"><span data-stu-id="0ce1c-132">Property</span></span>     | <span data-ttu-id="0ce1c-133">类型</span><span class="sxs-lookup"><span data-stu-id="0ce1c-133">Type</span></span>   |<span data-ttu-id="0ce1c-134">说明</span><span class="sxs-lookup"><span data-stu-id="0ce1c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ce1c-135">overlay</span><span class="sxs-lookup"><span data-stu-id="0ce1c-135">overlay</span></span>|<span data-ttu-id="0ce1c-136">boolean</span><span class="sxs-lookup"><span data-stu-id="0ce1c-136">boolean</span></span>|<span data-ttu-id="0ce1c-137">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-137">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="0ce1c-138">position</span><span class="sxs-lookup"><span data-stu-id="0ce1c-138">position</span></span>|<span data-ttu-id="0ce1c-139">string</span><span class="sxs-lookup"><span data-stu-id="0ce1c-139">string</span></span>|<span data-ttu-id="0ce1c-p106">表示图例在图表上的位置。可能的值是：`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-p106">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="0ce1c-142">visible</span><span class="sxs-lookup"><span data-stu-id="0ce1c-142">visible</span></span>|<span data-ttu-id="0ce1c-143">boolean</span><span class="sxs-lookup"><span data-stu-id="0ce1c-143">boolean</span></span>|<span data-ttu-id="0ce1c-144">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-144">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="0ce1c-145">响应</span><span class="sxs-lookup"><span data-stu-id="0ce1c-145">Response</span></span>

<span data-ttu-id="0ce1c-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [ChartLegend](../resources/chartlegend.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-146">If successful, this method returns a `200 OK` response code and updated [ChartLegend](../resources/chartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ce1c-147">示例</span><span class="sxs-lookup"><span data-stu-id="0ce1c-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ce1c-148">请求</span><span class="sxs-lookup"><span data-stu-id="0ce1c-148">Request</span></span>
<span data-ttu-id="0ce1c-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="0ce1c-150">响应</span><span class="sxs-lookup"><span data-stu-id="0ce1c-150">Response</span></span>
<span data-ttu-id="0ce1c-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ce1c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartLegend"
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
