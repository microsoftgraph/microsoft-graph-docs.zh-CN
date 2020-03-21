---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4fff364cced30e46d50bbef9ef5b8b50e4a058f5
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895606"
---
# <a name="printerstatus-resource-type"></a><span data-ttu-id="93fab-103">printerStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="93fab-103">printerStatus resource type</span></span>

<span data-ttu-id="93fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93fab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93fab-105">表示打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="93fab-105">Represents the processing status of the printer, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="93fab-106">属性</span><span class="sxs-lookup"><span data-stu-id="93fab-106">Properties</span></span>
| <span data-ttu-id="93fab-107">属性</span><span class="sxs-lookup"><span data-stu-id="93fab-107">Property</span></span>     | <span data-ttu-id="93fab-108">类型</span><span class="sxs-lookup"><span data-stu-id="93fab-108">Type</span></span>        | <span data-ttu-id="93fab-109">说明</span><span class="sxs-lookup"><span data-stu-id="93fab-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="93fab-110">processingState</span><span class="sxs-lookup"><span data-stu-id="93fab-110">processingState</span></span>|<span data-ttu-id="93fab-111">printerProcessingState</span><span class="sxs-lookup"><span data-stu-id="93fab-111">printerProcessingState</span></span>|<span data-ttu-id="93fab-112">当前的处理状态。</span><span class="sxs-lookup"><span data-stu-id="93fab-112">The current processing state.</span></span> <span data-ttu-id="93fab-113">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="93fab-113">Valid values are described in the following table.</span></span> <span data-ttu-id="93fab-114">只读。</span><span class="sxs-lookup"><span data-stu-id="93fab-114">Read-only.</span></span>|
|<span data-ttu-id="93fab-115">processingStateReasons</span><span class="sxs-lookup"><span data-stu-id="93fab-115">processingStateReasons</span></span>|<span data-ttu-id="93fab-116">printerProcessingStateReason 集合</span><span class="sxs-lookup"><span data-stu-id="93fab-116">printerProcessingStateReason collection</span></span>|<span data-ttu-id="93fab-117">描述打印机处于当前状态的原因的列表。</span><span class="sxs-lookup"><span data-stu-id="93fab-117">The list of reasons describing why the printer is in the current state.</span></span> <span data-ttu-id="93fab-118">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="93fab-118">Valid values are described in the following table.</span></span> <span data-ttu-id="93fab-119">只读。</span><span class="sxs-lookup"><span data-stu-id="93fab-119">Read-only.</span></span>|
|<span data-ttu-id="93fab-120">processingStateDescription</span><span class="sxs-lookup"><span data-stu-id="93fab-120">processingStateDescription</span></span>|<span data-ttu-id="93fab-121">String</span><span class="sxs-lookup"><span data-stu-id="93fab-121">String</span></span>|<span data-ttu-id="93fab-122">打印机当前处理状态的人可读说明。</span><span class="sxs-lookup"><span data-stu-id="93fab-122">A human-readable description of the printer's current processing state.</span></span> <span data-ttu-id="93fab-123">只读。</span><span class="sxs-lookup"><span data-stu-id="93fab-123">Read-only.</span></span>|

### <a name="printerprocessingstate-values"></a><span data-ttu-id="93fab-124">printerProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="93fab-124">printerProcessingState values</span></span>

