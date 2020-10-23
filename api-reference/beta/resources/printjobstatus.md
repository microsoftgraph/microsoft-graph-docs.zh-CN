---
title: printJobStatus 资源类型
description: 表示打印作业的当前状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bb3221eb12946d58664211731a31993e540aaf00
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728933"
---
# <a name="printjobstatus-resource-type"></a><span data-ttu-id="65157-103">printJobStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="65157-103">printJobStatus resource type</span></span>

<span data-ttu-id="65157-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65157-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65157-105">表示打印作业的当前状态。</span><span class="sxs-lookup"><span data-stu-id="65157-105">Represents the current status of a print job.</span></span>

## <a name="properties"></a><span data-ttu-id="65157-106">属性</span><span class="sxs-lookup"><span data-stu-id="65157-106">Properties</span></span>
| <span data-ttu-id="65157-107">属性</span><span class="sxs-lookup"><span data-stu-id="65157-107">Property</span></span>     | <span data-ttu-id="65157-108">类型</span><span class="sxs-lookup"><span data-stu-id="65157-108">Type</span></span>        | <span data-ttu-id="65157-109">说明</span><span class="sxs-lookup"><span data-stu-id="65157-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65157-110">state</span><span class="sxs-lookup"><span data-stu-id="65157-110">state</span></span>|<span data-ttu-id="65157-111">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="65157-111">printJobProcessingState</span></span>|<span data-ttu-id="65157-112">打印作业的当前处理状态。</span><span class="sxs-lookup"><span data-stu-id="65157-112">The print job's current processing state.</span></span> <span data-ttu-id="65157-113">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="65157-113">Valid values are described in the following table.</span></span> <span data-ttu-id="65157-114">只读。</span><span class="sxs-lookup"><span data-stu-id="65157-114">Read-only.</span></span>|
|<span data-ttu-id="65157-115">详细信息</span><span class="sxs-lookup"><span data-stu-id="65157-115">details</span></span>|<span data-ttu-id="65157-116">printJobProcessingDetail 集合</span><span class="sxs-lookup"><span data-stu-id="65157-116">printJobProcessingDetail collection</span></span>|<span data-ttu-id="65157-117">打印作业状态的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="65157-117">Additional details for print job state.</span></span> <span data-ttu-id="65157-118">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="65157-118">Valid values are described in the following table.</span></span> <span data-ttu-id="65157-119">只读。</span><span class="sxs-lookup"><span data-stu-id="65157-119">Read-only.</span></span>|
|<span data-ttu-id="65157-120">说明</span><span class="sxs-lookup"><span data-stu-id="65157-120">description</span></span>|<span data-ttu-id="65157-121">String</span><span class="sxs-lookup"><span data-stu-id="65157-121">String</span></span>|<span data-ttu-id="65157-122">打印作业的当前处理状态的可读说明。</span><span class="sxs-lookup"><span data-stu-id="65157-122">A human-readable description of the print job's current processing state.</span></span> <span data-ttu-id="65157-123">只读。</span><span class="sxs-lookup"><span data-stu-id="65157-123">Read-only.</span></span>|
|<span data-ttu-id="65157-124">isAcquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="65157-124">isAcquiredByPrinter</span></span>|<span data-ttu-id="65157-125">布尔</span><span class="sxs-lookup"><span data-stu-id="65157-125">Boolean</span></span>|<span data-ttu-id="65157-126">如果作业已由打印机确认，则为 True; 否则为 false。否则为 false。</span><span class="sxs-lookup"><span data-stu-id="65157-126">True if the job was acknowledged by a printer; false otherwise.</span></span> <span data-ttu-id="65157-127">只读。</span><span class="sxs-lookup"><span data-stu-id="65157-127">Read-only.</span></span>|

### <a name="printjobprocessingstate-values"></a><span data-ttu-id="65157-128">printJobProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="65157-128">printJobProcessingState values</span></span>

