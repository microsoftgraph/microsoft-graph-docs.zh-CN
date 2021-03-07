---
title: printJobStatus 资源类型
description: 表示打印作业的当前状态。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7a6f5e0c728c1de122f9b642b9de2f1db050cf09
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517292"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="7f79a-103">printJobStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f79a-103">printJobStatus resource type</span></span>

<span data-ttu-id="7f79a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f79a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="7f79a-105">表示打印作业的当前状态。</span><span class="sxs-lookup"><span data-stu-id="7f79a-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="7f79a-106">属性</span><span class="sxs-lookup"><span data-stu-id="7f79a-106">Properties</span></span>
|<span data-ttu-id="7f79a-107">属性</span><span class="sxs-lookup"><span data-stu-id="7f79a-107">Property</span></span>|<span data-ttu-id="7f79a-108">类型</span><span class="sxs-lookup"><span data-stu-id="7f79a-108">Type</span></span>|<span data-ttu-id="7f79a-109">Description</span><span class="sxs-lookup"><span data-stu-id="7f79a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f79a-110">state</span><span class="sxs-lookup"><span data-stu-id="7f79a-110">state</span></span>|<span data-ttu-id="7f79a-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="7f79a-111">printJobProcessingState</span></span>|<span data-ttu-id="7f79a-112">打印作业的当前处理状态。</span><span class="sxs-lookup"><span data-stu-id="7f79a-112">The print job's current processing state.</span></span> <span data-ttu-id="7f79a-113">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="7f79a-113">Valid values are described in the following table.</span></span> <span data-ttu-id="7f79a-114">只读。</span><span class="sxs-lookup"><span data-stu-id="7f79a-114">Read-only.</span></span>|
|<span data-ttu-id="7f79a-115">详细信息</span><span class="sxs-lookup"><span data-stu-id="7f79a-115">details</span></span>|<span data-ttu-id="7f79a-116">printJobProcessingDetail 集合</span><span class="sxs-lookup"><span data-stu-id="7f79a-116">printJobProcessingDetail collection</span></span>|<span data-ttu-id="7f79a-117">打印作业状态的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="7f79a-117">Additional details for print job state.</span></span> <span data-ttu-id="7f79a-118">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="7f79a-118">Valid values are described in the following table.</span></span> <span data-ttu-id="7f79a-119">只读。</span><span class="sxs-lookup"><span data-stu-id="7f79a-119">Read-only.</span></span>|
|<span data-ttu-id="7f79a-120">说明</span><span class="sxs-lookup"><span data-stu-id="7f79a-120">description</span></span>|<span data-ttu-id="7f79a-121">String</span><span class="sxs-lookup"><span data-stu-id="7f79a-121">String</span></span>|<span data-ttu-id="7f79a-122">可读的打印作业当前处理状态的说明。</span><span class="sxs-lookup"><span data-stu-id="7f79a-122">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="7f79a-123">只读。</span><span class="sxs-lookup"><span data-stu-id="7f79a-123">Read-only.</span></span>|
|<span data-ttu-id="7f79a-124">isAcquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="7f79a-124">isAcquiredByPrinter</span></span>|<span data-ttu-id="7f79a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f79a-125">Boolean</span></span>|<span data-ttu-id="7f79a-126">如此 如果打印机确认作业;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="7f79a-126">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="7f79a-127">只读。</span><span class="sxs-lookup"><span data-stu-id="7f79a-127">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="7f79a-128">printJobProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="7f79a-128">printJobProcessingState values</span></span>