|<span data-ttu-id="93fab-125">成员</span><span class="sxs-lookup"><span data-stu-id="93fab-125">Member</span></span>|<span data-ttu-id="93fab-126">值</span><span class="sxs-lookup"><span data-stu-id="93fab-126">Value</span></span>|<span data-ttu-id="93fab-127">说明</span><span class="sxs-lookup"><span data-stu-id="93fab-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93fab-128">unknown</span><span class="sxs-lookup"><span data-stu-id="93fab-128">unknown</span></span>|<span data-ttu-id="93fab-129">0</span><span class="sxs-lookup"><span data-stu-id="93fab-129">0</span></span>|<span data-ttu-id="93fab-130">打印机报告的处理状态未知。</span><span class="sxs-lookup"><span data-stu-id="93fab-130">The processing state reported by the printer is unknown.</span></span>|
|<span data-ttu-id="93fab-131">待机</span><span class="sxs-lookup"><span data-stu-id="93fab-131">idle</span></span>|<span data-ttu-id="93fab-132">1</span><span class="sxs-lookup"><span data-stu-id="93fab-132">1</span></span>|<span data-ttu-id="93fab-133">打印机处于空闲状态，并已准备好接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="93fab-133">The printer is idle and ready to accept new print jobs.</span></span>|
|<span data-ttu-id="93fab-134">处理</span><span class="sxs-lookup"><span data-stu-id="93fab-134">processing</span></span>|<span data-ttu-id="93fab-135">双面</span><span class="sxs-lookup"><span data-stu-id="93fab-135">2</span></span>|<span data-ttu-id="93fab-136">打印机当前正在处理打印作业，并将在完成时处理任何挂起的作业。</span><span class="sxs-lookup"><span data-stu-id="93fab-136">The printer is currently processing a print job and will process any pending jobs upon completion.</span></span>|
|<span data-ttu-id="93fab-137">停止</span><span class="sxs-lookup"><span data-stu-id="93fab-137">stopped</span></span>|<span data-ttu-id="93fab-138">第三章</span><span class="sxs-lookup"><span data-stu-id="93fab-138">3</span></span>|<span data-ttu-id="93fab-139">打印机遇到问题（例如，在当前送纸器中缺纸），无法继续使用当前的打印作业，直到问题得到解决。</span><span class="sxs-lookup"><span data-stu-id="93fab-139">The printer encountered an issue (for example, ran out of paper in the active tray) and cannot continue the current print job until the issue is addressed.</span></span> <span data-ttu-id="93fab-140">有关详细信息，请参阅**printerProcessingStateReasons**值或**printerProcessingStateDescription**值。</span><span class="sxs-lookup"><span data-stu-id="93fab-140">See the **printerProcessingStateReasons** value(s) or the **printerProcessingStateDescription** value for more information.</span></span>|
|<span data-ttu-id="93fab-141">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="93fab-141">unknownFutureValue</span></span>|<span data-ttu-id="93fab-142">4 </span><span class="sxs-lookup"><span data-stu-id="93fab-142">4</span></span>|<span data-ttu-id="93fab-143">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="93fab-143">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="93fab-144">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="93fab-144">Do not use.</span></span>|

### <a name="printerprocessingstatereason-values"></a><span data-ttu-id="93fab-145">printerProcessingStateReason 值</span><span class="sxs-lookup"><span data-stu-id="93fab-145">printerProcessingStateReason values</span></span>

