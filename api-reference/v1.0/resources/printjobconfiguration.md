---
title: printJobConfiguration 资源类型
description: 打印机用于打印作业的一组设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f848b9274172113404a39f13e42c003643dfdf74
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944239"
---
# <a name="printjobconfiguration-resource-type"></a><span data-ttu-id="dfeca-103">printJobConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfeca-103">printJobConfiguration resource type</span></span>

<span data-ttu-id="dfeca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfeca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="dfeca-105">打印机用于打印作业的一组设置。</span><span class="sxs-lookup"><span data-stu-id="dfeca-105">A group of settings that a printer should use to print a job.</span></span>

## <a name="properties"></a><span data-ttu-id="dfeca-106">属性</span><span class="sxs-lookup"><span data-stu-id="dfeca-106">Properties</span></span>
|<span data-ttu-id="dfeca-107">属性</span><span class="sxs-lookup"><span data-stu-id="dfeca-107">Property</span></span>|<span data-ttu-id="dfeca-108">类型</span><span class="sxs-lookup"><span data-stu-id="dfeca-108">Type</span></span>|<span data-ttu-id="dfeca-109">说明</span><span class="sxs-lookup"><span data-stu-id="dfeca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfeca-110">pageRanges</span><span class="sxs-lookup"><span data-stu-id="dfeca-110">pageRanges</span></span>|<span data-ttu-id="dfeca-111">[integerRange](integerrange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfeca-111">[integerRange](integerrange.md) collection</span></span>|<span data-ttu-id="dfeca-112">要打印的页面范围。</span><span class="sxs-lookup"><span data-stu-id="dfeca-112">The page ranges to print.</span></span> <span data-ttu-id="dfeca-113">只读。</span><span class="sxs-lookup"><span data-stu-id="dfeca-113">Read-only.</span></span>|
|<span data-ttu-id="dfeca-114">quality</span><span class="sxs-lookup"><span data-stu-id="dfeca-114">quality</span></span>|[<span data-ttu-id="dfeca-115">printQuality</span><span class="sxs-lookup"><span data-stu-id="dfeca-115">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="dfeca-116">打印作业时使用的打印质量。</span><span class="sxs-lookup"><span data-stu-id="dfeca-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="dfeca-117">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-117">Valid values are described in the table below.</span></span> <span data-ttu-id="dfeca-118">只读。</span><span class="sxs-lookup"><span data-stu-id="dfeca-118">Read-only.</span></span>|
|<span data-ttu-id="dfeca-119">dpi</span><span class="sxs-lookup"><span data-stu-id="dfeca-119">dpi</span></span>|<span data-ttu-id="dfeca-120">Int32</span><span class="sxs-lookup"><span data-stu-id="dfeca-120">Int32</span></span>|<span data-ttu-id="dfeca-121">打印作业时使用的分辨率，以每英寸点数表示 (DPI) 。</span><span class="sxs-lookup"><span data-stu-id="dfeca-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="dfeca-122">只读。</span><span class="sxs-lookup"><span data-stu-id="dfeca-122">Read-only.</span></span>|
|<span data-ttu-id="dfeca-123">feedOrientation</span><span class="sxs-lookup"><span data-stu-id="dfeca-123">feedOrientation</span></span>|<span data-ttu-id="dfeca-124">printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="dfeca-124">printerFeedOrientation</span></span>|<span data-ttu-id="dfeca-125">将媒体馈送到打印机时使用的方向。</span><span class="sxs-lookup"><span data-stu-id="dfeca-125">The orientation to use when feeding media into the printer.</span></span> <span data-ttu-id="dfeca-126">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-126">Valid values are described in the following table.</span></span> <span data-ttu-id="dfeca-127">只读。</span><span class="sxs-lookup"><span data-stu-id="dfeca-127">Read-only.</span></span>|
|<span data-ttu-id="dfeca-128">orientation</span><span class="sxs-lookup"><span data-stu-id="dfeca-128">orientation</span></span>|[<span data-ttu-id="dfeca-129">printOrientation</span><span class="sxs-lookup"><span data-stu-id="dfeca-129">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="dfeca-130">打印作业时打印机应该使用的方向设置。</span><span class="sxs-lookup"><span data-stu-id="dfeca-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="dfeca-131">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="dfeca-132">duplexMode</span><span class="sxs-lookup"><span data-stu-id="dfeca-132">duplexMode</span></span>|[<span data-ttu-id="dfeca-133">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="dfeca-133">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="dfeca-134">打印作业时打印机应该使用的双面模式。</span><span class="sxs-lookup"><span data-stu-id="dfeca-134">The duplex mode the printer should use when printing the job.</span></span> <span data-ttu-id="dfeca-135">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-135">Valid values are described in the table below.</span></span> <span data-ttu-id="dfeca-136">只读。</span><span class="sxs-lookup"><span data-stu-id="dfeca-136">Read-only.</span></span>|
|<span data-ttu-id="dfeca-137">copies</span><span class="sxs-lookup"><span data-stu-id="dfeca-137">copies</span></span>|<span data-ttu-id="dfeca-138">Int32</span><span class="sxs-lookup"><span data-stu-id="dfeca-138">Int32</span></span>|<span data-ttu-id="dfeca-139">应打印的副本数。</span><span class="sxs-lookup"><span data-stu-id="dfeca-139">The number of copies that should be printed.</span></span> <span data-ttu-id="dfeca-140">只读。</span><span class="sxs-lookup"><span data-stu-id="dfeca-140">Read-only.</span></span>|
|<span data-ttu-id="dfeca-141">colorMode</span><span class="sxs-lookup"><span data-stu-id="dfeca-141">colorMode</span></span>|[<span data-ttu-id="dfeca-142">printColorMode</span><span class="sxs-lookup"><span data-stu-id="dfeca-142">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="dfeca-143">打印机用于打印作业的颜色模式。</span><span class="sxs-lookup"><span data-stu-id="dfeca-143">The color mode the printer should use to print the job.</span></span> <span data-ttu-id="dfeca-144">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-144">Valid values are described in the table below.</span></span> <span data-ttu-id="dfeca-145">只读。</span><span class="sxs-lookup"><span data-stu-id="dfeca-145">Read-only.</span></span>|
|<span data-ttu-id="dfeca-146">inputBin</span><span class="sxs-lookup"><span data-stu-id="dfeca-146">inputBin</span></span>|<span data-ttu-id="dfeca-147">String</span><span class="sxs-lookup"><span data-stu-id="dfeca-147">String</span></span>|<span data-ttu-id="dfeca-148">打印时 (纸盒) 纸盒。</span><span class="sxs-lookup"><span data-stu-id="dfeca-148">The input bin (tray) to use when printing.</span></span> <span data-ttu-id="dfeca-149">有关受支持的 [输入箱](printercapabilities.md) 的列表，请参阅打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="dfeca-149">See the printer's [capabilities](printercapabilities.md) for a list of supported input bins.</span></span>|
|<span data-ttu-id="dfeca-150">outputBin</span><span class="sxs-lookup"><span data-stu-id="dfeca-150">outputBin</span></span>|<span data-ttu-id="dfeca-151">String</span><span class="sxs-lookup"><span data-stu-id="dfeca-151">String</span></span>|<span data-ttu-id="dfeca-152">要放入已完成打印输出的输出箱。</span><span class="sxs-lookup"><span data-stu-id="dfeca-152">The output bin to place completed prints into.</span></span> <span data-ttu-id="dfeca-153">有关受支持的 [输出箱](printercapabilities.md) 的列表，请参阅打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="dfeca-153">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="dfeca-154">mediaSize</span><span class="sxs-lookup"><span data-stu-id="dfeca-154">mediaSize</span></span>|<span data-ttu-id="dfeca-155">String</span><span class="sxs-lookup"><span data-stu-id="dfeca-155">String</span></span>|<span data-ttu-id="dfeca-156">打印时使用的媒体大小。</span><span class="sxs-lookup"><span data-stu-id="dfeca-156">The media size to use when printing.</span></span> <span data-ttu-id="dfeca-157">支持 ISO 和 ANSI 媒体大小的标准大小名称。</span><span class="sxs-lookup"><span data-stu-id="dfeca-157">Supports standard size names for ISO and ANSI media sizes.</span></span> <span data-ttu-id="dfeca-158">[printerCapabilities](printercapabilities.md#mediasizes-values)主题中列出的有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-158">Valid values listed in the [printerCapabilities](printercapabilities.md#mediasizes-values) topic.</span></span>|
|<span data-ttu-id="dfeca-159">margin</span><span class="sxs-lookup"><span data-stu-id="dfeca-159">margin</span></span>|[<span data-ttu-id="dfeca-160">printMargin</span><span class="sxs-lookup"><span data-stu-id="dfeca-160">printMargin</span></span>](printmargin.md)|<span data-ttu-id="dfeca-161">打印时使用的边距设置。</span><span class="sxs-lookup"><span data-stu-id="dfeca-161">The margin settings to use when printing.</span></span>|
|<span data-ttu-id="dfeca-162">mediaType</span><span class="sxs-lookup"><span data-stu-id="dfeca-162">mediaType</span></span>|<span data-ttu-id="dfeca-163">String</span><span class="sxs-lookup"><span data-stu-id="dfeca-163">String</span></span>|<span data-ttu-id="dfeca-164">默认媒体 (，如) 打印文档的类型。</span><span class="sxs-lookup"><span data-stu-id="dfeca-164">The default media (such as paper) type to print the document on.</span></span>|
|<span data-ttu-id="dfeca-165">finishings</span><span class="sxs-lookup"><span data-stu-id="dfeca-165">finishings</span></span>|<span data-ttu-id="dfeca-166">[printFinishing](enums.md#printfinishing-values) 集合</span><span class="sxs-lookup"><span data-stu-id="dfeca-166">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="dfeca-167">完成打印时使用的过程。</span><span class="sxs-lookup"><span data-stu-id="dfeca-167">Finishing processes to use when printing.</span></span>|
|<span data-ttu-id="dfeca-168">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="dfeca-168">pagesPerSheet</span></span>|<span data-ttu-id="dfeca-169">Int32</span><span class="sxs-lookup"><span data-stu-id="dfeca-169">Int32</span></span>|<span data-ttu-id="dfeca-170">每张工作表上要打印的文档页数。</span><span class="sxs-lookup"><span data-stu-id="dfeca-170">The number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="dfeca-171">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="dfeca-171">multipageLayout</span></span>|[<span data-ttu-id="dfeca-172">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="dfeca-172">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="dfeca-173">每张工作表打印多个页面时布局页面的方向。</span><span class="sxs-lookup"><span data-stu-id="dfeca-173">The direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="dfeca-174">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-174">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="dfeca-175">collate</span><span class="sxs-lookup"><span data-stu-id="dfeca-175">collate</span></span>|<span data-ttu-id="dfeca-176">布尔</span><span class="sxs-lookup"><span data-stu-id="dfeca-176">Boolean</span></span>|<span data-ttu-id="dfeca-177">打印多页文档的多个副本时，打印机是否应该整理页面。</span><span class="sxs-lookup"><span data-stu-id="dfeca-177">Whether the printer should collate pages wehen printing multiple copies of a multi-page document.</span></span>|
|<span data-ttu-id="dfeca-178">scaling</span><span class="sxs-lookup"><span data-stu-id="dfeca-178">scaling</span></span>|[<span data-ttu-id="dfeca-179">printScaling</span><span class="sxs-lookup"><span data-stu-id="dfeca-179">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="dfeca-180">指定打印机如何缩放文档数据以适应请求的媒体。</span><span class="sxs-lookup"><span data-stu-id="dfeca-180">Specifies how the printer should scale the document data to fit the requested media.</span></span> <span data-ttu-id="dfeca-181">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="dfeca-181">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfeca-182">关系</span><span class="sxs-lookup"><span data-stu-id="dfeca-182">Relationships</span></span>
<span data-ttu-id="dfeca-183">无。</span><span class="sxs-lookup"><span data-stu-id="dfeca-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfeca-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfeca-184">JSON representation</span></span>
<span data-ttu-id="dfeca-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfeca-185">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobConfiguration",
  "pageRanges": [
    {
      "@odata.type": "microsoft.graph.integerRange"
    }
  ],
  "quality": "String",
  "dpi": "Integer",
  "feedOrientation": "String",
  "orientation": "String",
  "duplexMode": "String",
  "copies": "Integer",
  "colorMode": "String",
  "inputBin": "String",
  "outputBin": "String",
  "mediaSize": "String",
  "margin": {
    "@odata.type": "microsoft.graph.printMargin"
  },
  "mediaType": "String",
  "finishings": [
    "String"
  ],
  "pagesPerSheet": "Integer",
  "multipageLayout": "String",
  "collate": "Boolean",
  "scaling": "String",
  "fitPdfToPage": "Boolean"
}
```