|<span data-ttu-id="7f79a-129">成员</span><span class="sxs-lookup"><span data-stu-id="7f79a-129">Member</span></span>|<span data-ttu-id="7f79a-130">值</span><span class="sxs-lookup"><span data-stu-id="7f79a-130">Value</span></span>|<span data-ttu-id="7f79a-131">Description</span><span class="sxs-lookup"><span data-stu-id="7f79a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f79a-132">unknown</span><span class="sxs-lookup"><span data-stu-id="7f79a-132">unknown</span></span>|<span data-ttu-id="7f79a-133">0</span><span class="sxs-lookup"><span data-stu-id="7f79a-133">0</span></span>|<span data-ttu-id="7f79a-134">无法识别打印机报告的处理状态。</span><span class="sxs-lookup"><span data-stu-id="7f79a-134">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="7f79a-135">挂起</span><span class="sxs-lookup"><span data-stu-id="7f79a-135">pending</span></span>|<span data-ttu-id="7f79a-136">1 </span><span class="sxs-lookup"><span data-stu-id="7f79a-136">1</span></span>|<span data-ttu-id="7f79a-137">打印机正在挂起打印作业的处理。</span><span class="sxs-lookup"><span data-stu-id="7f79a-137">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="7f79a-138">processing</span><span class="sxs-lookup"><span data-stu-id="7f79a-138">processing</span></span>|<span data-ttu-id="7f79a-139">2 </span><span class="sxs-lookup"><span data-stu-id="7f79a-139">2</span></span>|<span data-ttu-id="7f79a-140">打印作业当前正由打印机处理。</span><span class="sxs-lookup"><span data-stu-id="7f79a-140">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="7f79a-141">paused</span><span class="sxs-lookup"><span data-stu-id="7f79a-141">paused</span></span>|<span data-ttu-id="7f79a-142">3 </span><span class="sxs-lookup"><span data-stu-id="7f79a-142">3</span></span>|<span data-ttu-id="7f79a-143">打印作业已暂停。</span><span class="sxs-lookup"><span data-stu-id="7f79a-143">The print job has been paused.</span></span>|
|<span data-ttu-id="7f79a-144">已停止</span><span class="sxs-lookup"><span data-stu-id="7f79a-144">stopped</span></span>|<span data-ttu-id="7f79a-145">4 </span><span class="sxs-lookup"><span data-stu-id="7f79a-145">4</span></span>|<span data-ttu-id="7f79a-146">打印作业已停止，因为需要解决打印机的问题，然后作业才能继续。</span><span class="sxs-lookup"><span data-stu-id="7f79a-146">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="7f79a-147">可在打印机状态资源中找到详细信息。</span><span class="sxs-lookup"><span data-stu-id="7f79a-147">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="7f79a-148">已完成</span><span class="sxs-lookup"><span data-stu-id="7f79a-148">completed</span></span>|<span data-ttu-id="7f79a-149">5 </span><span class="sxs-lookup"><span data-stu-id="7f79a-149">5</span></span>|<span data-ttu-id="7f79a-150">打印作业已成功完成，不会进行进一步处理。</span><span class="sxs-lookup"><span data-stu-id="7f79a-150">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="7f79a-151">canceled</span><span class="sxs-lookup"><span data-stu-id="7f79a-151">canceled</span></span>|<span data-ttu-id="7f79a-152">6 </span><span class="sxs-lookup"><span data-stu-id="7f79a-152">6</span></span>|<span data-ttu-id="7f79a-153">打印作业已由用户取消，不会进行进一步处理。</span><span class="sxs-lookup"><span data-stu-id="7f79a-153">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="7f79a-154">已中止</span><span class="sxs-lookup"><span data-stu-id="7f79a-154">aborted</span></span>|<span data-ttu-id="7f79a-155">7 </span><span class="sxs-lookup"><span data-stu-id="7f79a-155">7</span></span>|<span data-ttu-id="7f79a-156">打印作业已由用户或打印机中止，不会进行进一步处理。</span><span class="sxs-lookup"><span data-stu-id="7f79a-156">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

### <a name="printjobprocessingdetail-values"></a><span data-ttu-id="7f79a-157">printJobProcessingDetail 值</span><span class="sxs-lookup"><span data-stu-id="7f79a-157">printJobProcessingDetail values</span></span>

