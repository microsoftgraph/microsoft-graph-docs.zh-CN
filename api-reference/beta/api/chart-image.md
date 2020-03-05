---
title: 图表：图像
description: 通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 30f614142486cb1403d6f4ca13cecbde68fd5c7d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440008"
---
# <a name="chart-image"></a><span data-ttu-id="9b56d-103">图表：图像</span><span class="sxs-lookup"><span data-stu-id="9b56d-103">Chart: Image</span></span>

<span data-ttu-id="9b56d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9b56d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b56d-105">通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="9b56d-105">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="9b56d-106">权限</span><span class="sxs-lookup"><span data-stu-id="9b56d-106">Permissions</span></span>
<span data-ttu-id="9b56d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b56d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b56d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b56d-109">Permission type</span></span>      | <span data-ttu-id="9b56d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b56d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b56d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9b56d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9b56d-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b56d-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b56d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9b56d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b56d-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b56d-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9b56d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b56d-115">Application</span></span> | <span data-ttu-id="9b56d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9b56d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b56d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b56d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="9b56d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b56d-118">Request headers</span></span>
| <span data-ttu-id="9b56d-119">名称</span><span class="sxs-lookup"><span data-stu-id="9b56d-119">Name</span></span>       | <span data-ttu-id="9b56d-120">说明</span><span class="sxs-lookup"><span data-stu-id="9b56d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9b56d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b56d-121">Authorization</span></span>  | <span data-ttu-id="9b56d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b56d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b56d-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9b56d-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9b56d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9b56d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b56d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b56d-127">Request body</span></span>
<span data-ttu-id="9b56d-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9b56d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b56d-129">参数</span><span class="sxs-lookup"><span data-stu-id="9b56d-129">Parameter</span></span>    | <span data-ttu-id="9b56d-130">类型</span><span class="sxs-lookup"><span data-stu-id="9b56d-130">Type</span></span>   |<span data-ttu-id="9b56d-131">说明</span><span class="sxs-lookup"><span data-stu-id="9b56d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b56d-132">height</span><span class="sxs-lookup"><span data-stu-id="9b56d-132">height</span></span>|<span data-ttu-id="9b56d-133">number</span><span class="sxs-lookup"><span data-stu-id="9b56d-133">number</span></span>|<span data-ttu-id="9b56d-p104">可选。生成的图像的所需高度。</span><span class="sxs-lookup"><span data-stu-id="9b56d-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="9b56d-136">width</span><span class="sxs-lookup"><span data-stu-id="9b56d-136">width</span></span>|<span data-ttu-id="9b56d-137">number</span><span class="sxs-lookup"><span data-stu-id="9b56d-137">number</span></span>|<span data-ttu-id="9b56d-p105">可选。生成的图像的所需宽度。</span><span class="sxs-lookup"><span data-stu-id="9b56d-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="9b56d-140">fittingMode</span><span class="sxs-lookup"><span data-stu-id="9b56d-140">fittingMode</span></span>|<span data-ttu-id="9b56d-141">string</span><span class="sxs-lookup"><span data-stu-id="9b56d-141">string</span></span>|<span data-ttu-id="9b56d-p106">可选。该方法用于将图表缩放到指定的尺寸（如果设置了高度和宽度）。”可能的值是：`Fit`、`FitAndCenter`、`Fill`。</span><span class="sxs-lookup"><span data-stu-id="9b56d-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="9b56d-145">响应</span><span class="sxs-lookup"><span data-stu-id="9b56d-145">Response</span></span>

<span data-ttu-id="9b56d-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 base-64 图像字符串。</span><span class="sxs-lookup"><span data-stu-id="9b56d-146">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b56d-147">示例</span><span class="sxs-lookup"><span data-stu-id="9b56d-147">Example</span></span>
<span data-ttu-id="9b56d-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9b56d-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b56d-149">请求</span><span class="sxs-lookup"><span data-stu-id="9b56d-149">Request</span></span>
<span data-ttu-id="9b56d-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9b56d-150">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="9b56d-151">响应</span><span class="sxs-lookup"><span data-stu-id="9b56d-151">Response</span></span>
<span data-ttu-id="9b56d-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9b56d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="9b56d-155">用法</span><span class="sxs-lookup"><span data-stu-id="9b56d-155">Usage</span></span>

<span data-ttu-id="9b56d-156">可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。</span><span class="sxs-lookup"><span data-stu-id="9b56d-156">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="9b56d-157">对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。</span><span class="sxs-lookup"><span data-stu-id="9b56d-157">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="9b56d-158">下面的示例展示了使用默认参数返回的图表图像。</span><span class="sxs-lookup"><span data-stu-id="9b56d-158">Here is an example of a chart image returned with the default parameters.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="9b56d-160">若要自定义图像的显示方式，请指定高度、宽度和调整模式。</span><span class="sxs-lookup"><span data-stu-id="9b56d-160">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="9b56d-161">下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。</span><span class="sxs-lookup"><span data-stu-id="9b56d-161">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-fill.png)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart: Image",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
