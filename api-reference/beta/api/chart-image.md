---
title: 图表：图像
description: 通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5892864d8adb94c4c6193dc4776f8febd938ff36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456530"
---
# <a name="chart-image"></a><span data-ttu-id="cba1d-103">图表：图像</span><span class="sxs-lookup"><span data-stu-id="cba1d-103">Chart: Image</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cba1d-104">通过缩放图表以适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="cba1d-104">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>
## <a name="permissions"></a><span data-ttu-id="cba1d-105">权限</span><span class="sxs-lookup"><span data-stu-id="cba1d-105">Permissions</span></span>
<span data-ttu-id="cba1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cba1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cba1d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cba1d-108">Permission type</span></span>      | <span data-ttu-id="cba1d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cba1d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cba1d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cba1d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cba1d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba1d-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cba1d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cba1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cba1d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba1d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cba1d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cba1d-114">Application</span></span> | <span data-ttu-id="cba1d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cba1d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cba1d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cba1d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')

```
## <a name="request-headers"></a><span data-ttu-id="cba1d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cba1d-117">Request headers</span></span>
| <span data-ttu-id="cba1d-118">名称</span><span class="sxs-lookup"><span data-stu-id="cba1d-118">Name</span></span>       | <span data-ttu-id="cba1d-119">说明</span><span class="sxs-lookup"><span data-stu-id="cba1d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cba1d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba1d-120">Authorization</span></span>  | <span data-ttu-id="cba1d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cba1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cba1d-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cba1d-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cba1d-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="cba1d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cba1d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cba1d-126">Request body</span></span>
<span data-ttu-id="cba1d-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cba1d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cba1d-128">参数</span><span class="sxs-lookup"><span data-stu-id="cba1d-128">Parameter</span></span>    | <span data-ttu-id="cba1d-129">类型</span><span class="sxs-lookup"><span data-stu-id="cba1d-129">Type</span></span>   |<span data-ttu-id="cba1d-130">说明</span><span class="sxs-lookup"><span data-stu-id="cba1d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cba1d-131">height</span><span class="sxs-lookup"><span data-stu-id="cba1d-131">height</span></span>|<span data-ttu-id="cba1d-132">number</span><span class="sxs-lookup"><span data-stu-id="cba1d-132">number</span></span>|<span data-ttu-id="cba1d-p104">可选。生成的图像的所需高度。</span><span class="sxs-lookup"><span data-stu-id="cba1d-p104">Optional. The desired height of the resulting image.</span></span>|
|<span data-ttu-id="cba1d-135">width</span><span class="sxs-lookup"><span data-stu-id="cba1d-135">width</span></span>|<span data-ttu-id="cba1d-136">number</span><span class="sxs-lookup"><span data-stu-id="cba1d-136">number</span></span>|<span data-ttu-id="cba1d-p105">可选。生成的图像的所需宽度。</span><span class="sxs-lookup"><span data-stu-id="cba1d-p105">Optional. The desired width of the resulting image.</span></span>|
|<span data-ttu-id="cba1d-139">fittingMode</span><span class="sxs-lookup"><span data-stu-id="cba1d-139">fittingMode</span></span>|<span data-ttu-id="cba1d-140">string</span><span class="sxs-lookup"><span data-stu-id="cba1d-140">string</span></span>|<span data-ttu-id="cba1d-p106">可选。该方法用于将图表缩放到指定的尺寸（如果设置了高度和宽度）。”可能的值是：`Fit`、`FitAndCenter`、`Fill`。</span><span class="sxs-lookup"><span data-stu-id="cba1d-p106">Optional. The method used to scale the chart to the specified to the specified dimensions (if both height and width are set)."  Possible values are: `Fit`, `FitAndCenter`, `Fill`.</span></span>|

## <a name="response"></a><span data-ttu-id="cba1d-144">响应</span><span class="sxs-lookup"><span data-stu-id="cba1d-144">Response</span></span>

<span data-ttu-id="cba1d-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 base-64 图像字符串。</span><span class="sxs-lookup"><span data-stu-id="cba1d-145">If successful, this method returns `200 OK` response code and base-64 image string in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba1d-146">示例</span><span class="sxs-lookup"><span data-stu-id="cba1d-146">Example</span></span>
<span data-ttu-id="cba1d-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="cba1d-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cba1d-148">请求</span><span class="sxs-lookup"><span data-stu-id="cba1d-148">Request</span></span>
<span data-ttu-id="cba1d-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cba1d-149">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/Image(width=0,height=0,fittingMode='fit')
```

##### <a name="response"></a><span data-ttu-id="cba1d-150">响应</span><span class="sxs-lookup"><span data-stu-id="cba1d-150">Response</span></span>
<span data-ttu-id="cba1d-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cba1d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3

{
"value" : "base-64 chart image string"
}
```

##### <a name="usage"></a><span data-ttu-id="cba1d-154">用法</span><span class="sxs-lookup"><span data-stu-id="cba1d-154">Usage</span></span>

<span data-ttu-id="cba1d-155">可以在 HTML 图像标记内显示 base-64 字符串：`<img src="data:image/png;base64,{base-64 chart image string}/>`。</span><span class="sxs-lookup"><span data-stu-id="cba1d-155">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="cba1d-156">对于默认行为，请使用 `Image(width=0,height=0,fittingMode='fit')`。</span><span class="sxs-lookup"><span data-stu-id="cba1d-156">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="cba1d-157">下面的示例展示了使用默认参数返回的图表图像。</span><span class="sxs-lookup"><span data-stu-id="cba1d-157">Here is an example of a chart image returned with the default parameters.</span></span>

![使用默认高度和宽度的 Excel 图表图像。](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="cba1d-159">若要自定义图像的显示方式，请指定高度、宽度和调整模式。</span><span class="sxs-lookup"><span data-stu-id="cba1d-159">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="cba1d-160">下面展示了使用 `Image(width=500,height=500,fittingMode='Fill')` 参数检索的同一个图表图像。</span><span class="sxs-lookup"><span data-stu-id="cba1d-160">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/chart-image.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
