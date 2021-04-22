---
title: printerCapabilities 复杂类型
description: 表示打印机报告的功能。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bda913275aff692df2f66472f61436665cbc3dd7
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944224"
---
# <a name="printercapabilities-resource-type"></a><span data-ttu-id="05f81-103">printerCapabilities 资源类型</span><span class="sxs-lookup"><span data-stu-id="05f81-103">printerCapabilities resource type</span></span>

<span data-ttu-id="05f81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05f81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="05f81-105">表示 printer/printerShare 报告的功能。</span><span class="sxs-lookup"><span data-stu-id="05f81-105">Represents the capabilities reported by a printer/printerShare.</span></span>

## <a name="properties"></a><span data-ttu-id="05f81-106">属性</span><span class="sxs-lookup"><span data-stu-id="05f81-106">Properties</span></span>
| <span data-ttu-id="05f81-107">属性</span><span class="sxs-lookup"><span data-stu-id="05f81-107">Property</span></span>     | <span data-ttu-id="05f81-108">类型</span><span class="sxs-lookup"><span data-stu-id="05f81-108">Type</span></span>        | <span data-ttu-id="05f81-109">说明</span><span class="sxs-lookup"><span data-stu-id="05f81-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="05f81-110">contentTypes</span><span class="sxs-lookup"><span data-stu-id="05f81-110">contentTypes</span></span>|<span data-ttu-id="05f81-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="05f81-111">String collection</span></span>|<span data-ttu-id="05f81-112">受支持内容列表 (打印机) 类型的 MIME。</span><span class="sxs-lookup"><span data-stu-id="05f81-112">A list of supported content (MIME) types that the printer supports.</span></span> <span data-ttu-id="05f81-113">不保证通用打印服务支持打印所有这些 MIME 类型。</span><span class="sxs-lookup"><span data-stu-id="05f81-113">It is not guaranteed that the Universal Print service supports printing all of these MIME types.</span></span>|
|<span data-ttu-id="05f81-114">isColorPrintingSupported</span><span class="sxs-lookup"><span data-stu-id="05f81-114">isColorPrintingSupported</span></span>|<span data-ttu-id="05f81-115">布尔</span><span class="sxs-lookup"><span data-stu-id="05f81-115">Boolean</span></span>|<span data-ttu-id="05f81-116">如此 如果打印机支持彩色打印;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="05f81-116">True if color printing is supported by the printer; false otherwise.</span></span> <span data-ttu-id="05f81-117">只读。</span><span class="sxs-lookup"><span data-stu-id="05f81-117">Read-only.</span></span>|
|<span data-ttu-id="05f81-118">feedOrientations</span><span class="sxs-lookup"><span data-stu-id="05f81-118">feedOrientations</span></span>|<span data-ttu-id="05f81-119">printerFeedOrientation 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-119">printerFeedOrientation collection</span></span>|<span data-ttu-id="05f81-120">打印机支持的送纸方向列表。</span><span class="sxs-lookup"><span data-stu-id="05f81-120">The list of feed orientations that are supported by the printer.</span></span>|
|<span data-ttu-id="05f81-121">isPageRangeSupported</span><span class="sxs-lookup"><span data-stu-id="05f81-121">isPageRangeSupported</span></span>|<span data-ttu-id="05f81-122">布尔</span><span class="sxs-lookup"><span data-stu-id="05f81-122">Boolean</span></span>|<span data-ttu-id="05f81-123">如此 如果打印机支持按页范围打印;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="05f81-123">True if the printer supports printing by page ranges; false otherwise.</span></span>|
|<span data-ttu-id="05f81-124">一些</span><span class="sxs-lookup"><span data-stu-id="05f81-124">qualities</span></span>|<span data-ttu-id="05f81-125">[printQuality](enums.md#printquality-values) 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-125">[printQuality](enums.md#printquality-values) collection</span></span>|<span data-ttu-id="05f81-126">打印机支持的打印质量。</span><span class="sxs-lookup"><span data-stu-id="05f81-126">The print qualities supported by the printer.</span></span>|
|<span data-ttu-id="05f81-127">dpis</span><span class="sxs-lookup"><span data-stu-id="05f81-127">dpis</span></span>|<span data-ttu-id="05f81-128">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-128">Int32 collection</span></span>|<span data-ttu-id="05f81-129">打印机支持的以 DPI 表示的打印分辨率列表。</span><span class="sxs-lookup"><span data-stu-id="05f81-129">The list of print resolutions in DPI that are supported by the printer.</span></span>|
|<span data-ttu-id="05f81-130">duplexModes</span><span class="sxs-lookup"><span data-stu-id="05f81-130">duplexModes</span></span>|<span data-ttu-id="05f81-131">[printDuplexMode](enums.md#printduplexmode-values) 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-131">[printDuplexMode](enums.md#printduplexmode-values) collection</span></span>|<span data-ttu-id="05f81-132">打印机支持的双面模式列表。</span><span class="sxs-lookup"><span data-stu-id="05f81-132">The list of duplex modes that are supported by the printer.</span></span> <span data-ttu-id="05f81-133">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="05f81-133">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="05f81-134">queueBufferSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="05f81-134">queueBufferSizeInBytes</span></span>|<span data-ttu-id="05f81-135">Int32</span><span class="sxs-lookup"><span data-stu-id="05f81-135">Int32</span></span>|<span data-ttu-id="05f81-136">打印机可以存储的最大打印作业队列大小。</span><span class="sxs-lookup"><span data-stu-id="05f81-136">The maximum print job queue size that can be stored by the printer.</span></span>|
|<span data-ttu-id="05f81-137">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="05f81-137">copiesPerJob</span></span>|[<span data-ttu-id="05f81-138">integerRange</span><span class="sxs-lookup"><span data-stu-id="05f81-138">integerRange</span></span>](integerrange.md)|<span data-ttu-id="05f81-139">打印机支持每个作业的副本范围。</span><span class="sxs-lookup"><span data-stu-id="05f81-139">The range of copies per job supported by the printer.</span></span>|
|<span data-ttu-id="05f81-140">finishings</span><span class="sxs-lookup"><span data-stu-id="05f81-140">finishings</span></span>|<span data-ttu-id="05f81-141">[printFinishing](enums.md#printfinishing-values) 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-141">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="05f81-142">打印机对打印文档支持的完成过程。</span><span class="sxs-lookup"><span data-stu-id="05f81-142">Finishing processes the printer supports for a printed document.</span></span>|
|<span data-ttu-id="05f81-143">mediaColors</span><span class="sxs-lookup"><span data-stu-id="05f81-143">mediaColors</span></span>|<span data-ttu-id="05f81-144">字符串集合</span><span class="sxs-lookup"><span data-stu-id="05f81-144">String collection</span></span>|<span data-ttu-id="05f81-145">媒体 (即纸张) 打印机支持的颜色。</span><span class="sxs-lookup"><span data-stu-id="05f81-145">The media (i.e., paper) colors supported by the printer.</span></span>|
|<span data-ttu-id="05f81-146">mediaTypes</span><span class="sxs-lookup"><span data-stu-id="05f81-146">mediaTypes</span></span>|<span data-ttu-id="05f81-147">字符串集合</span><span class="sxs-lookup"><span data-stu-id="05f81-147">String collection</span></span>|<span data-ttu-id="05f81-148">打印机支持的媒体类型。</span><span class="sxs-lookup"><span data-stu-id="05f81-148">The media types supported by the printer.</span></span>|
|<span data-ttu-id="05f81-149">mediaSizes</span><span class="sxs-lookup"><span data-stu-id="05f81-149">mediaSizes</span></span>|<span data-ttu-id="05f81-150">字符串集合</span><span class="sxs-lookup"><span data-stu-id="05f81-150">String collection</span></span>|<span data-ttu-id="05f81-151">打印机支持的媒体大小。</span><span class="sxs-lookup"><span data-stu-id="05f81-151">The media sizes supported by the printer.</span></span> <span data-ttu-id="05f81-152">支持 ISO 和 ANSI 媒体大小的标准大小名称。</span><span class="sxs-lookup"><span data-stu-id="05f81-152">Supports standard size names for ISO and ANSI media sizes.</span></span> <span data-ttu-id="05f81-153">有效值如下表 [所示](#mediasizes-values)。</span><span class="sxs-lookup"><span data-stu-id="05f81-153">Valid values are in the following [table](#mediasizes-values).</span></span>|
|<span data-ttu-id="05f81-154">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="05f81-154">pagesPerSheet</span></span>|<span data-ttu-id="05f81-155">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-155">Int32 collection</span></span>|<span data-ttu-id="05f81-156">支持对单个展示施加的输入页面数。</span><span class="sxs-lookup"><span data-stu-id="05f81-156">Supported number of Input Pages to impose upon a single Impression.</span></span>|
|<span data-ttu-id="05f81-157">orientations</span><span class="sxs-lookup"><span data-stu-id="05f81-157">orientations</span></span>|<span data-ttu-id="05f81-158">[printOrientation](enums.md#printorientation-values) 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-158">[printOrientation](enums.md#printorientation-values) collection</span></span>|<span data-ttu-id="05f81-159">打印机支持的打印方向。</span><span class="sxs-lookup"><span data-stu-id="05f81-159">The print orientations supported by the printer.</span></span> <span data-ttu-id="05f81-160">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="05f81-160">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="05f81-161">inputBins</span><span class="sxs-lookup"><span data-stu-id="05f81-161">inputBins</span></span>|<span data-ttu-id="05f81-162">字符串集合</span><span class="sxs-lookup"><span data-stu-id="05f81-162">String collection</span></span>|<span data-ttu-id="05f81-163">打印机支持的输入箱。</span><span class="sxs-lookup"><span data-stu-id="05f81-163">Supported input bins for the printer.</span></span>|
|<span data-ttu-id="05f81-164">outputBins</span><span class="sxs-lookup"><span data-stu-id="05f81-164">outputBins</span></span>|<span data-ttu-id="05f81-165">字符串集合</span><span class="sxs-lookup"><span data-stu-id="05f81-165">String collection</span></span>|<span data-ttu-id="05f81-166">打印机支持的输出箱 (纸盒) 。</span><span class="sxs-lookup"><span data-stu-id="05f81-166">The printer's supported output bins (trays).</span></span>|
|<span data-ttu-id="05f81-167">supportsFitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="05f81-167">supportsFitPdfToPage</span></span>|<span data-ttu-id="05f81-168">布尔</span><span class="sxs-lookup"><span data-stu-id="05f81-168">Boolean</span></span>|<span data-ttu-id="05f81-169">如此 如果打印机支持缩放 PDF 页面以匹配打印媒体大小;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="05f81-169">True if the printer supports scaling PDF pages to match the print media size; false otherwise.</span></span>|
|<span data-ttu-id="05f81-170">multipageLayouts</span><span class="sxs-lookup"><span data-stu-id="05f81-170">multipageLayouts</span></span>|<span data-ttu-id="05f81-171">[printMultipageLayout](enums.md#printmultipagelayout-values) 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-171">[printMultipageLayout](enums.md#printmultipagelayout-values) collection</span></span>|<span data-ttu-id="05f81-172">打印机支持的演示文稿方向。</span><span class="sxs-lookup"><span data-stu-id="05f81-172">The presentation directions supported by the printer.</span></span> <span data-ttu-id="05f81-173">下表介绍了支持的值。</span><span class="sxs-lookup"><span data-stu-id="05f81-173">Supported values are described in the following table.</span></span>|
|<span data-ttu-id="05f81-174">colorModes</span><span class="sxs-lookup"><span data-stu-id="05f81-174">colorModes</span></span>|<span data-ttu-id="05f81-175">[printColorMode](enums.md#printcolormode-values) 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-175">[printColorMode](enums.md#printcolormode-values) collection</span></span>|<span data-ttu-id="05f81-176">打印机支持的颜色模式。</span><span class="sxs-lookup"><span data-stu-id="05f81-176">The color modes supported by the printer.</span></span> <span data-ttu-id="05f81-177">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="05f81-177">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="05f81-178">topMargins</span><span class="sxs-lookup"><span data-stu-id="05f81-178">topMargins</span></span>|<span data-ttu-id="05f81-179">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-179">Int32 collection</span></span>|<span data-ttu-id="05f81-180">打印机支持的上边距 (以) 表示。</span><span class="sxs-lookup"><span data-stu-id="05f81-180">A list of supported top margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05f81-181">bottomMargins</span><span class="sxs-lookup"><span data-stu-id="05f81-181">bottomMargins</span></span>|<span data-ttu-id="05f81-182">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-182">Int32 collection</span></span>|<span data-ttu-id="05f81-183">支持的底部边距列表 (打印机) 以百分之位表示。</span><span class="sxs-lookup"><span data-stu-id="05f81-183">A list of supported bottom margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05f81-184">rightMargins</span><span class="sxs-lookup"><span data-stu-id="05f81-184">rightMargins</span></span>|<span data-ttu-id="05f81-185">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-185">Int32 collection</span></span>|<span data-ttu-id="05f81-186">打印机支持的右边距 (以) 表示。</span><span class="sxs-lookup"><span data-stu-id="05f81-186">A list of supported right margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05f81-187">leftMargins</span><span class="sxs-lookup"><span data-stu-id="05f81-187">leftMargins</span></span>|<span data-ttu-id="05f81-188">Int32 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-188">Int32 collection</span></span>|<span data-ttu-id="05f81-189">支持的左边距列表 (打印机) 的边距。</span><span class="sxs-lookup"><span data-stu-id="05f81-189">A list of supported left margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05f81-190">collation</span><span class="sxs-lookup"><span data-stu-id="05f81-190">collation</span></span>|<span data-ttu-id="05f81-191">布尔</span><span class="sxs-lookup"><span data-stu-id="05f81-191">Boolean</span></span>|<span data-ttu-id="05f81-192">如此 如果打印机支持逐份打印多页文档的副本;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="05f81-192">True if the printer supports collating when printing muliple copies of a multi-page document; false otherwise.</span></span>|
|<span data-ttu-id="05f81-193">scalings</span><span class="sxs-lookup"><span data-stu-id="05f81-193">scalings</span></span>|<span data-ttu-id="05f81-194">[printScaling](enums.md#printscaling-values) 集合</span><span class="sxs-lookup"><span data-stu-id="05f81-194">[printScaling](enums.md#printscaling-values) collection</span></span>|<span data-ttu-id="05f81-195">支持的打印缩放。</span><span class="sxs-lookup"><span data-stu-id="05f81-195">Supported print scalings.</span></span>|

### <a name="mediasizes-values"></a><span data-ttu-id="05f81-196">mediaSizes 值</span><span class="sxs-lookup"><span data-stu-id="05f81-196">mediaSizes values</span></span>

|<span data-ttu-id="05f81-197">值</span><span class="sxs-lookup"><span data-stu-id="05f81-197">Value</span></span>|
|:---|
|<span data-ttu-id="05f81-198">A3</span><span class="sxs-lookup"><span data-stu-id="05f81-198">A3</span></span>|
|<span data-ttu-id="05f81-199">A4</span><span class="sxs-lookup"><span data-stu-id="05f81-199">A4</span></span>|
|<span data-ttu-id="05f81-200">A5</span><span class="sxs-lookup"><span data-stu-id="05f81-200">A5</span></span>|
|<span data-ttu-id="05f81-201">A6</span><span class="sxs-lookup"><span data-stu-id="05f81-201">A6</span></span>|
|<span data-ttu-id="05f81-202">JIS B4</span><span class="sxs-lookup"><span data-stu-id="05f81-202">JIS B4</span></span>|
|<span data-ttu-id="05f81-203">JIS B5</span><span class="sxs-lookup"><span data-stu-id="05f81-203">JIS B5</span></span>|
|<span data-ttu-id="05f81-204">JPN Hag一</span><span class="sxs-lookup"><span data-stu-id="05f81-204">JPN Hagaki</span></span>|
|<span data-ttu-id="05f81-205">北美 5x7in</span><span class="sxs-lookup"><span data-stu-id="05f81-205">North America 5x7in</span></span>|
|<span data-ttu-id="05f81-206">北美管理人员</span><span class="sxs-lookup"><span data-stu-id="05f81-206">North America Executive</span></span>|
|<span data-ttu-id="05f81-207">北美 Goverment 信函</span><span class="sxs-lookup"><span data-stu-id="05f81-207">North America Goverment Letter</span></span>|
|<span data-ttu-id="05f81-208">北美索引 3x5in</span><span class="sxs-lookup"><span data-stu-id="05f81-208">North America Index 3x5in</span></span>|
|<span data-ttu-id="05f81-209">北美索引 4x8in</span><span class="sxs-lookup"><span data-stu-id="05f81-209">North America Index 4x8in</span></span>|
|<span data-ttu-id="05f81-210">北美索引 5x8in</span><span class="sxs-lookup"><span data-stu-id="05f81-210">North America Index 5x8in</span></span>|
|<span data-ttu-id="05f81-211">北美发票</span><span class="sxs-lookup"><span data-stu-id="05f81-211">North America Invoice</span></span>|
|<span data-ttu-id="05f81-212">北美分类帐</span><span class="sxs-lookup"><span data-stu-id="05f81-212">North America Ledger</span></span>|
|<span data-ttu-id="05f81-213">北美法律</span><span class="sxs-lookup"><span data-stu-id="05f81-213">North America Legal</span></span>|
|<span data-ttu-id="05f81-214">北美字母</span><span class="sxs-lookup"><span data-stu-id="05f81-214">North America Letter</span></span>|
|<span data-ttu-id="05f81-215">Photo l 3.5x5in</span><span class="sxs-lookup"><span data-stu-id="05f81-215">Photo l 3.5x5in</span></span>|
|<span data-ttu-id="05f81-216">名片</span><span class="sxs-lookup"><span data-stu-id="05f81-216">Business Card</span></span>|
|<span data-ttu-id="05f81-217">Photo</span><span class="sxs-lookup"><span data-stu-id="05f81-217">Photo</span></span>|

## <a name="relationships"></a><span data-ttu-id="05f81-218">关系</span><span class="sxs-lookup"><span data-stu-id="05f81-218">Relationships</span></span>
<span data-ttu-id="05f81-219">无。</span><span class="sxs-lookup"><span data-stu-id="05f81-219">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05f81-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05f81-220">JSON representation</span></span>
<span data-ttu-id="05f81-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05f81-221">The following is a JSON representation of the resource.</span></span>
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

