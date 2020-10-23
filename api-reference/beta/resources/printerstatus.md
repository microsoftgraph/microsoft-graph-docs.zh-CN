---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c6e6f756c91af14d4a5c17dbf873e52fb1d553b7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726288"
---
# <a name="printerstatus-resource-type"></a><span data-ttu-id="18e9a-103">printerStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="18e9a-103">printerStatus resource type</span></span>

<span data-ttu-id="18e9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18e9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e9a-105">表示打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="18e9a-105">Represents the processing status of the printer, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="18e9a-106">属性</span><span class="sxs-lookup"><span data-stu-id="18e9a-106">Properties</span></span>
| <span data-ttu-id="18e9a-107">属性</span><span class="sxs-lookup"><span data-stu-id="18e9a-107">Property</span></span>     | <span data-ttu-id="18e9a-108">类型</span><span class="sxs-lookup"><span data-stu-id="18e9a-108">Type</span></span>        | <span data-ttu-id="18e9a-109">说明</span><span class="sxs-lookup"><span data-stu-id="18e9a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="18e9a-110">state</span><span class="sxs-lookup"><span data-stu-id="18e9a-110">state</span></span>|<span data-ttu-id="18e9a-111">printerProcessingState</span><span class="sxs-lookup"><span data-stu-id="18e9a-111">printerProcessingState</span></span>|<span data-ttu-id="18e9a-112">当前的处理状态。</span><span class="sxs-lookup"><span data-stu-id="18e9a-112">The current processing state.</span></span> <span data-ttu-id="18e9a-113">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="18e9a-113">Valid values are described in the following table.</span></span> <span data-ttu-id="18e9a-114">只读。</span><span class="sxs-lookup"><span data-stu-id="18e9a-114">Read-only.</span></span>|
|<span data-ttu-id="18e9a-115">详细信息</span><span class="sxs-lookup"><span data-stu-id="18e9a-115">details</span></span>|<span data-ttu-id="18e9a-116">printerProcessingStateDetail 集合</span><span class="sxs-lookup"><span data-stu-id="18e9a-116">printerProcessingStateDetail collection</span></span>|<span data-ttu-id="18e9a-117">描述打印机处于当前状态的原因的详细信息列表。</span><span class="sxs-lookup"><span data-stu-id="18e9a-117">The list of details describing why the printer is in the current state.</span></span> <span data-ttu-id="18e9a-118">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="18e9a-118">Valid values are described in the following table.</span></span> <span data-ttu-id="18e9a-119">只读。</span><span class="sxs-lookup"><span data-stu-id="18e9a-119">Read-only.</span></span>|
|<span data-ttu-id="18e9a-120">说明</span><span class="sxs-lookup"><span data-stu-id="18e9a-120">description</span></span>|<span data-ttu-id="18e9a-121">String</span><span class="sxs-lookup"><span data-stu-id="18e9a-121">String</span></span>|<span data-ttu-id="18e9a-122">打印机当前处理状态的人可读说明。</span><span class="sxs-lookup"><span data-stu-id="18e9a-122">A human-readable description of the printer's current processing state.</span></span> <span data-ttu-id="18e9a-123">只读。</span><span class="sxs-lookup"><span data-stu-id="18e9a-123">Read-only.</span></span>|

### <a name="printerprocessingstate-values"></a><span data-ttu-id="18e9a-124">printerProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="18e9a-124">printerProcessingState values</span></span>

