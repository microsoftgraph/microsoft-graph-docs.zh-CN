---
title: 图表：图像
description: 通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0f61866885f0798b9e96f80e22a636fb5f619e34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939719"
---
# <a name="chart-image"></a><span data-ttu-id="6916e-103">图表：图像</span><span class="sxs-lookup"><span data-stu-id="6916e-103">Chart: Image</span></span>

<span data-ttu-id="6916e-104">通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="6916e-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="6916e-105">权限</span><span class="sxs-lookup"><span data-stu-id="6916e-105">Permissions</span></span>
<span data-ttu-id="6916e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6916e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6916e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6916e-108">Permission type</span></span>      | <span data-ttu-id="6916e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6916e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6916e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6916e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6916e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6916e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6916e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6916e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6916e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6916e-113">Not supported.</span></span>    |
|<span data-ttu-id="6916e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6916e-114">Application</span></span> | <span data-ttu-id="6916e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6916e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6916e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6916e-116">HTTP request</span></span>
<!-- { "blockType": "samples" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/image
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480)
GET /workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```
## <a name="request-headers"></a><span data-ttu-id="6916e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6916e-117">Request headers</span></span>
| <span data-ttu-id="6916e-118">名称</span><span class="sxs-lookup"><span data-stu-id="6916e-118">Name</span></span>       | <span data-ttu-id="6916e-119">说明</span><span class="sxs-lookup"><span data-stu-id="6916e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6916e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6916e-120">Authorization</span></span>  | <span data-ttu-id="6916e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6916e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6916e-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6916e-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6916e-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="6916e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="6916e-126">路径参数</span><span class="sxs-lookup"><span data-stu-id="6916e-126">Path parameters</span></span>
<span data-ttu-id="6916e-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6916e-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6916e-128">参数</span><span class="sxs-lookup"><span data-stu-id="6916e-128">Parameter</span></span>    | <span data-ttu-id="6916e-129">类型</span><span class="sxs-lookup"><span data-stu-id="6916e-129">Type</span></span>   |<span data-ttu-id="6916e-130">说明</span><span class="sxs-lookup"><span data-stu-id="6916e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6916e-131">height</span><span class="sxs-lookup"><span data-stu-id="6916e-131">height</span></span>|<span data-ttu-id="6916e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="6916e-132">Int32</span></span>|<span data-ttu-id="6916e-133">所需结果图像的高度。</span><span class="sxs-lookup"><span data-stu-id="6916e-133">The desired height of the resulting image.</span></span> <span data-ttu-id="6916e-134">可选。</span><span class="sxs-lookup"><span data-stu-id="6916e-134">Optional.</span></span>|
|<span data-ttu-id="6916e-135">width</span><span class="sxs-lookup"><span data-stu-id="6916e-135">width</span></span>|<span data-ttu-id="6916e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6916e-136">Int32</span></span>|<span data-ttu-id="6916e-137">所需结果图像的宽度。</span><span class="sxs-lookup"><span data-stu-id="6916e-137">The desired width of the resulting image.</span></span> <span data-ttu-id="6916e-138">可选。</span><span class="sxs-lookup"><span data-stu-id="6916e-138">Optional.</span></span>|
|<span data-ttu-id="6916e-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="6916e-139">fittingMode</span></span>|<span data-ttu-id="6916e-140">string</span><span class="sxs-lookup"><span data-stu-id="6916e-140">string</span></span>|<span data-ttu-id="6916e-141">使用的方法来扩展到指定的尺寸图表 （如果设置高度和宽度）。"</span><span class="sxs-lookup"><span data-stu-id="6916e-141">The method used to scale the chart to the specified dimensions (if both height and width are set)."</span></span>  <span data-ttu-id="6916e-142">可能的值为： `Fit`， `FitAndCenter`， `Fill`。</span><span class="sxs-lookup"><span data-stu-id="6916e-142">The possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="6916e-143">响应</span><span class="sxs-lookup"><span data-stu-id="6916e-143">Response</span></span>

<span data-ttu-id="6916e-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 base-64 图像字符串。</span><span class="sxs-lookup"><span data-stu-id="6916e-144">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6916e-145">示例</span><span class="sxs-lookup"><span data-stu-id="6916e-145">Example</span></span>
<span data-ttu-id="6916e-146">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6916e-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6916e-147">请求</span><span class="sxs-lookup"><span data-stu-id="6916e-147">Request</span></span>
<span data-ttu-id="6916e-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6916e-148">Here is an example of the request.</span></span>

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/image(width=640,height=480,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="6916e-149">响应</span><span class="sxs-lookup"><span data-stu-id="6916e-149">Response</span></span>
<span data-ttu-id="6916e-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6916e-150">Here is an example of the response.</span></span> <span data-ttu-id="6916e-151">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6916e-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6916e-152">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6916e-152">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "response", "@odata.type": "Edm.String" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json;odata.metadata=minimal;odata.streaming=true

{
"value" : "base-64 chart image string"
}
```

## <a name="usage"></a><span data-ttu-id="6916e-153">用法</span><span class="sxs-lookup"><span data-stu-id="6916e-153">Usage</span></span>

<span data-ttu-id="6916e-154">可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。</span><span class="sxs-lookup"><span data-stu-id="6916e-154">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="6916e-155">对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。</span><span class="sxs-lookup"><span data-stu-id="6916e-155">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="6916e-156">下面的示例展示了使用默认参数返回的图表图像。</span><span class="sxs-lookup"><span data-stu-id="6916e-156">Here is an example of a chart image returned with the default parameters.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="6916e-158">若要自定义图像的显示方式，请指定高度、宽度和调整模式。</span><span class="sxs-lookup"><span data-stu-id="6916e-158">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="6916e-159">下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。</span><span class="sxs-lookup"><span data-stu-id="6916e-159">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
