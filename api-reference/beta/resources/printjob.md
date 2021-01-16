---
title: printJob 资源类型
description: 表示已排入打印机队列的打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5124f3123331c4889f5e16110109938e7f264925
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883031"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="d83f9-103">printJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="d83f9-103">printJob resource type</span></span>

<span data-ttu-id="d83f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d83f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d83f9-105">表示已排入打印机队列的打印作业。</span><span class="sxs-lookup"><span data-stu-id="d83f9-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="d83f9-106">Methods</span><span class="sxs-lookup"><span data-stu-id="d83f9-106">Methods</span></span>

| <span data-ttu-id="d83f9-107">方法</span><span class="sxs-lookup"><span data-stu-id="d83f9-107">Method</span></span>       | <span data-ttu-id="d83f9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d83f9-108">Return Type</span></span> | <span data-ttu-id="d83f9-109">说明</span><span class="sxs-lookup"><span data-stu-id="d83f9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d83f9-110">获取</span><span class="sxs-lookup"><span data-stu-id="d83f9-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="d83f9-111">printJob</span><span class="sxs-lookup"><span data-stu-id="d83f9-111">printJob</span></span>](printjob.md) | <span data-ttu-id="d83f9-112">读取 printJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d83f9-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="d83f9-113">创建</span><span class="sxs-lookup"><span data-stu-id="d83f9-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="d83f9-114">printJob</span><span class="sxs-lookup"><span data-stu-id="d83f9-114">printJob</span></span>](printjob.md) | <span data-ttu-id="d83f9-115">创建新的打印作业对象。</span><span class="sxs-lookup"><span data-stu-id="d83f9-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="d83f9-116">开始</span><span class="sxs-lookup"><span data-stu-id="d83f9-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="d83f9-117">无</span><span class="sxs-lookup"><span data-stu-id="d83f9-117">None</span></span>|<span data-ttu-id="d83f9-118">启动打印作业。</span><span class="sxs-lookup"><span data-stu-id="d83f9-118">Start the print job.</span></span>|
| [<span data-ttu-id="d83f9-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="d83f9-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="d83f9-120">无</span><span class="sxs-lookup"><span data-stu-id="d83f9-120">None</span></span>|<span data-ttu-id="d83f9-121">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="d83f9-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="d83f9-122">中止</span><span class="sxs-lookup"><span data-stu-id="d83f9-122">Abort</span></span>](../api/printjob-abort.md)|<span data-ttu-id="d83f9-123">无</span><span class="sxs-lookup"><span data-stu-id="d83f9-123">None</span></span>|<span data-ttu-id="d83f9-124">中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="d83f9-124">Abort the print job.</span></span>|
| [<span data-ttu-id="d83f9-125">将 (重定向到另一个打印机) </span><span class="sxs-lookup"><span data-stu-id="d83f9-125">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="d83f9-126">printJob</span><span class="sxs-lookup"><span data-stu-id="d83f9-126">printJob</span></span>](printjob.md) | <span data-ttu-id="d83f9-127">已排入目标打印机队列的打印作业。</span><span class="sxs-lookup"><span data-stu-id="d83f9-127">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="d83f9-128">属性</span><span class="sxs-lookup"><span data-stu-id="d83f9-128">Properties</span></span>
| <span data-ttu-id="d83f9-129">属性</span><span class="sxs-lookup"><span data-stu-id="d83f9-129">Property</span></span>     | <span data-ttu-id="d83f9-130">类型</span><span class="sxs-lookup"><span data-stu-id="d83f9-130">Type</span></span>        | <span data-ttu-id="d83f9-131">说明</span><span class="sxs-lookup"><span data-stu-id="d83f9-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d83f9-132">id</span><span class="sxs-lookup"><span data-stu-id="d83f9-132">id</span></span>|<span data-ttu-id="d83f9-133">String</span><span class="sxs-lookup"><span data-stu-id="d83f9-133">String</span></span>|<span data-ttu-id="d83f9-134">打印机的 GUID。</span><span class="sxs-lookup"><span data-stu-id="d83f9-134">The printer's GUID.</span></span> <span data-ttu-id="d83f9-135">只读。</span><span class="sxs-lookup"><span data-stu-id="d83f9-135">Read-only.</span></span>|
|<span data-ttu-id="d83f9-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d83f9-136">createdDateTime</span></span>|<span data-ttu-id="d83f9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d83f9-137">DateTimeOffset</span></span>|<span data-ttu-id="d83f9-138">创建作业时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="d83f9-138">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="d83f9-139">只读。</span><span class="sxs-lookup"><span data-stu-id="d83f9-139">Read-only.</span></span>|
|<span data-ttu-id="d83f9-140">status</span><span class="sxs-lookup"><span data-stu-id="d83f9-140">status</span></span>|[<span data-ttu-id="d83f9-141">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="d83f9-141">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="d83f9-142">打印作业的状态。</span><span class="sxs-lookup"><span data-stu-id="d83f9-142">The status of the print job.</span></span> <span data-ttu-id="d83f9-143">只读。</span><span class="sxs-lookup"><span data-stu-id="d83f9-143">Read-only.</span></span>|
|<span data-ttu-id="d83f9-144">configuration</span><span class="sxs-lookup"><span data-stu-id="d83f9-144">configuration</span></span>|[<span data-ttu-id="d83f9-145">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="d83f9-145">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="d83f9-146">打印机用于打印作业的一组设置。</span><span class="sxs-lookup"><span data-stu-id="d83f9-146">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="d83f9-147">isFetchable</span><span class="sxs-lookup"><span data-stu-id="d83f9-147">isFetchable</span></span>|<span data-ttu-id="d83f9-148">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="d83f9-148">Edm.Boolean</span></span>|<span data-ttu-id="d83f9-149">如果为 true，则打印机可以提取文档。</span><span class="sxs-lookup"><span data-stu-id="d83f9-149">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="d83f9-150">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="d83f9-150">redirectedFrom</span></span>|<span data-ttu-id="d83f9-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="d83f9-151">Edm.String</span></span>|<span data-ttu-id="d83f9-152">包含源作业 URL（如果作业已从另一台打印机重定向）。</span><span class="sxs-lookup"><span data-stu-id="d83f9-152">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="d83f9-153">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="d83f9-153">redirectedTo</span></span>|<span data-ttu-id="d83f9-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="d83f9-154">Edm.String</span></span>|<span data-ttu-id="d83f9-155">包含目标作业 URL（如果作业已重定向到其他打印机）。</span><span class="sxs-lookup"><span data-stu-id="d83f9-155">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d83f9-156">关系</span><span class="sxs-lookup"><span data-stu-id="d83f9-156">Relationships</span></span>
| <span data-ttu-id="d83f9-157">关系</span><span class="sxs-lookup"><span data-stu-id="d83f9-157">Relationship</span></span> | <span data-ttu-id="d83f9-158">类型</span><span class="sxs-lookup"><span data-stu-id="d83f9-158">Type</span></span>        | <span data-ttu-id="d83f9-159">说明</span><span class="sxs-lookup"><span data-stu-id="d83f9-159">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d83f9-160">createdBy</span><span class="sxs-lookup"><span data-stu-id="d83f9-160">createdBy</span></span>|[<span data-ttu-id="d83f9-161">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d83f9-161">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="d83f9-162">只读。</span><span class="sxs-lookup"><span data-stu-id="d83f9-162">Read-only.</span></span> <span data-ttu-id="d83f9-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d83f9-163">Nullable.</span></span>|
|<span data-ttu-id="d83f9-164">documents</span><span class="sxs-lookup"><span data-stu-id="d83f9-164">documents</span></span>|<span data-ttu-id="d83f9-165">[printDocument](printdocument.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d83f9-165">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="d83f9-166">只读。</span><span class="sxs-lookup"><span data-stu-id="d83f9-166">Read-only.</span></span>|
|<span data-ttu-id="d83f9-167">tasks</span><span class="sxs-lookup"><span data-stu-id="d83f9-167">tasks</span></span>|<span data-ttu-id="d83f9-168">[printTask](printtask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d83f9-168">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="d83f9-169">此打印作业触发的 [printTasks](printtask.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="d83f9-169">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d83f9-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d83f9-170">JSON representation</span></span>

<span data-ttu-id="d83f9-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d83f9-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJob",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "isFetchable": "Boolean",
  "redirectedFrom": "String",
  "redirectedTo": "String",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "configuration": {"@odata.type": "microsoft.graph.printJobConfiguration"},
  "documents": [ {"@odata.type": "microsoft.graph.printDocument"} ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

