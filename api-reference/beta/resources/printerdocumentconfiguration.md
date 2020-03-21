---
title: printerDocumentConfiguration 资源类型
description: 打印机打印文档时应使用的一组设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ff1da92894f8854bcdee2ce24d7a9d5cef6288e7
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895610"
---
# <a name="printerdocumentconfiguration-resource-type"></a><span data-ttu-id="ac656-103">printerDocumentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac656-103">printerDocumentConfiguration resource type</span></span>

<span data-ttu-id="ac656-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac656-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac656-105">打印机打印文档时应使用的一组设置。</span><span class="sxs-lookup"><span data-stu-id="ac656-105">A group of settings that a printer should use to print a document.</span></span>

## <a name="properties"></a><span data-ttu-id="ac656-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac656-106">Properties</span></span>
| <span data-ttu-id="ac656-107">属性</span><span class="sxs-lookup"><span data-stu-id="ac656-107">Property</span></span>     | <span data-ttu-id="ac656-108">类型</span><span class="sxs-lookup"><span data-stu-id="ac656-108">Type</span></span>        | <span data-ttu-id="ac656-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac656-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac656-110">pageRanges</span><span class="sxs-lookup"><span data-stu-id="ac656-110">pageRanges</span></span>|<span data-ttu-id="ac656-111">[printPageRange](printpagerange.md)集合</span><span class="sxs-lookup"><span data-stu-id="ac656-111">[printPageRange](printpagerange.md) collection</span></span>|<span data-ttu-id="ac656-112">要打印的页面范围。</span><span class="sxs-lookup"><span data-stu-id="ac656-112">The page ranges to print.</span></span> <span data-ttu-id="ac656-113">只读。</span><span class="sxs-lookup"><span data-stu-id="ac656-113">Read-only.</span></span>|
|<span data-ttu-id="ac656-114">printQuality</span><span class="sxs-lookup"><span data-stu-id="ac656-114">printQuality</span></span>|<span data-ttu-id="ac656-115">printQuality</span><span class="sxs-lookup"><span data-stu-id="ac656-115">printQuality</span></span>|<span data-ttu-id="ac656-116">打印作业时使用的打印质量。</span><span class="sxs-lookup"><span data-stu-id="ac656-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="ac656-117">有效值如下表所示。</span><span class="sxs-lookup"><span data-stu-id="ac656-117">Valid values are described in the table below.</span></span> <span data-ttu-id="ac656-118">只读。</span><span class="sxs-lookup"><span data-stu-id="ac656-118">Read-only.</span></span>|
|<span data-ttu-id="ac656-119">printResolutionInDpi</span><span class="sxs-lookup"><span data-stu-id="ac656-119">printResolutionInDpi</span></span>|<span data-ttu-id="ac656-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ac656-120">Int32</span></span>|<span data-ttu-id="ac656-121">打印作业时要使用的分辨率，以每英寸点数（DPI）表示。</span><span class="sxs-lookup"><span data-stu-id="ac656-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="ac656-122">只读。</span><span class="sxs-lookup"><span data-stu-id="ac656-122">Read-only.</span></span>|
|<span data-ttu-id="ac656-123">feedDirection</span><span class="sxs-lookup"><span data-stu-id="ac656-123">feedDirection</span></span>|<span data-ttu-id="ac656-124">printerFeedDirection</span><span class="sxs-lookup"><span data-stu-id="ac656-124">printerFeedDirection</span></span>|<span data-ttu-id="ac656-125">将媒体送进打印机时使用的方向。</span><span class="sxs-lookup"><span data-stu-id="ac656-125">The direction to use when feeding media into the printer.</span></span> <span data-ttu-id="ac656-126">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="ac656-126">Valid values are described in the following table.</span></span> <span data-ttu-id="ac656-127">只读。</span><span class="sxs-lookup"><span data-stu-id="ac656-127">Read-only.</span></span>|
|<span data-ttu-id="ac656-128">orientation</span><span class="sxs-lookup"><span data-stu-id="ac656-128">orientation</span></span>|<span data-ttu-id="ac656-129">printOrientation</span><span class="sxs-lookup"><span data-stu-id="ac656-129">printOrientation</span></span>|<span data-ttu-id="ac656-130">打印机打印作业时应使用的方向设置。</span><span class="sxs-lookup"><span data-stu-id="ac656-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="ac656-131">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="ac656-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="ac656-132">duplexConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac656-132">duplexConfiguration</span></span>|<span data-ttu-id="ac656-133">printDuplexConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac656-133">printDuplexConfiguration</span></span>|<span data-ttu-id="ac656-134">打印作业时打印机应使用的双工配置。</span><span class="sxs-lookup"><span data-stu-id="ac656-134">The duplex configuration the printer should use when printing the job.</span></span> <span data-ttu-id="ac656-135">有效值如下表所示。</span><span class="sxs-lookup"><span data-stu-id="ac656-135">Valid values are described in the table below.</span></span> <span data-ttu-id="ac656-136">只读。</span><span class="sxs-lookup"><span data-stu-id="ac656-136">Read-only.</span></span>|
|<span data-ttu-id="ac656-137">副本</span><span class="sxs-lookup"><span data-stu-id="ac656-137">copies</span></span>|<span data-ttu-id="ac656-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ac656-138">Int32</span></span>|<span data-ttu-id="ac656-139">应打印的份数。</span><span class="sxs-lookup"><span data-stu-id="ac656-139">The number of copies that should be printed.</span></span> <span data-ttu-id="ac656-140">只读。</span><span class="sxs-lookup"><span data-stu-id="ac656-140">Read-only.</span></span>|
|<span data-ttu-id="ac656-141">colorConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac656-141">colorConfiguration</span></span>|<span data-ttu-id="ac656-142">printColorConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac656-142">printColorConfiguration</span></span>|<span data-ttu-id="ac656-143">打印机打印作业时应使用的颜色配置。</span><span class="sxs-lookup"><span data-stu-id="ac656-143">The color configuration the printer should use to print the job.</span></span> <span data-ttu-id="ac656-144">有效值如下表所示。</span><span class="sxs-lookup"><span data-stu-id="ac656-144">Valid values are described in the table below.</span></span> <span data-ttu-id="ac656-145">只读。</span><span class="sxs-lookup"><span data-stu-id="ac656-145">Read-only.</span></span>|