|<span data-ttu-id="65157-129">成员</span><span class="sxs-lookup"><span data-stu-id="65157-129">Member</span></span>|<span data-ttu-id="65157-130">值</span><span class="sxs-lookup"><span data-stu-id="65157-130">Value</span></span>|<span data-ttu-id="65157-131">说明</span><span class="sxs-lookup"><span data-stu-id="65157-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65157-132">unknown</span><span class="sxs-lookup"><span data-stu-id="65157-132">unknown</span></span>|<span data-ttu-id="65157-133">0</span><span class="sxs-lookup"><span data-stu-id="65157-133">0</span></span>|<span data-ttu-id="65157-134">无法识别打印机报告的处理状态。</span><span class="sxs-lookup"><span data-stu-id="65157-134">The processing state reported by the printer is not recognized.</span></span>|
|<span data-ttu-id="65157-135">决</span><span class="sxs-lookup"><span data-stu-id="65157-135">pending</span></span>|<span data-ttu-id="65157-136">1</span><span class="sxs-lookup"><span data-stu-id="65157-136">1</span></span>|<span data-ttu-id="65157-137">打印作业正在等待打印机处理。</span><span class="sxs-lookup"><span data-stu-id="65157-137">The print job is pending processing by the printer.</span></span>|
|<span data-ttu-id="65157-138">处理</span><span class="sxs-lookup"><span data-stu-id="65157-138">processing</span></span>|<span data-ttu-id="65157-139">双面</span><span class="sxs-lookup"><span data-stu-id="65157-139">2</span></span>|<span data-ttu-id="65157-140">打印机当前正在处理打印作业。</span><span class="sxs-lookup"><span data-stu-id="65157-140">The print job is currently being processed by the printer.</span></span>|
|<span data-ttu-id="65157-141">停留</span><span class="sxs-lookup"><span data-stu-id="65157-141">paused</span></span>|<span data-ttu-id="65157-142">第三章</span><span class="sxs-lookup"><span data-stu-id="65157-142">3</span></span>|<span data-ttu-id="65157-143">打印作业已暂停。</span><span class="sxs-lookup"><span data-stu-id="65157-143">The print job has been paused.</span></span>|
|<span data-ttu-id="65157-144">停止</span><span class="sxs-lookup"><span data-stu-id="65157-144">stopped</span></span>|<span data-ttu-id="65157-145">4 </span><span class="sxs-lookup"><span data-stu-id="65157-145">4</span></span>|<span data-ttu-id="65157-146">打印作业已停止，因为需要先解决打印机问题，然后才能继续执行作业。</span><span class="sxs-lookup"><span data-stu-id="65157-146">The print job has been stopped because an issue with the printer needs to be addressed before the job can continue.</span></span> <span data-ttu-id="65157-147">在打印机状态资源中可以找到详细信息。</span><span class="sxs-lookup"><span data-stu-id="65157-147">More information can be found in the printer state resource.</span></span>|
|<span data-ttu-id="65157-148">后</span><span class="sxs-lookup"><span data-stu-id="65157-148">completed</span></span>|<span data-ttu-id="65157-149">5 </span><span class="sxs-lookup"><span data-stu-id="65157-149">5</span></span>|<span data-ttu-id="65157-150">打印作业已成功完成，不会进行进一步的处理。</span><span class="sxs-lookup"><span data-stu-id="65157-150">The print job has completed successfully and no further processing will take place.</span></span>|
|<span data-ttu-id="65157-151">取消</span><span class="sxs-lookup"><span data-stu-id="65157-151">canceled</span></span>|<span data-ttu-id="65157-152">6 </span><span class="sxs-lookup"><span data-stu-id="65157-152">6</span></span>|<span data-ttu-id="65157-153">打印作业已被用户取消，不会进行进一步的处理。</span><span class="sxs-lookup"><span data-stu-id="65157-153">The print job has been canceled by a user and no further processing will take place.</span></span>|
|<span data-ttu-id="65157-154">其间</span><span class="sxs-lookup"><span data-stu-id="65157-154">aborted</span></span>|<span data-ttu-id="65157-155">7 </span><span class="sxs-lookup"><span data-stu-id="65157-155">7</span></span>|<span data-ttu-id="65157-156">打印作业已被用户或打印机中止，不会进行进一步处理。</span><span class="sxs-lookup"><span data-stu-id="65157-156">The print job has been aborted by a user or the printer and no further processing will take place.</span></span>|