|<span data-ttu-id="7f79a-158">成员</span><span class="sxs-lookup"><span data-stu-id="7f79a-158">Member</span></span>|<span data-ttu-id="7f79a-159">值</span><span class="sxs-lookup"><span data-stu-id="7f79a-159">Value</span></span>|<span data-ttu-id="7f79a-160">Description</span><span class="sxs-lookup"><span data-stu-id="7f79a-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f79a-161">uploadPending</span><span class="sxs-lookup"><span data-stu-id="7f79a-161">uploadPending</span></span>|<span data-ttu-id="7f79a-162">0</span><span class="sxs-lookup"><span data-stu-id="7f79a-162">0</span></span>|<span data-ttu-id="7f79a-163">尚未上载文档有效负载。</span><span class="sxs-lookup"><span data-stu-id="7f79a-163">Document payload has not been uploaded.</span></span>|
|<span data-ttu-id="7f79a-164">转换</span><span class="sxs-lookup"><span data-stu-id="7f79a-164">transforming</span></span>|<span data-ttu-id="7f79a-165">1 </span><span class="sxs-lookup"><span data-stu-id="7f79a-165">1</span></span>|<span data-ttu-id="7f79a-166">正在转换文档有效负载。</span><span class="sxs-lookup"><span data-stu-id="7f79a-166">Document payload is being transformed.</span></span>|
|<span data-ttu-id="7f79a-167">completedSuccessfully</span><span class="sxs-lookup"><span data-stu-id="7f79a-167">completedSuccessfully</span></span>|<span data-ttu-id="7f79a-168">2 </span><span class="sxs-lookup"><span data-stu-id="7f79a-168">2</span></span>|<span data-ttu-id="7f79a-169">作业已成功完成。</span><span class="sxs-lookup"><span data-stu-id="7f79a-169">Job has been completed successfully.</span></span>|
|<span data-ttu-id="7f79a-170">completedWithWarnings</span><span class="sxs-lookup"><span data-stu-id="7f79a-170">completedWithWarnings</span></span>|<span data-ttu-id="7f79a-171">3 </span><span class="sxs-lookup"><span data-stu-id="7f79a-171">3</span></span>|<span data-ttu-id="7f79a-172">作业已完成，并出现警告。</span><span class="sxs-lookup"><span data-stu-id="7f79a-172">Job has been completed with warnings.</span></span>|
|<span data-ttu-id="7f79a-173">completedWithErrors</span><span class="sxs-lookup"><span data-stu-id="7f79a-173">completedWithErrors</span></span>|<span data-ttu-id="7f79a-174">4 </span><span class="sxs-lookup"><span data-stu-id="7f79a-174">4</span></span>|<span data-ttu-id="7f79a-175">作业已完成，出现错误。</span><span class="sxs-lookup"><span data-stu-id="7f79a-175">Job has been completed with errors.</span></span>|
|<span data-ttu-id="7f79a-176">releaseWait</span><span class="sxs-lookup"><span data-stu-id="7f79a-176">releaseWait</span></span>|<span data-ttu-id="7f79a-177">5 </span><span class="sxs-lookup"><span data-stu-id="7f79a-177">5</span></span>|<span data-ttu-id="7f79a-178">作业正在等待发布。</span><span class="sxs-lookup"><span data-stu-id="7f79a-178">Job is pending to be released.</span></span>|
|<span data-ttu-id="7f79a-179">解释</span><span class="sxs-lookup"><span data-stu-id="7f79a-179">interpreting</span></span>|<span data-ttu-id="7f79a-180">6 </span><span class="sxs-lookup"><span data-stu-id="7f79a-180">6</span></span>|<span data-ttu-id="7f79a-181">作业正在"处理"状态，但更具体地说，正在解释文档有效负载。</span><span class="sxs-lookup"><span data-stu-id="7f79a-181">Job is in 'processing' state, but more specifically, document payload is being interpreted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f79a-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f79a-182">JSON representation</span></span>
<span data-ttu-id="7f79a-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f79a-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobStatus",
  "state": "String",
  "description": "String",
  "isAcquiredByPrinter": "Boolean",
  "details": [
    "String"
  ]
}
```

