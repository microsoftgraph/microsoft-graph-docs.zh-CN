---
title: printerDefaults 资源类型
description: 表示打印机的默认设置。 检查打印机的功能以查看它支持的所有值。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fbee453d42fbcb056ce3dce3ff7311e4d976b7dc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516949"
---
# <a name="printerdefaults-resource-type"></a><span data-ttu-id="a4fdc-104">printerDefaults 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4fdc-104">printerDefaults resource type</span></span>

<span data-ttu-id="a4fdc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4fdc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a4fdc-106">表示打印机的默认设置。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-106">Represents the printer's default settings.</span></span> <span data-ttu-id="a4fdc-107">检查打印机 [的功能以查看](printercapabilities.md) 它支持的所有值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-107">Check the printer's [capabilities](printercapabilities.md) to see all the values that it supports.</span></span>

## <a name="properties"></a><span data-ttu-id="a4fdc-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4fdc-108">Properties</span></span>
|<span data-ttu-id="a4fdc-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4fdc-109">Property</span></span>|<span data-ttu-id="a4fdc-110">类型</span><span class="sxs-lookup"><span data-stu-id="a4fdc-110">Type</span></span>|<span data-ttu-id="a4fdc-111">Description</span><span class="sxs-lookup"><span data-stu-id="a4fdc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4fdc-112">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="a4fdc-112">copiesPerJob</span></span>|<span data-ttu-id="a4fdc-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a4fdc-113">Int32</span></span>|<span data-ttu-id="a4fdc-114">每个作业打印的默认副本数。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-114">The default number of copies printed per job.</span></span>|
|<span data-ttu-id="a4fdc-115">contentType</span><span class="sxs-lookup"><span data-stu-id="a4fdc-115">contentType</span></span>|<span data-ttu-id="a4fdc-116">String</span><span class="sxs-lookup"><span data-stu-id="a4fdc-116">String</span></span>|<span data-ttu-id="a4fdc-117">处理文档 (MIME) 类型。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-117">The default content (MIME) type to use when processing documents.</span></span>|
|<span data-ttu-id="a4fdc-118">finishings</span><span class="sxs-lookup"><span data-stu-id="a4fdc-118">finishings</span></span>|<span data-ttu-id="a4fdc-119">[printFinishing](enums.md#printfinishing-values) 集合</span><span class="sxs-lookup"><span data-stu-id="a4fdc-119">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="a4fdc-120">要应用于打印作业的默认完成项集。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-120">The default set of finishings to apply to print jobs.</span></span> <span data-ttu-id="a4fdc-121">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-121">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a4fdc-122">mediaColor</span><span class="sxs-lookup"><span data-stu-id="a4fdc-122">mediaColor</span></span>|<span data-ttu-id="a4fdc-123">String</span><span class="sxs-lookup"><span data-stu-id="a4fdc-123">String</span></span>|<span data-ttu-id="a4fdc-124">默认媒体 (打印文档) 纸张颜色等。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-124">The default media (such as paper) color to print the document on.</span></span>
|<span data-ttu-id="a4fdc-125">mediaType</span><span class="sxs-lookup"><span data-stu-id="a4fdc-125">mediaType</span></span>|<span data-ttu-id="a4fdc-126">String</span><span class="sxs-lookup"><span data-stu-id="a4fdc-126">String</span></span>|<span data-ttu-id="a4fdc-127">默认媒体 (类型，例如) 打印文档的纸张类型。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-127">The default media (such as paper) type to print the document on.</span></span> <span data-ttu-id="a4fdc-128">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-128">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a4fdc-129">mediaSize</span><span class="sxs-lookup"><span data-stu-id="a4fdc-129">mediaSize</span></span>|<span data-ttu-id="a4fdc-130">String</span><span class="sxs-lookup"><span data-stu-id="a4fdc-130">String</span></span>|<span data-ttu-id="a4fdc-131">使用的默认媒体大小。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-131">The default media size to use.</span></span> <span data-ttu-id="a4fdc-132">支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联的打印机支持的任何自定义大小。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-132">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>
|<span data-ttu-id="a4fdc-133">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="a4fdc-133">pagesPerSheet</span></span>|<span data-ttu-id="a4fdc-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a4fdc-134">Int32</span></span>|<span data-ttu-id="a4fdc-135">要在每个工作表上打印的默认文档页数。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-135">The default number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="a4fdc-136">orientation</span><span class="sxs-lookup"><span data-stu-id="a4fdc-136">orientation</span></span>|[<span data-ttu-id="a4fdc-137">printOrientation</span><span class="sxs-lookup"><span data-stu-id="a4fdc-137">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="a4fdc-138">打印文档时使用的默认方向。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-138">The default orientation to use when printing the document.</span></span> <span data-ttu-id="a4fdc-139">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-139">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a4fdc-140">outputBin</span><span class="sxs-lookup"><span data-stu-id="a4fdc-140">outputBin</span></span>|<span data-ttu-id="a4fdc-141">String</span><span class="sxs-lookup"><span data-stu-id="a4fdc-141">String</span></span>|<span data-ttu-id="a4fdc-142">要放置已完成打印的默认输出箱。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-142">The default output bin to place completed prints into.</span></span> <span data-ttu-id="a4fdc-143">有关受支持的 [输出箱](printercapabilities.md) 的列表，请参阅打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-143">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="a4fdc-144">fitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="a4fdc-144">fitPdfToPage</span></span>|<span data-ttu-id="a4fdc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4fdc-145">Boolean</span></span>|<span data-ttu-id="a4fdc-146">默认的 fitPdfToPage 设置。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-146">The default fitPdfToPage setting.</span></span> <span data-ttu-id="a4fdc-147">True 表示 PDF 文档的每一页都适合媒体的物理工作表;false，让打印机决定如何设置展示次数。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-147">True to fit each page of a PDF document to a physical sheet of media; false to let the printer decide how to lay out impressions.</span></span>|
|<span data-ttu-id="a4fdc-148">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="a4fdc-148">multipageLayout</span></span>|[<span data-ttu-id="a4fdc-149">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="a4fdc-149">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="a4fdc-150">当每张工作表打印多个页面时，页面布局的默认方向。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-150">The default direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="a4fdc-151">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-151">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a4fdc-152">colorMode</span><span class="sxs-lookup"><span data-stu-id="a4fdc-152">colorMode</span></span>|[<span data-ttu-id="a4fdc-153">printColorMode</span><span class="sxs-lookup"><span data-stu-id="a4fdc-153">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="a4fdc-154">打印文档时使用的默认颜色模式。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-154">The default color mode to use when printing the document.</span></span> <span data-ttu-id="a4fdc-155">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-155">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a4fdc-156">quality</span><span class="sxs-lookup"><span data-stu-id="a4fdc-156">quality</span></span>|[<span data-ttu-id="a4fdc-157">printQuality</span><span class="sxs-lookup"><span data-stu-id="a4fdc-157">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="a4fdc-158">打印文档时使用的默认质量。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-158">The default quality to use when printing the document.</span></span> <span data-ttu-id="a4fdc-159">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-159">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a4fdc-160">duplexMode</span><span class="sxs-lookup"><span data-stu-id="a4fdc-160">duplexMode</span></span>|[<span data-ttu-id="a4fdc-161">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="a4fdc-161">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="a4fdc-162">默认双面 (双面) 打印文档时使用的配置。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-162">The default duplex (double-sided) configuration to use when printing a document.</span></span> <span data-ttu-id="a4fdc-163">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-163">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a4fdc-164">dpi</span><span class="sxs-lookup"><span data-stu-id="a4fdc-164">dpi</span></span>|<span data-ttu-id="a4fdc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a4fdc-165">Int32</span></span>|<span data-ttu-id="a4fdc-166">打印作业时使用的默认分辨率（DPI）。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-166">The default resolution in DPI to use when printing the job.</span></span>|
|<span data-ttu-id="a4fdc-167">scaling</span><span class="sxs-lookup"><span data-stu-id="a4fdc-167">scaling</span></span>|[<span data-ttu-id="a4fdc-168">printScaling</span><span class="sxs-lookup"><span data-stu-id="a4fdc-168">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="a4fdc-169">指定打印机如何缩放文档数据以适应请求的媒体。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-169">Specifies how the printer scales the document data to fit the requested media.</span></span> <span data-ttu-id="a4fdc-170">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-170">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4fdc-171">关系</span><span class="sxs-lookup"><span data-stu-id="a4fdc-171">Relationships</span></span>
<span data-ttu-id="a4fdc-172">无。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4fdc-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4fdc-173">JSON representation</span></span>
<span data-ttu-id="a4fdc-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4fdc-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDefaults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDefaults",
  "copiesPerJob": "Integer",
  "contentType": "String",
  "finishings": [
    "String"
  ],
  "mediaColor": "String",
  "mediaType": "String",
  "mediaSize": "String",
  "pagesPerSheet": "Integer",
  "orientation": "String",
  "outputBin": "String",
  "inputBin": "String",
  "fitPdfToPage": "Boolean",
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String",
  "dpi": "Integer",
  "scaling": "String"
}
```

