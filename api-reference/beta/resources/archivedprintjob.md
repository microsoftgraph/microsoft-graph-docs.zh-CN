---
title: archivedPrintJob 资源类型
description: 用于报告目的的 "最终状态" （已完成、已终止或已失败）打印作业的记录。 这不是活动的打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 170f3b735b4f14173058efbaaa1c81b80490f020
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895600"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="185d3-104">archivedPrintJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="185d3-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="185d3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="185d3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="185d3-106">用于报告目的的 "最终状态" （已完成、已终止或已失败）打印作业的记录。</span><span class="sxs-lookup"><span data-stu-id="185d3-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="185d3-107">这不是活动的打印作业。</span><span class="sxs-lookup"><span data-stu-id="185d3-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="185d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="185d3-108">Properties</span></span>
| <span data-ttu-id="185d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="185d3-109">Property</span></span>     | <span data-ttu-id="185d3-110">类型</span><span class="sxs-lookup"><span data-stu-id="185d3-110">Type</span></span>        | <span data-ttu-id="185d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="185d3-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="185d3-112">id</span><span class="sxs-lookup"><span data-stu-id="185d3-112">id</span></span>|<span data-ttu-id="185d3-113">String</span><span class="sxs-lookup"><span data-stu-id="185d3-113">String</span></span>|<span data-ttu-id="185d3-114">存档的打印作业的 GUID。</span><span class="sxs-lookup"><span data-stu-id="185d3-114">The archived print job's GUID.</span></span> <span data-ttu-id="185d3-115">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-115">Read-only.</span></span>|
|<span data-ttu-id="185d3-116">printerId</span><span class="sxs-lookup"><span data-stu-id="185d3-116">printerId</span></span>|<span data-ttu-id="185d3-117">String</span><span class="sxs-lookup"><span data-stu-id="185d3-117">String</span></span>|<span data-ttu-id="185d3-118">作业排队等待的打印机 ID。</span><span class="sxs-lookup"><span data-stu-id="185d3-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="185d3-119">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-119">Read-only.</span></span>|
|<span data-ttu-id="185d3-120">processingState</span><span class="sxs-lookup"><span data-stu-id="185d3-120">processingState</span></span>|<span data-ttu-id="185d3-121">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="185d3-121">printJobProcessingState</span></span>|<span data-ttu-id="185d3-122">打印作业的最终处理状态。</span><span class="sxs-lookup"><span data-stu-id="185d3-122">The print job's final processing state.</span></span> <span data-ttu-id="185d3-123">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-123">Read-only.</span></span>|
|<span data-ttu-id="185d3-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="185d3-124">createdDateTime</span></span>|<span data-ttu-id="185d3-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="185d3-125">DateTimeOffset</span></span>|<span data-ttu-id="185d3-126">创建作业时的 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="185d3-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="185d3-127">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-127">Read-only.</span></span>|
|<span data-ttu-id="185d3-128">acquiredDateTime</span><span class="sxs-lookup"><span data-stu-id="185d3-128">acquiredDateTime</span></span>|<span data-ttu-id="185d3-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="185d3-129">DateTimeOffset</span></span>|<span data-ttu-id="185d3-130">打印机获取作业时的 dateTimeOffset （如果有）。</span><span class="sxs-lookup"><span data-stu-id="185d3-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="185d3-131">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-131">Read-only.</span></span>|
|<span data-ttu-id="185d3-132">completionDateTime</span><span class="sxs-lookup"><span data-stu-id="185d3-132">completionDateTime</span></span>|<span data-ttu-id="185d3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="185d3-133">DateTimeOffset</span></span>|<span data-ttu-id="185d3-134">作业完成、取消或终止时的 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="185d3-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="185d3-135">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-135">Read-only.</span></span>|
|<span data-ttu-id="185d3-136">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="185d3-136">acquiredByPrinter</span></span>|<span data-ttu-id="185d3-137">布尔</span><span class="sxs-lookup"><span data-stu-id="185d3-137">Boolean</span></span>|<span data-ttu-id="185d3-138">如果作业是由打印机获取的，则为 True; 否则为否则为 false。</span><span class="sxs-lookup"><span data-stu-id="185d3-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="185d3-139">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-139">Read-only.</span></span>|
|<span data-ttu-id="185d3-140">copiesPrinted</span><span class="sxs-lookup"><span data-stu-id="185d3-140">copiesPrinted</span></span>|<span data-ttu-id="185d3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="185d3-141">Int32</span></span>|<span data-ttu-id="185d3-142">打印的份数。</span><span class="sxs-lookup"><span data-stu-id="185d3-142">The number of copies that were printed.</span></span> <span data-ttu-id="185d3-143">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-143">Read-only.</span></span>|
|<span data-ttu-id="185d3-144">pageCount</span><span class="sxs-lookup"><span data-stu-id="185d3-144">pageCount</span></span>|<span data-ttu-id="185d3-145">Int32</span><span class="sxs-lookup"><span data-stu-id="185d3-145">Int32</span></span>|<span data-ttu-id="185d3-146">打印的总页数。</span><span class="sxs-lookup"><span data-stu-id="185d3-146">The total number of pages that were printed.</span></span> <span data-ttu-id="185d3-147">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-147">Read-only.</span></span>|
|<span data-ttu-id="185d3-148">blackAndWhitePageCount</span><span class="sxs-lookup"><span data-stu-id="185d3-148">blackAndWhitePageCount</span></span>|<span data-ttu-id="185d3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="185d3-149">Int32</span></span>|<span data-ttu-id="185d3-150">打印的黑白页面数。</span><span class="sxs-lookup"><span data-stu-id="185d3-150">The number of black and white pages that were printed.</span></span> <span data-ttu-id="185d3-151">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-151">Read-only.</span></span>|
|<span data-ttu-id="185d3-152">colorPageCount</span><span class="sxs-lookup"><span data-stu-id="185d3-152">colorPageCount</span></span>|<span data-ttu-id="185d3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="185d3-153">Int32</span></span>|<span data-ttu-id="185d3-154">打印的彩色页面的数量。</span><span class="sxs-lookup"><span data-stu-id="185d3-154">The number of color pages that were printed.</span></span> <span data-ttu-id="185d3-155">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-155">Read-only.</span></span>|
|<span data-ttu-id="185d3-156">simplexPageCount</span><span class="sxs-lookup"><span data-stu-id="185d3-156">simplexPageCount</span></span>|<span data-ttu-id="185d3-157">Int32</span><span class="sxs-lookup"><span data-stu-id="185d3-157">Int32</span></span>|<span data-ttu-id="185d3-158">打印的单面（单面）页面的数量。</span><span class="sxs-lookup"><span data-stu-id="185d3-158">The number of simplex (single-sided) pages that were printed.</span></span> <span data-ttu-id="185d3-159">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-159">Read-only.</span></span>|
|<span data-ttu-id="185d3-160">duplexPageCount</span><span class="sxs-lookup"><span data-stu-id="185d3-160">duplexPageCount</span></span>|<span data-ttu-id="185d3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="185d3-161">Int32</span></span>|<span data-ttu-id="185d3-162">打印的双工（双面）页面的数量。</span><span class="sxs-lookup"><span data-stu-id="185d3-162">The number of duplex (double-sided) pages that were printed.</span></span> <span data-ttu-id="185d3-163">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-163">Read-only.</span></span>|
|<span data-ttu-id="185d3-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="185d3-164">createdBy</span></span>|[<span data-ttu-id="185d3-165">userIdentity</span><span class="sxs-lookup"><span data-stu-id="185d3-165">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="185d3-166">创建打印作业的用户。</span><span class="sxs-lookup"><span data-stu-id="185d3-166">The user who created the print job.</span></span> <span data-ttu-id="185d3-167">只读。</span><span class="sxs-lookup"><span data-stu-id="185d3-167">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="185d3-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="185d3-168">JSON representation</span></span>

<span data-ttu-id="185d3-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="185d3-169">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->

```json
{
    "id": "String (identifier)",
    "printer": {"@odata.type": "microsoft.graph.directoryObject"},
    "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
    "processingState": {"@odata.type": "microsoft.graph.printJobProcessingState"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "archivedPrintJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->