|<span data-ttu-id="93fab-146">成员</span><span class="sxs-lookup"><span data-stu-id="93fab-146">Member</span></span>|<span data-ttu-id="93fab-147">值</span><span class="sxs-lookup"><span data-stu-id="93fab-147">Value</span></span>|<span data-ttu-id="93fab-148">说明</span><span class="sxs-lookup"><span data-stu-id="93fab-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93fab-149">停留</span><span class="sxs-lookup"><span data-stu-id="93fab-149">paused</span></span>|<span data-ttu-id="93fab-150">0</span><span class="sxs-lookup"><span data-stu-id="93fab-150">0</span></span>| <span data-ttu-id="93fab-151">正在进行的打印作业已暂停。</span><span class="sxs-lookup"><span data-stu-id="93fab-151">An ongoing print job was paused.</span></span>|
|<span data-ttu-id="93fab-152">被</span><span class="sxs-lookup"><span data-stu-id="93fab-152">disconnected</span></span>|<span data-ttu-id="93fab-153">1</span><span class="sxs-lookup"><span data-stu-id="93fab-153">1</span></span>|<span data-ttu-id="93fab-154">与打印机的连接丢失或无法建立连接。</span><span class="sxs-lookup"><span data-stu-id="93fab-154">The connection to the printer was lost or cannot be established.</span></span>|
|<span data-ttu-id="93fab-155">mediaJam</span><span class="sxs-lookup"><span data-stu-id="93fab-155">mediaJam</span></span>|<span data-ttu-id="93fab-156">双面</span><span class="sxs-lookup"><span data-stu-id="93fab-156">2</span></span>|<span data-ttu-id="93fab-157">一个或多个纸盒中的介质卡纸。</span><span class="sxs-lookup"><span data-stu-id="93fab-157">Media in one or more trays is jammed.</span></span>|
|<span data-ttu-id="93fab-158">mediaNeeded</span><span class="sxs-lookup"><span data-stu-id="93fab-158">mediaNeeded</span></span>|<span data-ttu-id="93fab-159">第三章</span><span class="sxs-lookup"><span data-stu-id="93fab-159">3</span></span>|<span data-ttu-id="93fab-160">必须先替换当前使用的输入送纸器中的媒体，然后才能继续执行作业。</span><span class="sxs-lookup"><span data-stu-id="93fab-160">Media in the currently-used input tray needs to be replaced before the job can continue.</span></span>|
|<span data-ttu-id="93fab-161">mediaLow</span><span class="sxs-lookup"><span data-stu-id="93fab-161">mediaLow</span></span>|<span data-ttu-id="93fab-162">4 </span><span class="sxs-lookup"><span data-stu-id="93fab-162">4</span></span>|<span data-ttu-id="93fab-163">一个或多个送纸器中的媒体几乎耗尽。</span><span class="sxs-lookup"><span data-stu-id="93fab-163">Media in one or more trays is almost exhausted.</span></span>|
|<span data-ttu-id="93fab-164">mediaEmpty</span><span class="sxs-lookup"><span data-stu-id="93fab-164">mediaEmpty</span></span>|<span data-ttu-id="93fab-165">5 </span><span class="sxs-lookup"><span data-stu-id="93fab-165">5</span></span>|<span data-ttu-id="93fab-166">一个或多个托盘中的媒体已耗尽。</span><span class="sxs-lookup"><span data-stu-id="93fab-166">Media in one or more trays is exhausted.</span></span>|
|<span data-ttu-id="93fab-167">coverOpen</span><span class="sxs-lookup"><span data-stu-id="93fab-167">coverOpen</span></span>|<span data-ttu-id="93fab-168">6 </span><span class="sxs-lookup"><span data-stu-id="93fab-168">6</span></span>|<span data-ttu-id="93fab-169">打开了一个或多个封面。</span><span class="sxs-lookup"><span data-stu-id="93fab-169">One or more covers are open.</span></span>|
|<span data-ttu-id="93fab-170">interlockOpen</span><span class="sxs-lookup"><span data-stu-id="93fab-170">interlockOpen</span></span>|<span data-ttu-id="93fab-171">7 </span><span class="sxs-lookup"><span data-stu-id="93fab-171">7</span></span>|<span data-ttu-id="93fab-172">一个或多个互锁设备已打开。</span><span class="sxs-lookup"><span data-stu-id="93fab-172">One or more interlock devices are open.</span></span>|
|<span data-ttu-id="93fab-173">queueFull</span><span class="sxs-lookup"><span data-stu-id="93fab-173">queueFull</span></span>|<span data-ttu-id="93fab-174">8 </span><span class="sxs-lookup"><span data-stu-id="93fab-174">8</span></span>|<span data-ttu-id="93fab-175">打印机的后台打印程序队列已满，无法排队新的作业。</span><span class="sxs-lookup"><span data-stu-id="93fab-175">The printer's spooler queue is full and new jobs cannot be queued.</span></span>|
|<span data-ttu-id="93fab-176">outputTrayMissing</span><span class="sxs-lookup"><span data-stu-id="93fab-176">outputTrayMissing</span></span>|<span data-ttu-id="93fab-177">9 </span><span class="sxs-lookup"><span data-stu-id="93fab-177">9</span></span>|<span data-ttu-id="93fab-178">一个或多个输出送纸器丢失。</span><span class="sxs-lookup"><span data-stu-id="93fab-178">One or more output trays are missing.</span></span>|
|<span data-ttu-id="93fab-179">outputAreaFull</span><span class="sxs-lookup"><span data-stu-id="93fab-179">outputAreaFull</span></span>|<span data-ttu-id="93fab-180">10 </span><span class="sxs-lookup"><span data-stu-id="93fab-180">10</span></span>|<span data-ttu-id="93fab-181">一个或多个输出托盘已满，无法接受更多的媒体。</span><span class="sxs-lookup"><span data-stu-id="93fab-181">One or more output trays are full and cannot accept more media.</span></span>|
|<span data-ttu-id="93fab-182">markerSupplyLow</span><span class="sxs-lookup"><span data-stu-id="93fab-182">markerSupplyLow</span></span>|<span data-ttu-id="93fab-183">11x17</span><span class="sxs-lookup"><span data-stu-id="93fab-183">11</span></span>|<span data-ttu-id="93fab-184">一个或多个标记源（例如，墨迹、墨粉或功能区）不足。</span><span class="sxs-lookup"><span data-stu-id="93fab-184">One or more marker sources (for example, ink, toner or ribbon) are low.</span></span>|
|<span data-ttu-id="93fab-185">markerSupplyEmpty</span><span class="sxs-lookup"><span data-stu-id="93fab-185">markerSupplyEmpty</span></span>|<span data-ttu-id="93fab-186">12 </span><span class="sxs-lookup"><span data-stu-id="93fab-186">12</span></span>|<span data-ttu-id="93fab-187">一个或多个标记源（例如，墨迹、墨粉或功能区）已耗尽。</span><span class="sxs-lookup"><span data-stu-id="93fab-187">One or more marker sources (for example, ink, toner or ribbon) are exhausted.</span></span>|
|<span data-ttu-id="93fab-188">inputTrayMissing</span><span class="sxs-lookup"><span data-stu-id="93fab-188">inputTrayMissing</span></span>|<span data-ttu-id="93fab-189">13 </span><span class="sxs-lookup"><span data-stu-id="93fab-189">13</span></span>|<span data-ttu-id="93fab-190">一个或多个输入送纸器不在设备中。</span><span class="sxs-lookup"><span data-stu-id="93fab-190">One or more input trays are not in the device.</span></span>|
|<span data-ttu-id="93fab-191">outputAlmostFull</span><span class="sxs-lookup"><span data-stu-id="93fab-191">outputAlmostFull</span></span>|<span data-ttu-id="93fab-192">14 </span><span class="sxs-lookup"><span data-stu-id="93fab-192">14</span></span>|<span data-ttu-id="93fab-193">一个或多个输出区域几乎已满（例如，送纸器、堆栈器、排序程序）。</span><span class="sxs-lookup"><span data-stu-id="93fab-193">One or more output area is almost full (for example, tray, stacker, collator).</span></span>|
|<span data-ttu-id="93fab-194">markerWasteAlmostFull</span><span class="sxs-lookup"><span data-stu-id="93fab-194">markerWasteAlmostFull</span></span>|<span data-ttu-id="93fab-195">15 </span><span class="sxs-lookup"><span data-stu-id="93fab-195">15</span></span>|<span data-ttu-id="93fab-196">设备标记供应废物容器几乎已满。</span><span class="sxs-lookup"><span data-stu-id="93fab-196">The device marker supply waste receptacle is almost full.</span></span>|
|<span data-ttu-id="93fab-197">markerWasteFull</span><span class="sxs-lookup"><span data-stu-id="93fab-197">markerWasteFull</span></span>|<span data-ttu-id="93fab-198">16 </span><span class="sxs-lookup"><span data-stu-id="93fab-198">16</span></span>|<span data-ttu-id="93fab-199">设备标记供应废物容器已满。</span><span class="sxs-lookup"><span data-stu-id="93fab-199">The device marker supply waste receptacle is full.</span></span>|
|<span data-ttu-id="93fab-200">fuserOverTemp</span><span class="sxs-lookup"><span data-stu-id="93fab-200">fuserOverTemp</span></span>|<span data-ttu-id="93fab-201">17 </span><span class="sxs-lookup"><span data-stu-id="93fab-201">17</span></span>|<span data-ttu-id="93fab-202">热熔器温度高于正常水平。</span><span class="sxs-lookup"><span data-stu-id="93fab-202">The fuser temperature is above normal.</span></span>|
|<span data-ttu-id="93fab-203">fuserUnderTemp</span><span class="sxs-lookup"><span data-stu-id="93fab-203">fuserUnderTemp</span></span>|<span data-ttu-id="93fab-204">18 </span><span class="sxs-lookup"><span data-stu-id="93fab-204">18</span></span>|<span data-ttu-id="93fab-205">热熔器温度低于正常水平。</span><span class="sxs-lookup"><span data-stu-id="93fab-205">The fuser temperature is below normal.</span></span>|
|<span data-ttu-id="93fab-206">相互</span><span class="sxs-lookup"><span data-stu-id="93fab-206">other</span></span>|<span data-ttu-id="93fab-207">合</span><span class="sxs-lookup"><span data-stu-id="93fab-207">19</span></span>|<span data-ttu-id="93fab-208">不属于其余原因的任何其他原因。</span><span class="sxs-lookup"><span data-stu-id="93fab-208">Any other reason that does not fall in rest of the reasons.</span></span>|
|<span data-ttu-id="93fab-209">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="93fab-209">unknownFutureValue</span></span>|<span data-ttu-id="93fab-210">20</span><span class="sxs-lookup"><span data-stu-id="93fab-210">20</span></span>|<span data-ttu-id="93fab-211">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="93fab-211">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="93fab-212">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="93fab-212">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93fab-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93fab-213">JSON representation</span></span>

<span data-ttu-id="93fab-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93fab-214">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerStatus"
}-->

```json
{
    "processingState": "String",
    "processingStateReasons": ["String"],
    "processingStateDescription": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->