### <a name="printduplexconfiguration-values"></a><span data-ttu-id="ac656-146">printDuplexConfiguration 值</span><span class="sxs-lookup"><span data-stu-id="ac656-146">printDuplexConfiguration values</span></span>

|<span data-ttu-id="ac656-147">成员</span><span class="sxs-lookup"><span data-stu-id="ac656-147">Member</span></span>|<span data-ttu-id="ac656-148">值</span><span class="sxs-lookup"><span data-stu-id="ac656-148">Value</span></span>|<span data-ttu-id="ac656-149">说明</span><span class="sxs-lookup"><span data-stu-id="ac656-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac656-150">twoSidedLongEdge</span><span class="sxs-lookup"><span data-stu-id="ac656-150">twoSidedLongEdge</span></span>|<span data-ttu-id="ac656-151">0</span><span class="sxs-lookup"><span data-stu-id="ac656-151">0</span></span>|<span data-ttu-id="ac656-152">打印机将双面打印，并且将沿长边翻转文档。</span><span class="sxs-lookup"><span data-stu-id="ac656-152">The printer will print double-sided, and will flip documents along the long edge.</span></span>|
|<span data-ttu-id="ac656-153">twoSidedShortEdge</span><span class="sxs-lookup"><span data-stu-id="ac656-153">twoSidedShortEdge</span></span>|<span data-ttu-id="ac656-154">1</span><span class="sxs-lookup"><span data-stu-id="ac656-154">1</span></span>|<span data-ttu-id="ac656-155">打印机将双面打印，并且将沿短边翻转文档。</span><span class="sxs-lookup"><span data-stu-id="ac656-155">The printer will print double-sided, and will flip documents along the short edge.</span></span>|
|<span data-ttu-id="ac656-156">oneSided</span><span class="sxs-lookup"><span data-stu-id="ac656-156">oneSided</span></span>|<span data-ttu-id="ac656-157">双面</span><span class="sxs-lookup"><span data-stu-id="ac656-157">2</span></span>|<span data-ttu-id="ac656-158">打印机将单面打印。</span><span class="sxs-lookup"><span data-stu-id="ac656-158">The printer will print single-sided.</span></span>|

