---
title: printerCapabilities 复杂类型
description: 表示打印机报告的功能。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5416cf43e266bab65254ac5aaee1a79c9c3e17be
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516948"
---
# <a name="printercapabilities-resource-type"></a><span data-ttu-id="0e233-103">printerCapabilities 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e233-103">printerCapabilities resource type</span></span>

<span data-ttu-id="0e233-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e233-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0e233-105">表示打印机/打印机共享报告的功能。</span><span class="sxs-lookup"><span data-stu-id="0e233-105">Represents the capabilities reported by a printer/printerShare.</span></span>

## <a name="properties"></a><span data-ttu-id="0e233-106">属性</span><span class="sxs-lookup"><span data-stu-id="0e233-106">Properties</span></span>
| <span data-ttu-id="0e233-107">属性</span><span class="sxs-lookup"><span data-stu-id="0e233-107">Property</span></span>     | <span data-ttu-id="0e233-108">类型</span><span class="sxs-lookup"><span data-stu-id="0e233-108">Type</span></span>        | <span data-ttu-id="0e233-109">Description</span><span class="sxs-lookup"><span data-stu-id="0e233-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e233-110">contentTypes</span><span class="sxs-lookup"><span data-stu-id="0e233-110">contentTypes</span></span>|<span data-ttu-id="0e233-111">String collection</span><span class="sxs-lookup"><span data-stu-id="0e233-111">String collection</span></span>|<span data-ttu-id="0e233-112">打印机支持的 MIME (类型) 支持的内容列表。</span><span class="sxs-lookup"><span data-stu-id="0e233-112">A list of supported content (MIME) types that the printer supports.</span></span> <span data-ttu-id="0e233-113">不保证通用打印服务支持打印所有这些 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="0e233-113">It is not guaranteed that the Universal Print service supports printing all of these MIME types.</span></span>|
|<span data-ttu-id="0e233-114">isColorPrintingSupported</span><span class="sxs-lookup"><span data-stu-id="0e233-114">isColorPrintingSupported</span></span>|<span data-ttu-id="0e233-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e233-115">Boolean</span></span>|<span data-ttu-id="0e233-116">如此 如果打印机支持彩色打印;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="0e233-116">True if color printing is supported by the printer; false otherwise.</span></span> <span data-ttu-id="0e233-117">只读。</span><span class="sxs-lookup"><span data-stu-id="0e233-117">Read-only.</span></span>|
|<span data-ttu-id="0e233-118">feedOrientations</span><span class="sxs-lookup"><span data-stu-id="0e233-118">feedOrientations</span></span>|<span data-ttu-id="0e233-119">printerFeedOrientation 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-119">printerFeedOrientation collection</span></span>|<span data-ttu-id="0e233-120">打印机支持的送纸方向列表。</span><span class="sxs-lookup"><span data-stu-id="0e233-120">The list of feed orientations that are supported by the printer.</span></span>|
|<span data-ttu-id="0e233-121">isPageRangeSupported</span><span class="sxs-lookup"><span data-stu-id="0e233-121">isPageRangeSupported</span></span>|<span data-ttu-id="0e233-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e233-122">Boolean</span></span>|<span data-ttu-id="0e233-123">如此 如果打印机支持按页范围打印;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="0e233-123">True if the printer supports printing by page ranges; false otherwise.</span></span>|
|<span data-ttu-id="0e233-124">质量</span><span class="sxs-lookup"><span data-stu-id="0e233-124">qualities</span></span>|<span data-ttu-id="0e233-125">[printQuality](enums.md#printquality-values) 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-125">[printQuality](enums.md#printquality-values) collection</span></span>|<span data-ttu-id="0e233-126">打印机支持的打印质量。</span><span class="sxs-lookup"><span data-stu-id="0e233-126">The print qualities supported by the printer.</span></span>|
|<span data-ttu-id="0e233-127">dpis</span><span class="sxs-lookup"><span data-stu-id="0e233-127">dpis</span></span>|<span data-ttu-id="0e233-128">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-128">Int32 collection</span></span>|<span data-ttu-id="0e233-129">打印机支持的以 DPI 表示的打印分辨率列表。</span><span class="sxs-lookup"><span data-stu-id="0e233-129">The list of print resolutions in DPI that are supported by the printer.</span></span>|
|<span data-ttu-id="0e233-130">duplexModes</span><span class="sxs-lookup"><span data-stu-id="0e233-130">duplexModes</span></span>|<span data-ttu-id="0e233-131">[printDuplexMode](enums.md#printduplexmode-values) 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-131">[printDuplexMode](enums.md#printduplexmode-values) collection</span></span>|<span data-ttu-id="0e233-132">打印机支持的双面模式列表。</span><span class="sxs-lookup"><span data-stu-id="0e233-132">The list of duplex modes that are supported by the printer.</span></span> <span data-ttu-id="0e233-133">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="0e233-133">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="0e233-134">queueBufferSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="0e233-134">queueBufferSizeInBytes</span></span>|<span data-ttu-id="0e233-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0e233-135">Int32</span></span>|<span data-ttu-id="0e233-136">打印机可存储的最大打印作业队列大小。</span><span class="sxs-lookup"><span data-stu-id="0e233-136">The maximum print job queue size that can be stored by the printer.</span></span>|
|<span data-ttu-id="0e233-137">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="0e233-137">copiesPerJob</span></span>|[<span data-ttu-id="0e233-138">integerRange</span><span class="sxs-lookup"><span data-stu-id="0e233-138">integerRange</span></span>](integerrange.md)|<span data-ttu-id="0e233-139">打印机支持每个作业的副本范围。</span><span class="sxs-lookup"><span data-stu-id="0e233-139">The range of copies per job supported by the printer.</span></span>|
|<span data-ttu-id="0e233-140">finishings</span><span class="sxs-lookup"><span data-stu-id="0e233-140">finishings</span></span>|<span data-ttu-id="0e233-141">[printFinishing](enums.md#printfinishing-values) 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-141">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="0e233-142">打印机支持打印文档的完成过程。</span><span class="sxs-lookup"><span data-stu-id="0e233-142">Finishing processes the printer supports for a printed document.</span></span>|
|<span data-ttu-id="0e233-143">mediaColors</span><span class="sxs-lookup"><span data-stu-id="0e233-143">mediaColors</span></span>|<span data-ttu-id="0e233-144">String collection</span><span class="sxs-lookup"><span data-stu-id="0e233-144">String collection</span></span>|<span data-ttu-id="0e233-145">媒体 (，即纸张) 打印机支持的颜色。</span><span class="sxs-lookup"><span data-stu-id="0e233-145">The media (i.e., paper) colors supported by the printer.</span></span>|
|<span data-ttu-id="0e233-146">mediaTypes</span><span class="sxs-lookup"><span data-stu-id="0e233-146">mediaTypes</span></span>|<span data-ttu-id="0e233-147">String collection</span><span class="sxs-lookup"><span data-stu-id="0e233-147">String collection</span></span>|<span data-ttu-id="0e233-148">打印机支持的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="0e233-148">The media types supported by the printer.</span></span> <span data-ttu-id="0e233-149">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="0e233-149">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="0e233-150">mediaSizes</span><span class="sxs-lookup"><span data-stu-id="0e233-150">mediaSizes</span></span>|<span data-ttu-id="0e233-151">String collection</span><span class="sxs-lookup"><span data-stu-id="0e233-151">String collection</span></span>|<span data-ttu-id="0e233-152">打印机支持的媒体大小。</span><span class="sxs-lookup"><span data-stu-id="0e233-152">The media sizes supported by the printer.</span></span> <span data-ttu-id="0e233-153">支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联的打印机支持的任何自定义大小。</span><span class="sxs-lookup"><span data-stu-id="0e233-153">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>|
|<span data-ttu-id="0e233-154">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="0e233-154">pagesPerSheet</span></span>|<span data-ttu-id="0e233-155">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-155">Int32 collection</span></span>|<span data-ttu-id="0e233-156">支持对单个展示施加的输入页面数。</span><span class="sxs-lookup"><span data-stu-id="0e233-156">Supported number of Input Pages to impose upon a single Impression.</span></span>|
|<span data-ttu-id="0e233-157">orientations</span><span class="sxs-lookup"><span data-stu-id="0e233-157">orientations</span></span>|<span data-ttu-id="0e233-158">[printOrientation](enums.md#printorientation-values) 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-158">[printOrientation](enums.md#printorientation-values) collection</span></span>|<span data-ttu-id="0e233-159">打印机支持的打印方向。</span><span class="sxs-lookup"><span data-stu-id="0e233-159">The print orientations supported by the printer.</span></span> <span data-ttu-id="0e233-160">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="0e233-160">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="0e233-161">inputBins</span><span class="sxs-lookup"><span data-stu-id="0e233-161">inputBins</span></span>|<span data-ttu-id="0e233-162">String collection</span><span class="sxs-lookup"><span data-stu-id="0e233-162">String collection</span></span>|<span data-ttu-id="0e233-163">打印机支持的输入箱。</span><span class="sxs-lookup"><span data-stu-id="0e233-163">Supported input bins for the printer.</span></span>|
|<span data-ttu-id="0e233-164">outputBins</span><span class="sxs-lookup"><span data-stu-id="0e233-164">outputBins</span></span>|<span data-ttu-id="0e233-165">String collection</span><span class="sxs-lookup"><span data-stu-id="0e233-165">String collection</span></span>|<span data-ttu-id="0e233-166">打印机支持的输出箱 (纸盒) 。</span><span class="sxs-lookup"><span data-stu-id="0e233-166">The printer's supported output bins (trays).</span></span>|
|<span data-ttu-id="0e233-167">supportsFitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="0e233-167">supportsFitPdfToPage</span></span>|<span data-ttu-id="0e233-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e233-168">Boolean</span></span>|<span data-ttu-id="0e233-169">如此 如果打印机支持缩放 PDF 页面以匹配打印媒体大小;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="0e233-169">True if the printer supports scaling PDF pages to match the print media size; false otherwise.</span></span>|
|<span data-ttu-id="0e233-170">multipageLayouts</span><span class="sxs-lookup"><span data-stu-id="0e233-170">multipageLayouts</span></span>|<span data-ttu-id="0e233-171">[printMultipageLayout](enums.md#printmultipagelayout-values) 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-171">[printMultipageLayout](enums.md#printmultipagelayout-values) collection</span></span>|<span data-ttu-id="0e233-172">打印机支持的演示方向。</span><span class="sxs-lookup"><span data-stu-id="0e233-172">The presentation directions supported by the printer.</span></span> <span data-ttu-id="0e233-173">下表介绍了受支持的值。</span><span class="sxs-lookup"><span data-stu-id="0e233-173">Supported values are described in the following table.</span></span>|
|<span data-ttu-id="0e233-174">colorModes</span><span class="sxs-lookup"><span data-stu-id="0e233-174">colorModes</span></span>|<span data-ttu-id="0e233-175">[printColorMode](enums.md#printcolormode-values) 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-175">[printColorMode](enums.md#printcolormode-values) collection</span></span>|<span data-ttu-id="0e233-176">打印机支持的颜色模式。</span><span class="sxs-lookup"><span data-stu-id="0e233-176">The color modes supported by the printer.</span></span> <span data-ttu-id="0e233-177">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="0e233-177">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="0e233-178">topMargins</span><span class="sxs-lookup"><span data-stu-id="0e233-178">topMargins</span></span>|<span data-ttu-id="0e233-179">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-179">Int32 collection</span></span>|<span data-ttu-id="0e233-180">支持的上边距列表 (打印机) 以密) 。</span><span class="sxs-lookup"><span data-stu-id="0e233-180">A list of supported top margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="0e233-181">bottomMargins</span><span class="sxs-lookup"><span data-stu-id="0e233-181">bottomMargins</span></span>|<span data-ttu-id="0e233-182">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-182">Int32 collection</span></span>|<span data-ttu-id="0e233-183">支持的底部边距列表 (打印机) 以密) 。</span><span class="sxs-lookup"><span data-stu-id="0e233-183">A list of supported bottom margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="0e233-184">rightMargins</span><span class="sxs-lookup"><span data-stu-id="0e233-184">rightMargins</span></span>|<span data-ttu-id="0e233-185">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-185">Int32 collection</span></span>|<span data-ttu-id="0e233-186">支持的右边距列表 (以) 以小数表示。</span><span class="sxs-lookup"><span data-stu-id="0e233-186">A list of supported right margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="0e233-187">leftMargins</span><span class="sxs-lookup"><span data-stu-id="0e233-187">leftMargins</span></span>|<span data-ttu-id="0e233-188">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-188">Int32 collection</span></span>|<span data-ttu-id="0e233-189">打印机支持的左边距 (以) 以密分表示。</span><span class="sxs-lookup"><span data-stu-id="0e233-189">A list of supported left margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="0e233-190">collation</span><span class="sxs-lookup"><span data-stu-id="0e233-190">collation</span></span>|<span data-ttu-id="0e233-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e233-191">Boolean</span></span>|<span data-ttu-id="0e233-192">如此 如果打印多页文档的副本时打印机支持整理;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="0e233-192">True if the printer supports collating when printing muliple copies of a multi-page document; false otherwise.</span></span>|
|<span data-ttu-id="0e233-193">scalings</span><span class="sxs-lookup"><span data-stu-id="0e233-193">scalings</span></span>|<span data-ttu-id="0e233-194">[printScaling](enums.md#printscaling-values) 集合</span><span class="sxs-lookup"><span data-stu-id="0e233-194">[printScaling](enums.md#printscaling-values) collection</span></span>|<span data-ttu-id="0e233-195">支持的打印缩放。</span><span class="sxs-lookup"><span data-stu-id="0e233-195">Supported print scalings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e233-196">关系</span><span class="sxs-lookup"><span data-stu-id="0e233-196">Relationships</span></span>
<span data-ttu-id="0e233-197">无。</span><span class="sxs-lookup"><span data-stu-id="0e233-197">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e233-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e233-198">JSON representation</span></span>
<span data-ttu-id="0e233-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e233-199">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "contentTypes": [
    "String"
  ],
  "isColorPrintingSupported": "Boolean",
  "feedOrientations": [
    "String"
  ],
  "isPageRangeSupported": "Boolean",
  "qualities": [
    "String"
  ],
  "dpis": [
    "Integer"
  ],
  "duplexModes": [
    "String"
  ],
  "copiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "finishings": [
    "String"
  ],
  "mediaColors": [
    "String"
  ],
  "mediaTypes": [
    "String"
  ],
  "mediaSizes": [
    "String"
  ],
  "pagesPerSheet": [
    "Integer"
  ],
  "orientations": [
    "String"
  ],
  "outputBins": [
    "String"
  ],
  "supportsFitPdfToPage": "Boolean",
  "multipageLayouts": [
    "String"
  ],
  "colorModes": [
    "String"
  ],
  "inputBins": [
    "String"
  ],
  "topMargins": [
    "Integer"
  ],
  "bottomMargins": [
    "Integer"
  ],
  "rightMargins": [
    "Integer"
  ],
  "leftMargins": [
    "Integer"
  ],
  "collation": "Boolean",
  "scalings": [
    "String"
  ]
}
```