### <a name="printjobprocessingdetail-values"></a><span data-ttu-id="65157-157">printJobProcessingDetail 值</span><span class="sxs-lookup"><span data-stu-id="65157-157">printJobProcessingDetail values</span></span>

|<span data-ttu-id="65157-158">成员</span><span class="sxs-lookup"><span data-stu-id="65157-158">Member</span></span>|<span data-ttu-id="65157-159">值</span><span class="sxs-lookup"><span data-stu-id="65157-159">Value</span></span>|<span data-ttu-id="65157-160">说明</span><span class="sxs-lookup"><span data-stu-id="65157-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65157-161">uploadPending</span><span class="sxs-lookup"><span data-stu-id="65157-161">uploadPending</span></span>|<span data-ttu-id="65157-162">0</span><span class="sxs-lookup"><span data-stu-id="65157-162">0</span></span>|<span data-ttu-id="65157-163">尚未上传文档有效负载。</span><span class="sxs-lookup"><span data-stu-id="65157-163">Document payload has not been uploaded.</span></span>|
|<span data-ttu-id="65157-164">改变</span><span class="sxs-lookup"><span data-stu-id="65157-164">transforming</span></span>|<span data-ttu-id="65157-165">1</span><span class="sxs-lookup"><span data-stu-id="65157-165">1</span></span>|<span data-ttu-id="65157-166">正在转换文档有效负载。</span><span class="sxs-lookup"><span data-stu-id="65157-166">Document payload is being transformed.</span></span>|
|<span data-ttu-id="65157-167">completedSuccessfully</span><span class="sxs-lookup"><span data-stu-id="65157-167">completedSuccessfully</span></span>|<span data-ttu-id="65157-168">双面</span><span class="sxs-lookup"><span data-stu-id="65157-168">2</span></span>|<span data-ttu-id="65157-169">作业已成功完成。</span><span class="sxs-lookup"><span data-stu-id="65157-169">Job has been completed successfully.</span></span>|
|<span data-ttu-id="65157-170">completedWithWarnings</span><span class="sxs-lookup"><span data-stu-id="65157-170">completedWithWarnings</span></span>|<span data-ttu-id="65157-171">第三章</span><span class="sxs-lookup"><span data-stu-id="65157-171">3</span></span>|<span data-ttu-id="65157-172">作业已完成，但出现警告。</span><span class="sxs-lookup"><span data-stu-id="65157-172">Job has been completed with warnings.</span></span>|
|<span data-ttu-id="65157-173">completedWithErrors</span><span class="sxs-lookup"><span data-stu-id="65157-173">completedWithErrors</span></span>|<span data-ttu-id="65157-174">4 </span><span class="sxs-lookup"><span data-stu-id="65157-174">4</span></span>|<span data-ttu-id="65157-175">作业已完成，但有错误。</span><span class="sxs-lookup"><span data-stu-id="65157-175">Job has been completed with errors.</span></span>|
|<span data-ttu-id="65157-176">releaseWait</span><span class="sxs-lookup"><span data-stu-id="65157-176">releaseWait</span></span>|<span data-ttu-id="65157-177">5 </span><span class="sxs-lookup"><span data-stu-id="65157-177">5</span></span>|<span data-ttu-id="65157-178">作业挂起，无法释放。</span><span class="sxs-lookup"><span data-stu-id="65157-178">Job is pending to be released.</span></span>|
|<span data-ttu-id="65157-179">口译</span><span class="sxs-lookup"><span data-stu-id="65157-179">interpreting</span></span>|<span data-ttu-id="65157-180">6 </span><span class="sxs-lookup"><span data-stu-id="65157-180">6</span></span>|<span data-ttu-id="65157-181">作业处于 "正在处理" 状态，但更具体地说，是解释文档有效负载。</span><span class="sxs-lookup"><span data-stu-id="65157-181">Job is in 'processing' state, but more specifically, document payload is being interpreted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65157-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65157-182">JSON representation</span></span>

<span data-ttu-id="65157-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65157-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJobStatus"
}-->

```json
{
    "state": "String",
    "description": "String",
    "isAcquiredByPrinter": true,    
    "details": ["String"]
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