### <a name="printquality-values"></a><span data-ttu-id="ac656-159">printQuality 值</span><span class="sxs-lookup"><span data-stu-id="ac656-159">printQuality values</span></span>

|<span data-ttu-id="ac656-160">成员</span><span class="sxs-lookup"><span data-stu-id="ac656-160">Member</span></span>|<span data-ttu-id="ac656-161">说明</span><span class="sxs-lookup"><span data-stu-id="ac656-161">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac656-162">降低</span><span class="sxs-lookup"><span data-stu-id="ac656-162">low</span></span>|<span data-ttu-id="ac656-163">打印机将使用低（通常称为 "草稿"）质量打印作业。</span><span class="sxs-lookup"><span data-stu-id="ac656-163">The printer will print the job using low (commonly known as "draft") quality.</span></span>|
|<span data-ttu-id="ac656-164">中等</span><span class="sxs-lookup"><span data-stu-id="ac656-164">medium</span></span>|<span data-ttu-id="ac656-165">打印机将使用 medim （通常称为 "普通"）质量打印作业。</span><span class="sxs-lookup"><span data-stu-id="ac656-165">The printer will print the job using medim (commonly known as "normal") quality.</span></span>|
|<span data-ttu-id="ac656-166">高效</span><span class="sxs-lookup"><span data-stu-id="ac656-166">high</span></span>|<span data-ttu-id="ac656-167">打印机将使用 "高" （通常称为 "最佳" 或 "精细"）质量打印作业。</span><span class="sxs-lookup"><span data-stu-id="ac656-167">The printer will print the job using high (commonly known as "best" or "fine") quality.</span></span>|

## <a name="printerfeeddirection-values"></a><span data-ttu-id="ac656-168">printerFeedDirection 值</span><span class="sxs-lookup"><span data-stu-id="ac656-168">printerFeedDirection values</span></span>

|<span data-ttu-id="ac656-169">成员</span><span class="sxs-lookup"><span data-stu-id="ac656-169">Member</span></span>|<span data-ttu-id="ac656-170">说明</span><span class="sxs-lookup"><span data-stu-id="ac656-170">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac656-171">longEdgeFirst</span><span class="sxs-lookup"><span data-stu-id="ac656-171">longEdgeFirst</span></span>|<span data-ttu-id="ac656-172">打印机将使用 "横向" 方向的活动栏中的工作表，并在工作表的长边先进行处理。</span><span class="sxs-lookup"><span data-stu-id="ac656-172">The printer will consume sheets from the active tray in "landscape" orientation, with the long edge of the sheet first.</span></span>|
|<span data-ttu-id="ac656-173">shortEdgeFirst</span><span class="sxs-lookup"><span data-stu-id="ac656-173">shortEdgeFirst</span></span>|<span data-ttu-id="ac656-174">打印机将使用 "纵向" 方向的活动托盘中的工作表，并在工作表中先短边。</span><span class="sxs-lookup"><span data-stu-id="ac656-174">The printer will consume sheets from the active tray in "portrait" orientation, with the short edge of the sheet first.</span></span>|

## <a name="printorientation-values"></a><span data-ttu-id="ac656-175">printOrientation 值</span><span class="sxs-lookup"><span data-stu-id="ac656-175">printOrientation values</span></span>