|<span data-ttu-id="18e9a-125">成员</span><span class="sxs-lookup"><span data-stu-id="18e9a-125">Member</span></span>|<span data-ttu-id="18e9a-126">值</span><span class="sxs-lookup"><span data-stu-id="18e9a-126">Value</span></span>|<span data-ttu-id="18e9a-127">说明</span><span class="sxs-lookup"><span data-stu-id="18e9a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e9a-128">unknown</span><span class="sxs-lookup"><span data-stu-id="18e9a-128">unknown</span></span>|<span data-ttu-id="18e9a-129">0</span><span class="sxs-lookup"><span data-stu-id="18e9a-129">0</span></span>|<span data-ttu-id="18e9a-130">打印机报告的处理状态未知。</span><span class="sxs-lookup"><span data-stu-id="18e9a-130">The processing state reported by the printer is unknown.</span></span>|
|<span data-ttu-id="18e9a-131">待机</span><span class="sxs-lookup"><span data-stu-id="18e9a-131">idle</span></span>|<span data-ttu-id="18e9a-132">1</span><span class="sxs-lookup"><span data-stu-id="18e9a-132">1</span></span>|<span data-ttu-id="18e9a-133">打印机处于空闲状态，并已准备好接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="18e9a-133">The printer is idle and ready to accept new print jobs.</span></span>|
|<span data-ttu-id="18e9a-134">处理</span><span class="sxs-lookup"><span data-stu-id="18e9a-134">processing</span></span>|<span data-ttu-id="18e9a-135">双面</span><span class="sxs-lookup"><span data-stu-id="18e9a-135">2</span></span>|<span data-ttu-id="18e9a-136">打印机当前正在处理打印作业，并将在完成时处理任何挂起的作业。</span><span class="sxs-lookup"><span data-stu-id="18e9a-136">The printer is currently processing a print job and will process any pending jobs upon completion.</span></span>|
|<span data-ttu-id="18e9a-137">停止</span><span class="sxs-lookup"><span data-stu-id="18e9a-137">stopped</span></span>|<span data-ttu-id="18e9a-138">第三章</span><span class="sxs-lookup"><span data-stu-id="18e9a-138">3</span></span>|<span data-ttu-id="18e9a-139">打印机遇到问题 (例如，在活动纸盒中缺纸) ，并且在解决问题之前无法继续当前的打印作业。</span><span class="sxs-lookup"><span data-stu-id="18e9a-139">The printer encountered an issue (for example, ran out of paper in the active tray) and cannot continue the current print job until the issue is addressed.</span></span> <span data-ttu-id="18e9a-140">有关详细信息，请参阅 (s) 的 **详细** 信息值或 **描述** 值。</span><span class="sxs-lookup"><span data-stu-id="18e9a-140">See the **details** value(s) or the **description** value for more information.</span></span>|
|<span data-ttu-id="18e9a-141">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="18e9a-141">unknownFutureValue</span></span>|<span data-ttu-id="18e9a-142">4 </span><span class="sxs-lookup"><span data-stu-id="18e9a-142">4</span></span>|<span data-ttu-id="18e9a-143">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="18e9a-143">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="18e9a-144">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="18e9a-144">Do not use.</span></span>|

### <a name="printerprocessingstatedetail-values"></a><span data-ttu-id="18e9a-145">printerProcessingStateDetail 值</span><span class="sxs-lookup"><span data-stu-id="18e9a-145">printerProcessingStateDetail values</span></span>

