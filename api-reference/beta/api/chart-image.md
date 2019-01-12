---
title: 图表：图像
description: 通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5ee56b38ca75162a760be54e58dacb6ced6bbc16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976406"
---
# <a name="chart-image"></a><span data-ttu-id="20aa2-103">图表：图像</span><span class="sxs-lookup"><span data-stu-id="20aa2-103">Chart: Image</span></span>

> <span data-ttu-id="20aa2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="20aa2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20aa2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="20aa2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20aa2-106">通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="20aa2-106">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="20aa2-107">权限</span><span class="sxs-lookup"><span data-stu-id="20aa2-107">Permissions</span></span>
<span data-ttu-id="20aa2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20aa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20aa2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="20aa2-110">Permission type</span></span>      | <span data-ttu-id="20aa2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20aa2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20aa2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20aa2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20aa2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20aa2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20aa2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20aa2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20aa2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20aa2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="20aa2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="20aa2-116">Application</span></span> | <span data-ttu-id="20aa2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="20aa2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20aa2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20aa2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="20aa2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="20aa2-119">Request headers</span></span>
| <span data-ttu-id="20aa2-120">名称</span><span class="sxs-lookup"><span data-stu-id="20aa2-120">Name</span></span>       | <span data-ttu-id="20aa2-121">说明</span><span class="sxs-lookup"><span data-stu-id="20aa2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20aa2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20aa2-122">Authorization</span></span>  | <span data-ttu-id="20aa2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20aa2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20aa2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20aa2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="20aa2-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="20aa2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20aa2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="20aa2-128">Request body</span></span>
<span data-ttu-id="20aa2-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="20aa2-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20aa2-130">参数</span><span class="sxs-lookup"><span data-stu-id="20aa2-130">Parameter</span></span>    | <span data-ttu-id="20aa2-131">类型</span><span class="sxs-lookup"><span data-stu-id="20aa2-131">Type</span></span>   |<span data-ttu-id="20aa2-132">说明</span><span class="sxs-lookup"><span data-stu-id="20aa2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20aa2-133">height</span><span class="sxs-lookup"><span data-stu-id="20aa2-133">height</span></span>|<span data-ttu-id="20aa2-134">number</span><span class="sxs-lookup"><span data-stu-id="20aa2-134">number</span></span>|<span data-ttu-id="20aa2-p105">可选。生成的图像的所需高度。</span><span class="sxs-lookup"><span data-stu-id="20aa2-p105">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="20aa2-137">width</span><span class="sxs-lookup"><span data-stu-id="20aa2-137">width</span></span>|<span data-ttu-id="20aa2-138">number</span><span class="sxs-lookup"><span data-stu-id="20aa2-138">number</span></span>|<span data-ttu-id="20aa2-p106">可选。生成的图像的所需宽度。</span><span class="sxs-lookup"><span data-stu-id="20aa2-p106">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="20aa2-141">fittingMode</span><span class="sxs-lookup"><span data-stu-id="20aa2-141">fittingMode</span></span>|<span data-ttu-id="20aa2-142">string</span><span class="sxs-lookup"><span data-stu-id="20aa2-142">string</span></span>|<span data-ttu-id="20aa2-p107">可选。该方法用于将图表缩放到指定的尺寸（如果设置了高度和宽度）。”可能的值是：`Fit`、`FitAndCenter`、`Fill`。</span><span class="sxs-lookup"><span data-stu-id="20aa2-p107">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="20aa2-146">响应</span><span class="sxs-lookup"><span data-stu-id="20aa2-146">Response</span></span>

<span data-ttu-id="20aa2-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 base-64 图像字符串。</span><span class="sxs-lookup"><span data-stu-id="20aa2-147">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20aa2-148">示例</span><span class="sxs-lookup"><span data-stu-id="20aa2-148">Example</span></span>
<span data-ttu-id="20aa2-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="20aa2-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="20aa2-150">请求</span><span class="sxs-lookup"><span data-stu-id="20aa2-150">Request</span></span>
<span data-ttu-id="20aa2-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20aa2-151">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="20aa2-152">响应</span><span class="sxs-lookup"><span data-stu-id="20aa2-152">Response</span></span>
<span data-ttu-id="20aa2-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="20aa2-153">Here is an example of the response.</span></span> <span data-ttu-id="20aa2-154">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="20aa2-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="20aa2-155">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20aa2-155">All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="20aa2-156">用法</span><span class="sxs-lookup"><span data-stu-id="20aa2-156">Usage</span></span>

<span data-ttu-id="20aa2-157">可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。</span><span class="sxs-lookup"><span data-stu-id="20aa2-157">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="20aa2-158">对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。</span><span class="sxs-lookup"><span data-stu-id="20aa2-158">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="20aa2-159">下面的示例展示了使用默认参数返回的图表图像。</span><span class="sxs-lookup"><span data-stu-id="20aa2-159">Here is an example of a chart image returned with the default parameters.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="20aa2-161">若要自定义图像的显示方式，请指定高度、宽度和调整模式。</span><span class="sxs-lookup"><span data-stu-id="20aa2-161">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="20aa2-162">下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。</span><span class="sxs-lookup"><span data-stu-id="20aa2-162">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