|<span data-ttu-id="ac656-176">成员</span><span class="sxs-lookup"><span data-stu-id="ac656-176">Member</span></span>|<span data-ttu-id="ac656-177">值</span><span class="sxs-lookup"><span data-stu-id="ac656-177">Value</span></span>|<span data-ttu-id="ac656-178">说明</span><span class="sxs-lookup"><span data-stu-id="ac656-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac656-179">纵</span><span class="sxs-lookup"><span data-stu-id="ac656-179">portrait</span></span>|<span data-ttu-id="ac656-180">第三章</span><span class="sxs-lookup"><span data-stu-id="ac656-180">3</span></span>|<span data-ttu-id="ac656-181">打印机将在 "纵向" 方向上打印为印记。</span><span class="sxs-lookup"><span data-stu-id="ac656-181">The printer will print impressions in the "portrait" orientation.</span></span>|
|<span data-ttu-id="ac656-182">现状</span><span class="sxs-lookup"><span data-stu-id="ac656-182">landscape</span></span>|<span data-ttu-id="ac656-183">4 </span><span class="sxs-lookup"><span data-stu-id="ac656-183">4</span></span>|<span data-ttu-id="ac656-184">打印机将在 "横向" 方向上打印为印记。</span><span class="sxs-lookup"><span data-stu-id="ac656-184">The printer will print impressions in the "landscape" orientation.</span></span>|
|<span data-ttu-id="ac656-185">reverseLandscape</span><span class="sxs-lookup"><span data-stu-id="ac656-185">reverseLandscape</span></span>|<span data-ttu-id="ac656-186">5 </span><span class="sxs-lookup"><span data-stu-id="ac656-186">5</span></span>|<span data-ttu-id="ac656-187">打印机将在 "翻转横向" 方向上打印为印记。</span><span class="sxs-lookup"><span data-stu-id="ac656-187">The printer will print impressions in the "reverse landscape" orientation.</span></span>|
|<span data-ttu-id="ac656-188">reversePortrait</span><span class="sxs-lookup"><span data-stu-id="ac656-188">reversePortrait</span></span>|<span data-ttu-id="ac656-189">6 </span><span class="sxs-lookup"><span data-stu-id="ac656-189">6</span></span>|<span data-ttu-id="ac656-190">打印机将在 "反转纵向" 方向上打印为印记。</span><span class="sxs-lookup"><span data-stu-id="ac656-190">The printer will print impressions in the "reverse portrait" orientation.</span></span>|

### <a name="printcolorconfiguration-values"></a><span data-ttu-id="ac656-191">printColorConfiguration 值</span><span class="sxs-lookup"><span data-stu-id="ac656-191">printColorConfiguration values</span></span>

|<span data-ttu-id="ac656-192">成员</span><span class="sxs-lookup"><span data-stu-id="ac656-192">Member</span></span>|<span data-ttu-id="ac656-193">值</span><span class="sxs-lookup"><span data-stu-id="ac656-193">Value</span></span>|<span data-ttu-id="ac656-194">说明</span><span class="sxs-lookup"><span data-stu-id="ac656-194">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac656-195">blackAndWhite</span><span class="sxs-lookup"><span data-stu-id="ac656-195">blackAndWhite</span></span>|<span data-ttu-id="ac656-196">0</span><span class="sxs-lookup"><span data-stu-id="ac656-196">0</span></span>|<span data-ttu-id="ac656-197">黑色和白色（仅使用黑色标记材料。）</span><span class="sxs-lookup"><span data-stu-id="ac656-197">Black and white (use black marker material only.)</span></span>|
|<span data-ttu-id="ac656-198">灰度</span><span class="sxs-lookup"><span data-stu-id="ac656-198">grayscale</span></span>|<span data-ttu-id="ac656-199">1</span><span class="sxs-lookup"><span data-stu-id="ac656-199">1</span></span>|<span data-ttu-id="ac656-200">灰度（可能使用某些颜色标记材料。）</span><span class="sxs-lookup"><span data-stu-id="ac656-200">Grayscale (may use some color marker material.)</span></span>|
|<span data-ttu-id="ac656-201">color</span><span class="sxs-lookup"><span data-stu-id="ac656-201">color</span></span>|<span data-ttu-id="ac656-202">双面</span><span class="sxs-lookup"><span data-stu-id="ac656-202">2</span></span>|<span data-ttu-id="ac656-203">颜色（使用标记材料的任意组合来创建颜色印象）。</span><span class="sxs-lookup"><span data-stu-id="ac656-203">Color (use any combination of marker materials to create a color impression).</span></span>|
|<span data-ttu-id="ac656-204">自动</span><span class="sxs-lookup"><span data-stu-id="ac656-204">auto</span></span>|<span data-ttu-id="ac656-205">第三章</span><span class="sxs-lookup"><span data-stu-id="ac656-205">3</span></span>|<span data-ttu-id="ac656-206">让打印机决定要使用哪种颜色模式。</span><span class="sxs-lookup"><span data-stu-id="ac656-206">Let the printer decide which color mode to use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac656-207">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac656-207">JSON representation</span></span>

<span data-ttu-id="ac656-208">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac656-208">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerDocumentConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.printPageRange"}],
  "printQuality": "String",
  "printResolutionInDpi": 123456,
  "feedDirection": "String",
  "orientation": "String",
  "duplexConfiguration": "String",
  "copies": 123456,
  "colorConfiguration": "String",
}

```