|<span data-ttu-id="18e9a-146">成员</span><span class="sxs-lookup"><span data-stu-id="18e9a-146">Member</span></span>|<span data-ttu-id="18e9a-147">值</span><span class="sxs-lookup"><span data-stu-id="18e9a-147">Value</span></span>|<span data-ttu-id="18e9a-148">说明</span><span class="sxs-lookup"><span data-stu-id="18e9a-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e9a-149">停留</span><span class="sxs-lookup"><span data-stu-id="18e9a-149">paused</span></span>|<span data-ttu-id="18e9a-150">0</span><span class="sxs-lookup"><span data-stu-id="18e9a-150">0</span></span>| <span data-ttu-id="18e9a-151">正在进行的打印作业已暂停。</span><span class="sxs-lookup"><span data-stu-id="18e9a-151">An ongoing print job was paused.</span></span>|
|<span data-ttu-id="18e9a-152">被</span><span class="sxs-lookup"><span data-stu-id="18e9a-152">disconnected</span></span>|<span data-ttu-id="18e9a-153">1</span><span class="sxs-lookup"><span data-stu-id="18e9a-153">1</span></span>|<span data-ttu-id="18e9a-154">与打印机的连接丢失或无法建立连接。</span><span class="sxs-lookup"><span data-stu-id="18e9a-154">The connection to the printer was lost or cannot be established.</span></span>|
|<span data-ttu-id="18e9a-155">mediaJam</span><span class="sxs-lookup"><span data-stu-id="18e9a-155">mediaJam</span></span>|<span data-ttu-id="18e9a-156">双面</span><span class="sxs-lookup"><span data-stu-id="18e9a-156">2</span></span>|<span data-ttu-id="18e9a-157">一个或多个纸盒中的介质卡纸。</span><span class="sxs-lookup"><span data-stu-id="18e9a-157">Media in one or more trays is jammed.</span></span>|
|<span data-ttu-id="18e9a-158">mediaNeeded</span><span class="sxs-lookup"><span data-stu-id="18e9a-158">mediaNeeded</span></span>|<span data-ttu-id="18e9a-159">第三章</span><span class="sxs-lookup"><span data-stu-id="18e9a-159">3</span></span>|<span data-ttu-id="18e9a-160">必须先替换当前使用的输入送纸器中的媒体，然后才能继续执行作业。</span><span class="sxs-lookup"><span data-stu-id="18e9a-160">Media in the currently-used input tray needs to be replaced before the job can continue.</span></span>|
|<span data-ttu-id="18e9a-161">mediaLow</span><span class="sxs-lookup"><span data-stu-id="18e9a-161">mediaLow</span></span>|<span data-ttu-id="18e9a-162">4 </span><span class="sxs-lookup"><span data-stu-id="18e9a-162">4</span></span>|<span data-ttu-id="18e9a-163">一个或多个送纸器中的媒体几乎耗尽。</span><span class="sxs-lookup"><span data-stu-id="18e9a-163">Media in one or more trays is almost exhausted.</span></span>|
|<span data-ttu-id="18e9a-164">mediaEmpty</span><span class="sxs-lookup"><span data-stu-id="18e9a-164">mediaEmpty</span></span>|<span data-ttu-id="18e9a-165">5 </span><span class="sxs-lookup"><span data-stu-id="18e9a-165">5</span></span>|<span data-ttu-id="18e9a-166">一个或多个托盘中的媒体已耗尽。</span><span class="sxs-lookup"><span data-stu-id="18e9a-166">Media in one or more trays is exhausted.</span></span>|
|<span data-ttu-id="18e9a-167">coverOpen</span><span class="sxs-lookup"><span data-stu-id="18e9a-167">coverOpen</span></span>|<span data-ttu-id="18e9a-168">6 </span><span class="sxs-lookup"><span data-stu-id="18e9a-168">6</span></span>|<span data-ttu-id="18e9a-169">打开了一个或多个封面。</span><span class="sxs-lookup"><span data-stu-id="18e9a-169">One or more covers are open.</span></span>|
|<span data-ttu-id="18e9a-170">interlockOpen</span><span class="sxs-lookup"><span data-stu-id="18e9a-170">interlockOpen</span></span>|<span data-ttu-id="18e9a-171">7 </span><span class="sxs-lookup"><span data-stu-id="18e9a-171">7</span></span>|<span data-ttu-id="18e9a-172">一个或多个互锁设备已打开。</span><span class="sxs-lookup"><span data-stu-id="18e9a-172">One or more interlock devices are open.</span></span>|
|<span data-ttu-id="18e9a-173">queueFull</span><span class="sxs-lookup"><span data-stu-id="18e9a-173">queueFull</span></span>|<span data-ttu-id="18e9a-174">8 </span><span class="sxs-lookup"><span data-stu-id="18e9a-174">8</span></span>|<span data-ttu-id="18e9a-175">打印机的后台打印程序队列已满，无法排队新的作业。</span><span class="sxs-lookup"><span data-stu-id="18e9a-175">The printer's spooler queue is full and new jobs cannot be queued.</span></span>|
|<span data-ttu-id="18e9a-176">outputTrayMissing</span><span class="sxs-lookup"><span data-stu-id="18e9a-176">outputTrayMissing</span></span>|<span data-ttu-id="18e9a-177">9 </span><span class="sxs-lookup"><span data-stu-id="18e9a-177">9</span></span>|<span data-ttu-id="18e9a-178">一个或多个输出送纸器丢失。</span><span class="sxs-lookup"><span data-stu-id="18e9a-178">One or more output trays are missing.</span></span>|
|<span data-ttu-id="18e9a-179">outputAreaFull</span><span class="sxs-lookup"><span data-stu-id="18e9a-179">outputAreaFull</span></span>|<span data-ttu-id="18e9a-180">10  </span><span class="sxs-lookup"><span data-stu-id="18e9a-180">10</span></span>|<span data-ttu-id="18e9a-181">一个或多个输出托盘已满，无法接受更多的媒体。</span><span class="sxs-lookup"><span data-stu-id="18e9a-181">One or more output trays are full and cannot accept more media.</span></span>|
|<span data-ttu-id="18e9a-182">markerSupplyLow</span><span class="sxs-lookup"><span data-stu-id="18e9a-182">markerSupplyLow</span></span>|<span data-ttu-id="18e9a-183">11x17</span><span class="sxs-lookup"><span data-stu-id="18e9a-183">11</span></span>|<span data-ttu-id="18e9a-184">一个或多个标记源 (例如，墨水、墨粉或功能区) 不足。</span><span class="sxs-lookup"><span data-stu-id="18e9a-184">One or more marker sources (for example, ink, toner or ribbon) are low.</span></span>|
|<span data-ttu-id="18e9a-185">markerSupplyEmpty</span><span class="sxs-lookup"><span data-stu-id="18e9a-185">markerSupplyEmpty</span></span>|<span data-ttu-id="18e9a-186">12 </span><span class="sxs-lookup"><span data-stu-id="18e9a-186">12</span></span>|<span data-ttu-id="18e9a-187">一个或多个标记源 (例如，墨水、墨粉或功能区) 耗尽。</span><span class="sxs-lookup"><span data-stu-id="18e9a-187">One or more marker sources (for example, ink, toner or ribbon) are exhausted.</span></span>|
|<span data-ttu-id="18e9a-188">inputTrayMissing</span><span class="sxs-lookup"><span data-stu-id="18e9a-188">inputTrayMissing</span></span>|<span data-ttu-id="18e9a-189">13 </span><span class="sxs-lookup"><span data-stu-id="18e9a-189">13</span></span>|<span data-ttu-id="18e9a-190">一个或多个输入送纸器不在设备中。</span><span class="sxs-lookup"><span data-stu-id="18e9a-190">One or more input trays are not in the device.</span></span>|
|<span data-ttu-id="18e9a-191">outputAlmostFull</span><span class="sxs-lookup"><span data-stu-id="18e9a-191">outputAlmostFull</span></span>|<span data-ttu-id="18e9a-192">14 </span><span class="sxs-lookup"><span data-stu-id="18e9a-192">14</span></span>|<span data-ttu-id="18e9a-193">一个或多个输出区域几乎已满 (例如，"任务栏"、"堆栈器"、"排序程序") 。</span><span class="sxs-lookup"><span data-stu-id="18e9a-193">One or more output area is almost full (for example, tray, stacker, collator).</span></span>|
|<span data-ttu-id="18e9a-194">markerWasteAlmostFull</span><span class="sxs-lookup"><span data-stu-id="18e9a-194">markerWasteAlmostFull</span></span>|<span data-ttu-id="18e9a-195">15 </span><span class="sxs-lookup"><span data-stu-id="18e9a-195">15</span></span>|<span data-ttu-id="18e9a-196">设备标记供应废物容器几乎已满。</span><span class="sxs-lookup"><span data-stu-id="18e9a-196">The device marker supply waste receptacle is almost full.</span></span>|
|<span data-ttu-id="18e9a-197">markerWasteFull</span><span class="sxs-lookup"><span data-stu-id="18e9a-197">markerWasteFull</span></span>|<span data-ttu-id="18e9a-198">16 </span><span class="sxs-lookup"><span data-stu-id="18e9a-198">16</span></span>|<span data-ttu-id="18e9a-199">设备标记供应废物容器已满。</span><span class="sxs-lookup"><span data-stu-id="18e9a-199">The device marker supply waste receptacle is full.</span></span>|
|<span data-ttu-id="18e9a-200">fuserOverTemp</span><span class="sxs-lookup"><span data-stu-id="18e9a-200">fuserOverTemp</span></span>|<span data-ttu-id="18e9a-201">17 </span><span class="sxs-lookup"><span data-stu-id="18e9a-201">17</span></span>|<span data-ttu-id="18e9a-202">热熔器温度高于正常水平。</span><span class="sxs-lookup"><span data-stu-id="18e9a-202">The fuser temperature is above normal.</span></span>|
|<span data-ttu-id="18e9a-203">fuserUnderTemp</span><span class="sxs-lookup"><span data-stu-id="18e9a-203">fuserUnderTemp</span></span>|<span data-ttu-id="18e9a-204">18 </span><span class="sxs-lookup"><span data-stu-id="18e9a-204">18</span></span>|<span data-ttu-id="18e9a-205">热熔器温度低于正常水平。</span><span class="sxs-lookup"><span data-stu-id="18e9a-205">The fuser temperature is below normal.</span></span>|
|<span data-ttu-id="18e9a-206">相互</span><span class="sxs-lookup"><span data-stu-id="18e9a-206">other</span></span>|<span data-ttu-id="18e9a-207">合</span><span class="sxs-lookup"><span data-stu-id="18e9a-207">19</span></span>|<span data-ttu-id="18e9a-208">不属于其余原因的任何其他原因。</span><span class="sxs-lookup"><span data-stu-id="18e9a-208">Any other reason that does not fall in rest of the reasons.</span></span>|
|<span data-ttu-id="18e9a-209">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="18e9a-209">unknownFutureValue</span></span>|<span data-ttu-id="18e9a-210">20</span><span class="sxs-lookup"><span data-stu-id="18e9a-210">20</span></span>|<span data-ttu-id="18e9a-211">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="18e9a-211">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="18e9a-212">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="18e9a-212">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18e9a-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18e9a-213">JSON representation</span></span>

<span data-ttu-id="18e9a-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18e9a-214">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerStatus"
}-->

```json
{
    "state": "String",
    "details": ["String"],
    "description": "String"
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

