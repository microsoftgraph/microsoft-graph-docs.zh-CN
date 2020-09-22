---
title: archivedPrintJob 资源类型
description: "\"最终状态\" (\"已完成\"、\"已中止\" 或 \"失败\" 的记录) 用于报告目的的打印作业。 这不是活动的打印作业。"
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d4bd76dc84ad41c6d412144d13a784bec4f6a9f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050127"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="32546-104">archivedPrintJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="32546-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="32546-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32546-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32546-106">"最终状态" ("已完成"、"已中止" 或 "失败" 的记录) 用于报告目的的打印作业。</span><span class="sxs-lookup"><span data-stu-id="32546-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="32546-107">这不是活动的打印作业。</span><span class="sxs-lookup"><span data-stu-id="32546-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="32546-108">属性</span><span class="sxs-lookup"><span data-stu-id="32546-108">Properties</span></span>
| <span data-ttu-id="32546-109">属性</span><span class="sxs-lookup"><span data-stu-id="32546-109">Property</span></span>     | <span data-ttu-id="32546-110">类型</span><span class="sxs-lookup"><span data-stu-id="32546-110">Type</span></span>        | <span data-ttu-id="32546-111">说明</span><span class="sxs-lookup"><span data-stu-id="32546-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="32546-112">id</span><span class="sxs-lookup"><span data-stu-id="32546-112">id</span></span>|<span data-ttu-id="32546-113">String</span><span class="sxs-lookup"><span data-stu-id="32546-113">String</span></span>|<span data-ttu-id="32546-114">存档的打印作业的 GUID。</span><span class="sxs-lookup"><span data-stu-id="32546-114">The archived print job's GUID.</span></span> <span data-ttu-id="32546-115">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-115">Read-only.</span></span>|
|<span data-ttu-id="32546-116">printerId</span><span class="sxs-lookup"><span data-stu-id="32546-116">printerId</span></span>|<span data-ttu-id="32546-117">String</span><span class="sxs-lookup"><span data-stu-id="32546-117">String</span></span>|<span data-ttu-id="32546-118">作业排队等待的打印机 ID。</span><span class="sxs-lookup"><span data-stu-id="32546-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="32546-119">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-119">Read-only.</span></span>|
|<span data-ttu-id="32546-120">processingState</span><span class="sxs-lookup"><span data-stu-id="32546-120">processingState</span></span>|<span data-ttu-id="32546-121">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="32546-121">printJobProcessingState</span></span>|<span data-ttu-id="32546-122">打印作业的最终处理状态。</span><span class="sxs-lookup"><span data-stu-id="32546-122">The print job's final processing state.</span></span> <span data-ttu-id="32546-123">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-123">Read-only.</span></span>|
|<span data-ttu-id="32546-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32546-124">createdDateTime</span></span>|<span data-ttu-id="32546-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32546-125">DateTimeOffset</span></span>|<span data-ttu-id="32546-126">创建作业时的 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="32546-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="32546-127">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-127">Read-only.</span></span>|
|<span data-ttu-id="32546-128">acquiredDateTime</span><span class="sxs-lookup"><span data-stu-id="32546-128">acquiredDateTime</span></span>|<span data-ttu-id="32546-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32546-129">DateTimeOffset</span></span>|<span data-ttu-id="32546-130">打印机获取作业时的 dateTimeOffset （如果有）。</span><span class="sxs-lookup"><span data-stu-id="32546-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="32546-131">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-131">Read-only.</span></span>|
|<span data-ttu-id="32546-132">completionDateTime</span><span class="sxs-lookup"><span data-stu-id="32546-132">completionDateTime</span></span>|<span data-ttu-id="32546-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32546-133">DateTimeOffset</span></span>|<span data-ttu-id="32546-134">作业完成、取消或终止时的 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="32546-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="32546-135">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-135">Read-only.</span></span>|
|<span data-ttu-id="32546-136">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="32546-136">acquiredByPrinter</span></span>|<span data-ttu-id="32546-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="32546-137">Boolean</span></span>|<span data-ttu-id="32546-138">如果作业是由打印机获取的，则为 True; 否则为否则为 false。</span><span class="sxs-lookup"><span data-stu-id="32546-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="32546-139">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-139">Read-only.</span></span>|
|<span data-ttu-id="32546-140">copiesPrinted</span><span class="sxs-lookup"><span data-stu-id="32546-140">copiesPrinted</span></span>|<span data-ttu-id="32546-141">Int32</span><span class="sxs-lookup"><span data-stu-id="32546-141">Int32</span></span>|<span data-ttu-id="32546-142">打印的份数。</span><span class="sxs-lookup"><span data-stu-id="32546-142">The number of copies that were printed.</span></span> <span data-ttu-id="32546-143">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-143">Read-only.</span></span>|
|<span data-ttu-id="32546-144">pageCount</span><span class="sxs-lookup"><span data-stu-id="32546-144">pageCount</span></span>|<span data-ttu-id="32546-145">Int32</span><span class="sxs-lookup"><span data-stu-id="32546-145">Int32</span></span>|<span data-ttu-id="32546-146">打印的总页数。</span><span class="sxs-lookup"><span data-stu-id="32546-146">The total number of pages that were printed.</span></span> <span data-ttu-id="32546-147">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-147">Read-only.</span></span>|
|<span data-ttu-id="32546-148">blackAndWhitePageCount</span><span class="sxs-lookup"><span data-stu-id="32546-148">blackAndWhitePageCount</span></span>|<span data-ttu-id="32546-149">Int32</span><span class="sxs-lookup"><span data-stu-id="32546-149">Int32</span></span>|<span data-ttu-id="32546-150">打印的黑白页面数。</span><span class="sxs-lookup"><span data-stu-id="32546-150">The number of black and white pages that were printed.</span></span> <span data-ttu-id="32546-151">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-151">Read-only.</span></span>|
|<span data-ttu-id="32546-152">colorPageCount</span><span class="sxs-lookup"><span data-stu-id="32546-152">colorPageCount</span></span>|<span data-ttu-id="32546-153">Int32</span><span class="sxs-lookup"><span data-stu-id="32546-153">Int32</span></span>|<span data-ttu-id="32546-154">打印的彩色页面的数量。</span><span class="sxs-lookup"><span data-stu-id="32546-154">The number of color pages that were printed.</span></span> <span data-ttu-id="32546-155">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-155">Read-only.</span></span>|
|<span data-ttu-id="32546-156">simplexPageCount</span><span class="sxs-lookup"><span data-stu-id="32546-156">simplexPageCount</span></span>|<span data-ttu-id="32546-157">Int32</span><span class="sxs-lookup"><span data-stu-id="32546-157">Int32</span></span>|<span data-ttu-id="32546-158">打印的单 (单面) 页的数量。</span><span class="sxs-lookup"><span data-stu-id="32546-158">The number of simplex (single-sided) pages that were printed.</span></span> <span data-ttu-id="32546-159">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-159">Read-only.</span></span>|
|<span data-ttu-id="32546-160">duplexPageCount</span><span class="sxs-lookup"><span data-stu-id="32546-160">duplexPageCount</span></span>|<span data-ttu-id="32546-161">Int32</span><span class="sxs-lookup"><span data-stu-id="32546-161">Int32</span></span>|<span data-ttu-id="32546-162">打印的双面打印 (双面) 页的数量。</span><span class="sxs-lookup"><span data-stu-id="32546-162">The number of duplex (double-sided) pages that were printed.</span></span> <span data-ttu-id="32546-163">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-163">Read-only.</span></span>|
|<span data-ttu-id="32546-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="32546-164">createdBy</span></span>|[<span data-ttu-id="32546-165">userIdentity</span><span class="sxs-lookup"><span data-stu-id="32546-165">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="32546-166">创建打印作业的用户。</span><span class="sxs-lookup"><span data-stu-id="32546-166">The user who created the print job.</span></span> <span data-ttu-id="32546-167">只读。</span><span class="sxs-lookup"><span data-stu-id="32546-167">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32546-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32546-168">JSON representation</span></span>

<span data-ttu-id="32546-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32546-169">The following is a JSON representation of the resource.</span></span>

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

