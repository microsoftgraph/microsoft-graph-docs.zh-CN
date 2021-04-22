---
title: printerDefaults 资源类型
description: 表示打印机的默认设置。 检查打印机的功能以查看它支持的所有值。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 06566b30e2292d6552e5c0a79281693b97ab6350
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944240"
---
# <a name="printerdefaults-resource-type"></a><span data-ttu-id="de72d-104">printerDefaults 资源类型</span><span class="sxs-lookup"><span data-stu-id="de72d-104">printerDefaults resource type</span></span>

<span data-ttu-id="de72d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de72d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="de72d-106">表示打印机的默认设置。</span><span class="sxs-lookup"><span data-stu-id="de72d-106">Represents the printer's default settings.</span></span> <span data-ttu-id="de72d-107">检查打印机 [的功能以查看](printercapabilities.md) 它支持的所有值。</span><span class="sxs-lookup"><span data-stu-id="de72d-107">Check the printer's [capabilities](printercapabilities.md) to see all the values that it supports.</span></span>

## <a name="properties"></a><span data-ttu-id="de72d-108">属性</span><span class="sxs-lookup"><span data-stu-id="de72d-108">Properties</span></span>
|<span data-ttu-id="de72d-109">属性</span><span class="sxs-lookup"><span data-stu-id="de72d-109">Property</span></span>|<span data-ttu-id="de72d-110">类型</span><span class="sxs-lookup"><span data-stu-id="de72d-110">Type</span></span>|<span data-ttu-id="de72d-111">说明</span><span class="sxs-lookup"><span data-stu-id="de72d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de72d-112">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="de72d-112">copiesPerJob</span></span>|<span data-ttu-id="de72d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="de72d-113">Int32</span></span>|<span data-ttu-id="de72d-114">每个作业打印的默认副本数。</span><span class="sxs-lookup"><span data-stu-id="de72d-114">The default number of copies printed per job.</span></span>|
|<span data-ttu-id="de72d-115">contentType</span><span class="sxs-lookup"><span data-stu-id="de72d-115">contentType</span></span>|<span data-ttu-id="de72d-116">String</span><span class="sxs-lookup"><span data-stu-id="de72d-116">String</span></span>|<span data-ttu-id="de72d-117">MIME (类型) 处理文档时使用。</span><span class="sxs-lookup"><span data-stu-id="de72d-117">The default content (MIME) type to use when processing documents.</span></span>|
|<span data-ttu-id="de72d-118">finishings</span><span class="sxs-lookup"><span data-stu-id="de72d-118">finishings</span></span>|<span data-ttu-id="de72d-119">[printFinishing](enums.md#printfinishing-values) 集合</span><span class="sxs-lookup"><span data-stu-id="de72d-119">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="de72d-120">应用于打印作业的默认完成集。</span><span class="sxs-lookup"><span data-stu-id="de72d-120">The default set of finishings to apply to print jobs.</span></span> <span data-ttu-id="de72d-121">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-121">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="de72d-122">mediaColor</span><span class="sxs-lookup"><span data-stu-id="de72d-122">mediaColor</span></span>|<span data-ttu-id="de72d-123">String</span><span class="sxs-lookup"><span data-stu-id="de72d-123">String</span></span>|<span data-ttu-id="de72d-124">默认媒体 (，例如) 打印文档的纸张颜色。</span><span class="sxs-lookup"><span data-stu-id="de72d-124">The default media (such as paper) color to print the document on.</span></span>|
|<span data-ttu-id="de72d-125">mediaType</span><span class="sxs-lookup"><span data-stu-id="de72d-125">mediaType</span></span>|<span data-ttu-id="de72d-126">String</span><span class="sxs-lookup"><span data-stu-id="de72d-126">String</span></span>|<span data-ttu-id="de72d-127">默认媒体 (，如) 打印文档的类型。</span><span class="sxs-lookup"><span data-stu-id="de72d-127">The default media (such as paper) type to print the document on.</span></span>|
|<span data-ttu-id="de72d-128">mediaSize</span><span class="sxs-lookup"><span data-stu-id="de72d-128">mediaSize</span></span>|<span data-ttu-id="de72d-129">String</span><span class="sxs-lookup"><span data-stu-id="de72d-129">String</span></span>|<span data-ttu-id="de72d-130">使用的默认媒体大小。</span><span class="sxs-lookup"><span data-stu-id="de72d-130">The default media size to use.</span></span> <span data-ttu-id="de72d-131">支持 ISO 和 ANSI 媒体大小的标准大小名称。</span><span class="sxs-lookup"><span data-stu-id="de72d-131">Supports standard size names for ISO and ANSI media sizes.</span></span> <span data-ttu-id="de72d-132">[printerCapabilities](printercapabilities.md#mediasizes-values)主题中列出了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-132">Valid values are listed in the [printerCapabilities](printercapabilities.md#mediasizes-values) topic.</span></span>|
|<span data-ttu-id="de72d-133">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="de72d-133">pagesPerSheet</span></span>|<span data-ttu-id="de72d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="de72d-134">Int32</span></span>|<span data-ttu-id="de72d-135">每张工作表上要打印的默认文档页数。</span><span class="sxs-lookup"><span data-stu-id="de72d-135">The default number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="de72d-136">orientation</span><span class="sxs-lookup"><span data-stu-id="de72d-136">orientation</span></span>|[<span data-ttu-id="de72d-137">printOrientation</span><span class="sxs-lookup"><span data-stu-id="de72d-137">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="de72d-138">打印文档时使用的默认方向。</span><span class="sxs-lookup"><span data-stu-id="de72d-138">The default orientation to use when printing the document.</span></span> <span data-ttu-id="de72d-139">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-139">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="de72d-140">outputBin</span><span class="sxs-lookup"><span data-stu-id="de72d-140">outputBin</span></span>|<span data-ttu-id="de72d-141">String</span><span class="sxs-lookup"><span data-stu-id="de72d-141">String</span></span>|<span data-ttu-id="de72d-142">将已完成打印放入的默认输出箱。</span><span class="sxs-lookup"><span data-stu-id="de72d-142">The default output bin to place completed prints into.</span></span> <span data-ttu-id="de72d-143">有关受支持的 [输出箱](printercapabilities.md) 的列表，请参阅打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="de72d-143">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="de72d-144">fitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="de72d-144">fitPdfToPage</span></span>|<span data-ttu-id="de72d-145">布尔</span><span class="sxs-lookup"><span data-stu-id="de72d-145">Boolean</span></span>|<span data-ttu-id="de72d-146">默认 fitPdfToPage 设置。</span><span class="sxs-lookup"><span data-stu-id="de72d-146">The default fitPdfToPage setting.</span></span> <span data-ttu-id="de72d-147">如果为 True，将 PDF 文档的每一页都适合媒体的物理工作表;如果为 false，则打印机决定如何设置展示次数。</span><span class="sxs-lookup"><span data-stu-id="de72d-147">True to fit each page of a PDF document to a physical sheet of media; false to let the printer decide how to lay out impressions.</span></span>|
|<span data-ttu-id="de72d-148">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="de72d-148">multipageLayout</span></span>|[<span data-ttu-id="de72d-149">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="de72d-149">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="de72d-150">当每张工作表打印多个页面时，对页面进行布局的默认方向。</span><span class="sxs-lookup"><span data-stu-id="de72d-150">The default direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="de72d-151">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-151">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="de72d-152">colorMode</span><span class="sxs-lookup"><span data-stu-id="de72d-152">colorMode</span></span>|[<span data-ttu-id="de72d-153">printColorMode</span><span class="sxs-lookup"><span data-stu-id="de72d-153">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="de72d-154">打印文档时使用的默认颜色模式。</span><span class="sxs-lookup"><span data-stu-id="de72d-154">The default color mode to use when printing the document.</span></span> <span data-ttu-id="de72d-155">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-155">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="de72d-156">quality</span><span class="sxs-lookup"><span data-stu-id="de72d-156">quality</span></span>|[<span data-ttu-id="de72d-157">printQuality</span><span class="sxs-lookup"><span data-stu-id="de72d-157">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="de72d-158">打印文档时使用的默认质量。</span><span class="sxs-lookup"><span data-stu-id="de72d-158">The default quality to use when printing the document.</span></span> <span data-ttu-id="de72d-159">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-159">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="de72d-160">duplexMode</span><span class="sxs-lookup"><span data-stu-id="de72d-160">duplexMode</span></span>|[<span data-ttu-id="de72d-161">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="de72d-161">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="de72d-162">默认双面 (双面) 打印文档时使用的配置。</span><span class="sxs-lookup"><span data-stu-id="de72d-162">The default duplex (double-sided) configuration to use when printing a document.</span></span> <span data-ttu-id="de72d-163">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-163">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="de72d-164">dpi</span><span class="sxs-lookup"><span data-stu-id="de72d-164">dpi</span></span>|<span data-ttu-id="de72d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="de72d-165">Int32</span></span>|<span data-ttu-id="de72d-166">打印作业时使用的默认分辨率（以 DPI 表示）。</span><span class="sxs-lookup"><span data-stu-id="de72d-166">The default resolution in DPI to use when printing the job.</span></span>|
|<span data-ttu-id="de72d-167">scaling</span><span class="sxs-lookup"><span data-stu-id="de72d-167">scaling</span></span>|[<span data-ttu-id="de72d-168">printScaling</span><span class="sxs-lookup"><span data-stu-id="de72d-168">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="de72d-169">指定打印机如何缩放文档数据以适应请求的媒体。</span><span class="sxs-lookup"><span data-stu-id="de72d-169">Specifies how the printer scales the document data to fit the requested media.</span></span> <span data-ttu-id="de72d-170">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="de72d-170">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de72d-171">关系</span><span class="sxs-lookup"><span data-stu-id="de72d-171">Relationships</span></span>
<span data-ttu-id="de72d-172">无。</span><span class="sxs-lookup"><span data-stu-id="de72d-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de72d-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de72d-173">JSON representation</span></span>
<span data-ttu-id="de72d-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de72d-174">The following is a JSON representation of the resource.</span></span>
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

