---
title: printJobConfiguration 资源类型
description: 打印机用于打印作业的一组设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1e12541bd4426dca1e0d7b48b0e3bcbd9e2bb7ea
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517294"
---
# <a name="printjobconfiguration-resource-type"></a><span data-ttu-id="54573-103">printJobConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="54573-103">printJobConfiguration resource type</span></span>

<span data-ttu-id="54573-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54573-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="54573-105">打印机用于打印作业的一组设置。</span><span class="sxs-lookup"><span data-stu-id="54573-105">A group of settings that a printer should use to print a job.</span></span>

## <a name="properties"></a><span data-ttu-id="54573-106">属性</span><span class="sxs-lookup"><span data-stu-id="54573-106">Properties</span></span>
|<span data-ttu-id="54573-107">属性</span><span class="sxs-lookup"><span data-stu-id="54573-107">Property</span></span>|<span data-ttu-id="54573-108">类型</span><span class="sxs-lookup"><span data-stu-id="54573-108">Type</span></span>|<span data-ttu-id="54573-109">Description</span><span class="sxs-lookup"><span data-stu-id="54573-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54573-110">pageRanges</span><span class="sxs-lookup"><span data-stu-id="54573-110">pageRanges</span></span>|<span data-ttu-id="54573-111">[integerRange](integerrange.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54573-111">[integerRange](integerrange.md) collection</span></span>|<span data-ttu-id="54573-112">要打印的页面范围。</span><span class="sxs-lookup"><span data-stu-id="54573-112">The page ranges to print.</span></span> <span data-ttu-id="54573-113">只读。</span><span class="sxs-lookup"><span data-stu-id="54573-113">Read-only.</span></span>|
|<span data-ttu-id="54573-114">quality</span><span class="sxs-lookup"><span data-stu-id="54573-114">quality</span></span>|[<span data-ttu-id="54573-115">printQuality</span><span class="sxs-lookup"><span data-stu-id="54573-115">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="54573-116">打印作业时使用的打印质量。</span><span class="sxs-lookup"><span data-stu-id="54573-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="54573-117">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-117">Valid values are described in the table below.</span></span> <span data-ttu-id="54573-118">只读。</span><span class="sxs-lookup"><span data-stu-id="54573-118">Read-only.</span></span>|
|<span data-ttu-id="54573-119">dpi</span><span class="sxs-lookup"><span data-stu-id="54573-119">dpi</span></span>|<span data-ttu-id="54573-120">Int32</span><span class="sxs-lookup"><span data-stu-id="54573-120">Int32</span></span>|<span data-ttu-id="54573-121">打印作业时使用的分辨率，以每英寸点数表示 (DPI) 。</span><span class="sxs-lookup"><span data-stu-id="54573-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="54573-122">只读。</span><span class="sxs-lookup"><span data-stu-id="54573-122">Read-only.</span></span>|
|<span data-ttu-id="54573-123">feedOrientation</span><span class="sxs-lookup"><span data-stu-id="54573-123">feedOrientation</span></span>|<span data-ttu-id="54573-124">printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="54573-124">printerFeedOrientation</span></span>|<span data-ttu-id="54573-125">将媒体馈送到打印机时使用的方向。</span><span class="sxs-lookup"><span data-stu-id="54573-125">The orientation to use when feeding media into the printer.</span></span> <span data-ttu-id="54573-126">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-126">Valid values are described in the following table.</span></span> <span data-ttu-id="54573-127">只读。</span><span class="sxs-lookup"><span data-stu-id="54573-127">Read-only.</span></span>|
|<span data-ttu-id="54573-128">orientation</span><span class="sxs-lookup"><span data-stu-id="54573-128">orientation</span></span>|[<span data-ttu-id="54573-129">printOrientation</span><span class="sxs-lookup"><span data-stu-id="54573-129">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="54573-130">打印作业时打印机应该使用的方向设置。</span><span class="sxs-lookup"><span data-stu-id="54573-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="54573-131">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="54573-132">duplexMode</span><span class="sxs-lookup"><span data-stu-id="54573-132">duplexMode</span></span>|[<span data-ttu-id="54573-133">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="54573-133">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="54573-134">打印作业时打印机应该使用的双面模式。</span><span class="sxs-lookup"><span data-stu-id="54573-134">The duplex mode the printer should use when printing the job.</span></span> <span data-ttu-id="54573-135">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-135">Valid values are described in the table below.</span></span> <span data-ttu-id="54573-136">只读。</span><span class="sxs-lookup"><span data-stu-id="54573-136">Read-only.</span></span>|
|<span data-ttu-id="54573-137">copies</span><span class="sxs-lookup"><span data-stu-id="54573-137">copies</span></span>|<span data-ttu-id="54573-138">Int32</span><span class="sxs-lookup"><span data-stu-id="54573-138">Int32</span></span>|<span data-ttu-id="54573-139">应打印的副本数。</span><span class="sxs-lookup"><span data-stu-id="54573-139">The number of copies that should be printed.</span></span> <span data-ttu-id="54573-140">只读。</span><span class="sxs-lookup"><span data-stu-id="54573-140">Read-only.</span></span>|
|<span data-ttu-id="54573-141">colorMode</span><span class="sxs-lookup"><span data-stu-id="54573-141">colorMode</span></span>|[<span data-ttu-id="54573-142">printColorMode</span><span class="sxs-lookup"><span data-stu-id="54573-142">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="54573-143">打印机用于打印作业的颜色模式。</span><span class="sxs-lookup"><span data-stu-id="54573-143">The color mode the printer should use to print the job.</span></span> <span data-ttu-id="54573-144">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-144">Valid values are described in the table below.</span></span> <span data-ttu-id="54573-145">只读。</span><span class="sxs-lookup"><span data-stu-id="54573-145">Read-only.</span></span>|
|<span data-ttu-id="54573-146">inputBin</span><span class="sxs-lookup"><span data-stu-id="54573-146">inputBin</span></span>|<span data-ttu-id="54573-147">String</span><span class="sxs-lookup"><span data-stu-id="54573-147">String</span></span>|<span data-ttu-id="54573-148">打印时 (纸盒) 纸盒。</span><span class="sxs-lookup"><span data-stu-id="54573-148">The input bin (tray) to use when printing.</span></span> <span data-ttu-id="54573-149">有关受支持的 [输入箱](printercapabilities.md) 列表，请参阅打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="54573-149">See the printer's [capabilities](printercapabilities.md) for a list of supported input bins.</span></span>|
|<span data-ttu-id="54573-150">outputBin</span><span class="sxs-lookup"><span data-stu-id="54573-150">outputBin</span></span>|<span data-ttu-id="54573-151">String</span><span class="sxs-lookup"><span data-stu-id="54573-151">String</span></span>|<span data-ttu-id="54573-152">要放入已完成打印的输出箱。</span><span class="sxs-lookup"><span data-stu-id="54573-152">The output bin to place completed prints into.</span></span> <span data-ttu-id="54573-153">有关受支持的 [输出箱](printercapabilities.md) 的列表，请参阅打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="54573-153">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="54573-154">mediaSize</span><span class="sxs-lookup"><span data-stu-id="54573-154">mediaSize</span></span>|<span data-ttu-id="54573-155">String</span><span class="sxs-lookup"><span data-stu-id="54573-155">String</span></span>|<span data-ttu-id="54573-156">打印时使用的媒体大小。</span><span class="sxs-lookup"><span data-stu-id="54573-156">The media sizeto use when printing.</span></span> <span data-ttu-id="54573-157">支持 ISO 和 ANSI 媒体大小的标准大小名称，以及关联的打印机支持的任何自定义大小。</span><span class="sxs-lookup"><span data-stu-id="54573-157">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>|
|<span data-ttu-id="54573-158">margin</span><span class="sxs-lookup"><span data-stu-id="54573-158">margin</span></span>|[<span data-ttu-id="54573-159">printMargin</span><span class="sxs-lookup"><span data-stu-id="54573-159">printMargin</span></span>](printmargin.md)|<span data-ttu-id="54573-160">打印时使用的边距设置。</span><span class="sxs-lookup"><span data-stu-id="54573-160">The margin settings to use when printing.</span></span>|
|<span data-ttu-id="54573-161">mediaType</span><span class="sxs-lookup"><span data-stu-id="54573-161">mediaType</span></span>|<span data-ttu-id="54573-162">String</span><span class="sxs-lookup"><span data-stu-id="54573-162">String</span></span>|<span data-ttu-id="54573-163">默认媒体 (类型，例如) 打印文档的纸张类型。</span><span class="sxs-lookup"><span data-stu-id="54573-163">The default media (such as paper) type to print the document on.</span></span> <span data-ttu-id="54573-164">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-164">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="54573-165">finishings</span><span class="sxs-lookup"><span data-stu-id="54573-165">finishings</span></span>|<span data-ttu-id="54573-166">[printFinishing](enums.md#printfinishing-values) 集合</span><span class="sxs-lookup"><span data-stu-id="54573-166">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="54573-167">打印时使用的完成过程。</span><span class="sxs-lookup"><span data-stu-id="54573-167">Finishing processes to use when printing.</span></span>|
|<span data-ttu-id="54573-168">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="54573-168">pagesPerSheet</span></span>|<span data-ttu-id="54573-169">Int32</span><span class="sxs-lookup"><span data-stu-id="54573-169">Int32</span></span>|<span data-ttu-id="54573-170">要在每个工作表上打印的文档页数。</span><span class="sxs-lookup"><span data-stu-id="54573-170">The number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="54573-171">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="54573-171">multipageLayout</span></span>|[<span data-ttu-id="54573-172">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="54573-172">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="54573-173">每张工作表打印多个页面时页面的布局方向。</span><span class="sxs-lookup"><span data-stu-id="54573-173">The direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="54573-174">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-174">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="54573-175">collate</span><span class="sxs-lookup"><span data-stu-id="54573-175">collate</span></span>|<span data-ttu-id="54573-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="54573-176">Boolean</span></span>|<span data-ttu-id="54573-177">打印多页文档的多个副本时，打印机是否应该整理页面。</span><span class="sxs-lookup"><span data-stu-id="54573-177">Whether the printer should collate pages wehen printing multiple copies of a multi-page document.</span></span>|
|<span data-ttu-id="54573-178">scaling</span><span class="sxs-lookup"><span data-stu-id="54573-178">scaling</span></span>|[<span data-ttu-id="54573-179">printScaling</span><span class="sxs-lookup"><span data-stu-id="54573-179">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="54573-180">指定打印机如何缩放文档数据以适应请求的媒体。</span><span class="sxs-lookup"><span data-stu-id="54573-180">Specifies how the printer should scale the document data to fit the requested media.</span></span> <span data-ttu-id="54573-181">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="54573-181">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54573-182">关系</span><span class="sxs-lookup"><span data-stu-id="54573-182">Relationships</span></span>
<span data-ttu-id="54573-183">无。</span><span class="sxs-lookup"><span data-stu-id="54573-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54573-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54573-184">JSON representation</span></span>
<span data-ttu-id="54573-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54573-185">The following is a JSON representation of the resource.</span></span>
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

