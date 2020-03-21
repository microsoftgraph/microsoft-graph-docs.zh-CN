---
title: printJobStatus 资源类型
description: 表示打印作业的当前状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 1973d00ff8ca544f0acd1992626de9a3eaf59700
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895602"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="4c8ab-103">printJobStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c8ab-103">printJobStatus resource type</span></span>

<span data-ttu-id="4c8ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c8ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c8ab-105">表示打印作业的当前状态。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="4c8ab-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c8ab-106">Properties</span></span>
| <span data-ttu-id="4c8ab-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c8ab-107">Property</span></span>     | <span data-ttu-id="4c8ab-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c8ab-108">Type</span></span>        | <span data-ttu-id="4c8ab-109">说明</span><span class="sxs-lookup"><span data-stu-id="4c8ab-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4c8ab-110">processingState</span><span class="sxs-lookup"><span data-stu-id="4c8ab-110">processingState</span></span>|<span data-ttu-id="4c8ab-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="4c8ab-111">printJobProcessingState</span></span>|<span data-ttu-id="4c8ab-112">打印作业的当前处理状态。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-112">The print job's current processing state.</span></span> <span data-ttu-id="4c8ab-113">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-113">Valid values are described in the following table.</span></span> <span data-ttu-id="4c8ab-114">只读。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-114">Read-only.</span></span>|
|<span data-ttu-id="4c8ab-115">processingStateDescription</span><span class="sxs-lookup"><span data-stu-id="4c8ab-115">processingStateDescription</span></span>|<span data-ttu-id="4c8ab-116">String</span><span class="sxs-lookup"><span data-stu-id="4c8ab-116">String</span></span>|<span data-ttu-id="4c8ab-117">打印作业的当前处理状态的可读说明。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-117">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="4c8ab-118">只读。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-118">Read-only.</span></span>|
|<span data-ttu-id="4c8ab-119">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="4c8ab-119">acquiredByPrinter</span></span>|<span data-ttu-id="4c8ab-120">布尔</span><span class="sxs-lookup"><span data-stu-id="4c8ab-120">Boolean</span></span>|<span data-ttu-id="4c8ab-121">如果作业已由打印机确认，则为 True; 否则为 false。否则为 false。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-121">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="4c8ab-122">只读。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-122">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="4c8ab-123">printJobProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="4c8ab-123">printJobProcessingState values</span></span>

|<span data-ttu-id="4c8ab-124">成员</span><span class="sxs-lookup"><span data-stu-id="4c8ab-124">Member</span></span>|<span data-ttu-id="4c8ab-125">值</span><span class="sxs-lookup"><span data-stu-id="4c8ab-125">Value</span></span>|<span data-ttu-id="4c8ab-126">说明</span><span class="sxs-lookup"><span data-stu-id="4c8ab-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c8ab-127">unknown</span><span class="sxs-lookup"><span data-stu-id="4c8ab-127">unknown</span></span>|<span data-ttu-id="4c8ab-128">0</span><span class="sxs-lookup"><span data-stu-id="4c8ab-128">0</span></span>|<span data-ttu-id="4c8ab-129">无法识别打印机报告的处理状态。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-129">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="4c8ab-130">决</span><span class="sxs-lookup"><span data-stu-id="4c8ab-130">pending</span></span>|<span data-ttu-id="4c8ab-131">1</span><span class="sxs-lookup"><span data-stu-id="4c8ab-131">1</span></span>|<span data-ttu-id="4c8ab-132">打印作业正在等待打印机处理。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-132">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="4c8ab-133">pendingHeld</span><span class="sxs-lookup"><span data-stu-id="4c8ab-133">pendingHeld</span></span>|<span data-ttu-id="4c8ab-134">双面</span><span class="sxs-lookup"><span data-stu-id="4c8ab-134">2</span></span>|<span data-ttu-id="4c8ab-135">该作业不是处理的候选项。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-135">The job is not a candidate for processing yet.</span></span> <span data-ttu-id="4c8ab-136">确保没有导致作业无法启动的错误或资源限制。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-136">Ensure that there are no errors or resource limitations preventing the job from starting.</span></span>|
|<span data-ttu-id="4c8ab-137">处理</span><span class="sxs-lookup"><span data-stu-id="4c8ab-137">processing</span></span>|<span data-ttu-id="4c8ab-138">第三章</span><span class="sxs-lookup"><span data-stu-id="4c8ab-138">3</span></span>|<span data-ttu-id="4c8ab-139">打印机当前正在处理打印作业。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-139">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="4c8ab-140">停留</span><span class="sxs-lookup"><span data-stu-id="4c8ab-140">paused</span></span>|<span data-ttu-id="4c8ab-141">4 </span><span class="sxs-lookup"><span data-stu-id="4c8ab-141">4</span></span>|<span data-ttu-id="4c8ab-142">用户已暂停打印作业。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-142">The print job has been paused by a user.</span></span>|
|<span data-ttu-id="4c8ab-143">停止</span><span class="sxs-lookup"><span data-stu-id="4c8ab-143">stopped</span></span>|<span data-ttu-id="4c8ab-144">5 </span><span class="sxs-lookup"><span data-stu-id="4c8ab-144">5</span></span>|<span data-ttu-id="4c8ab-145">打印作业已停止，因为需要先解决打印机问题，然后才能继续执行作业。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-145">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="4c8ab-146">在打印机状态资源中可以找到详细信息。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-146">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="4c8ab-147">后</span><span class="sxs-lookup"><span data-stu-id="4c8ab-147">completed</span></span>|<span data-ttu-id="4c8ab-148">6 </span><span class="sxs-lookup"><span data-stu-id="4c8ab-148">6</span></span>|<span data-ttu-id="4c8ab-149">打印作业已成功完成，不会进行进一步的处理。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-149">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="4c8ab-150">取消</span><span class="sxs-lookup"><span data-stu-id="4c8ab-150">canceled</span></span>|<span data-ttu-id="4c8ab-151">7 </span><span class="sxs-lookup"><span data-stu-id="4c8ab-151">7</span></span>|<span data-ttu-id="4c8ab-152">打印作业已被用户取消，不会进行进一步的处理。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-152">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="4c8ab-153">其间</span><span class="sxs-lookup"><span data-stu-id="4c8ab-153">aborted</span></span>|<span data-ttu-id="4c8ab-154">8 </span><span class="sxs-lookup"><span data-stu-id="4c8ab-154">8</span></span>|<span data-ttu-id="4c8ab-155">打印作业已被用户或打印机中止，不会进行进一步处理。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-155">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c8ab-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c8ab-156">JSON representation</span></span>

<span data-ttu-id="4c8ab-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c8ab-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "processingState": "String",
    "processingStateDescription": "String",
    "acquiredByPrinter": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJobStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->