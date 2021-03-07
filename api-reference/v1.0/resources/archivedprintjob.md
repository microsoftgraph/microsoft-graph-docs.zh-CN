---
title: archivedPrintJob 资源类型
description: "\"最终状态\"记录 (用于报告目的) 打印作业已完成、中止或失败。 这不是活动的打印作业。"
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2132b5a7cdf5024fb13845c57844220594ba6e1f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517213"
---
# <a name="archivedprintjob-resource-type"></a><span data-ttu-id="d1a92-104">archivedPrintJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1a92-104">archivedPrintJob resource type</span></span>

<span data-ttu-id="d1a92-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1a92-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1a92-106">"最终状态"记录 (用于报告目的) 打印作业已完成、中止或失败。</span><span class="sxs-lookup"><span data-stu-id="d1a92-106">A record of a "final state" (completed, aborted or failed) print job that is used for reporting purposes.</span></span> <span data-ttu-id="d1a92-107">这不是活动的打印作业。</span><span class="sxs-lookup"><span data-stu-id="d1a92-107">This is not an active print job.</span></span>

## <a name="properties"></a><span data-ttu-id="d1a92-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1a92-108">Properties</span></span>
| <span data-ttu-id="d1a92-109">属性</span><span class="sxs-lookup"><span data-stu-id="d1a92-109">Property</span></span>     | <span data-ttu-id="d1a92-110">类型</span><span class="sxs-lookup"><span data-stu-id="d1a92-110">Type</span></span>        | <span data-ttu-id="d1a92-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1a92-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d1a92-112">id</span><span class="sxs-lookup"><span data-stu-id="d1a92-112">id</span></span>|<span data-ttu-id="d1a92-113">String</span><span class="sxs-lookup"><span data-stu-id="d1a92-113">String</span></span>|<span data-ttu-id="d1a92-114">已存档打印作业的 GUID。</span><span class="sxs-lookup"><span data-stu-id="d1a92-114">The archived print job's GUID.</span></span> <span data-ttu-id="d1a92-115">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-115">Read-only.</span></span>|
|<span data-ttu-id="d1a92-116">printerId</span><span class="sxs-lookup"><span data-stu-id="d1a92-116">printerId</span></span>|<span data-ttu-id="d1a92-117">String</span><span class="sxs-lookup"><span data-stu-id="d1a92-117">String</span></span>|<span data-ttu-id="d1a92-118">作业排队的打印机 ID。</span><span class="sxs-lookup"><span data-stu-id="d1a92-118">The printer ID that the job was queued for.</span></span> <span data-ttu-id="d1a92-119">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-119">Read-only.</span></span>|
|<span data-ttu-id="d1a92-120">processingState</span><span class="sxs-lookup"><span data-stu-id="d1a92-120">processingState</span></span>|<span data-ttu-id="d1a92-121">printJobProcessingState</span><span class="sxs-lookup"><span data-stu-id="d1a92-121">printJobProcessingState</span></span>|<span data-ttu-id="d1a92-122">打印作业的最终处理状态。</span><span class="sxs-lookup"><span data-stu-id="d1a92-122">The print job's final processing state.</span></span> <span data-ttu-id="d1a92-123">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-123">Read-only.</span></span>|
|<span data-ttu-id="d1a92-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1a92-124">createdDateTime</span></span>|<span data-ttu-id="d1a92-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1a92-125">DateTimeOffset</span></span>|<span data-ttu-id="d1a92-126">创建作业时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="d1a92-126">The dateTimeOffset when the job was created.</span></span> <span data-ttu-id="d1a92-127">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-127">Read-only.</span></span>|
|<span data-ttu-id="d1a92-128">acquiredDateTime</span><span class="sxs-lookup"><span data-stu-id="d1a92-128">acquiredDateTime</span></span>|<span data-ttu-id="d1a92-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1a92-129">DateTimeOffset</span></span>|<span data-ttu-id="d1a92-130">打印机获取作业的日期时间Offset（如果有）。</span><span class="sxs-lookup"><span data-stu-id="d1a92-130">The dateTimeOffset when the job was acquired by the printer, if any.</span></span> <span data-ttu-id="d1a92-131">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-131">Read-only.</span></span>|
|<span data-ttu-id="d1a92-132">completionDateTime</span><span class="sxs-lookup"><span data-stu-id="d1a92-132">completionDateTime</span></span>|<span data-ttu-id="d1a92-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1a92-133">DateTimeOffset</span></span>|<span data-ttu-id="d1a92-134">作业完成、取消或中止时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="d1a92-134">The dateTimeOffset when the job was completed, canceled or aborted.</span></span> <span data-ttu-id="d1a92-135">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-135">Read-only.</span></span>|
|<span data-ttu-id="d1a92-136">acquiredByPrinter</span><span class="sxs-lookup"><span data-stu-id="d1a92-136">acquiredByPrinter</span></span>|<span data-ttu-id="d1a92-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1a92-137">Boolean</span></span>|<span data-ttu-id="d1a92-138">如此 如果打印机获取作业;否则为 false。</span><span class="sxs-lookup"><span data-stu-id="d1a92-138">True if the job was acquired by a printer; false otherwise.</span></span> <span data-ttu-id="d1a92-139">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-139">Read-only.</span></span>|
|<span data-ttu-id="d1a92-140">copiesPrinted</span><span class="sxs-lookup"><span data-stu-id="d1a92-140">copiesPrinted</span></span>|<span data-ttu-id="d1a92-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d1a92-141">Int32</span></span>|<span data-ttu-id="d1a92-142">打印的副本数。</span><span class="sxs-lookup"><span data-stu-id="d1a92-142">The number of copies that were printed.</span></span> <span data-ttu-id="d1a92-143">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-143">Read-only.</span></span>|
|<span data-ttu-id="d1a92-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="d1a92-144">createdBy</span></span>|[<span data-ttu-id="d1a92-145">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d1a92-145">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="d1a92-146">创建打印作业的用户。</span><span class="sxs-lookup"><span data-stu-id="d1a92-146">The user who created the print job.</span></span> <span data-ttu-id="d1a92-147">只读。</span><span class="sxs-lookup"><span data-stu-id="d1a92-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1a92-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1a92-148">JSON representation</span></span>

<span data-ttu-id="d1a92-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1a92-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.archivedPrintJob"
}-->
```json
    {   
  "@odata.type": "#microsoft.graph.archivedPrintJob",   
  "id": "String (identifier)",  
  "printerId": "String",    
  "processingState": "String",  
  "createdDateTime": "String (timestamp)",  
  "acquiredDateTime": "String (timestamp)", 
  "completionDateTime": "String (timestamp)",   
  "acquiredByPrinter": "Boolean",   
  "copiesPrinted": "Integer",   
  "createdBy": {    
    "@odata.type": "microsoft.graph.userIdentity"   
  } 
}
```