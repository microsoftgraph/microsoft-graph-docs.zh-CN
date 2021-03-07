---
title: printJob 资源类型
description: 表示已排入打印机队列的打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3115164fcc15ef6c2133ef3616624af9141da1af
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517295"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="e31bc-103">printJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="e31bc-103">printJob resource type</span></span>

<span data-ttu-id="e31bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e31bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e31bc-105">表示已排入打印机队列的打印作业。</span><span class="sxs-lookup"><span data-stu-id="e31bc-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="e31bc-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e31bc-106">Methods</span></span>
| <span data-ttu-id="e31bc-107">方法</span><span class="sxs-lookup"><span data-stu-id="e31bc-107">Method</span></span>       | <span data-ttu-id="e31bc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e31bc-108">Return Type</span></span> | <span data-ttu-id="e31bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="e31bc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e31bc-110">获取</span><span class="sxs-lookup"><span data-stu-id="e31bc-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="e31bc-111">printJob</span><span class="sxs-lookup"><span data-stu-id="e31bc-111">printJob</span></span>](printjob.md) | <span data-ttu-id="e31bc-112">读取 printJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e31bc-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="e31bc-113">创建</span><span class="sxs-lookup"><span data-stu-id="e31bc-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="e31bc-114">printJob</span><span class="sxs-lookup"><span data-stu-id="e31bc-114">printJob</span></span>](printjob.md) | <span data-ttu-id="e31bc-115">创建新的打印作业对象。</span><span class="sxs-lookup"><span data-stu-id="e31bc-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="e31bc-116">更新</span><span class="sxs-lookup"><span data-stu-id="e31bc-116">Update</span></span>](../api/printjob-update.md) | [<span data-ttu-id="e31bc-117">printJob</span><span class="sxs-lookup"><span data-stu-id="e31bc-117">printJob</span></span>](printjob.md) | <span data-ttu-id="e31bc-118">更新打印作业对象。</span><span class="sxs-lookup"><span data-stu-id="e31bc-118">Update a print job object.</span></span> |
| [<span data-ttu-id="e31bc-119">开始</span><span class="sxs-lookup"><span data-stu-id="e31bc-119">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="e31bc-120">无</span><span class="sxs-lookup"><span data-stu-id="e31bc-120">None</span></span>|<span data-ttu-id="e31bc-121">启动打印作业。</span><span class="sxs-lookup"><span data-stu-id="e31bc-121">Start the print job.</span></span>|
| [<span data-ttu-id="e31bc-122">Cancel</span><span class="sxs-lookup"><span data-stu-id="e31bc-122">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="e31bc-123">无</span><span class="sxs-lookup"><span data-stu-id="e31bc-123">None</span></span>|<span data-ttu-id="e31bc-124">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="e31bc-124">Cancel the print job.</span></span>|
| [<span data-ttu-id="e31bc-125">中止</span><span class="sxs-lookup"><span data-stu-id="e31bc-125">Abort</span></span>](../api/printjob-abort.md)|<span data-ttu-id="e31bc-126">无</span><span class="sxs-lookup"><span data-stu-id="e31bc-126">None</span></span>|<span data-ttu-id="e31bc-127">中止打印作业。</span><span class="sxs-lookup"><span data-stu-id="e31bc-127">Abort the print job.</span></span>|
| [<span data-ttu-id="e31bc-128">将 (重定向到另一个打印机) </span><span class="sxs-lookup"><span data-stu-id="e31bc-128">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="e31bc-129">printJob</span><span class="sxs-lookup"><span data-stu-id="e31bc-129">printJob</span></span>](printjob.md) | <span data-ttu-id="e31bc-130">已排入目标打印机队列的打印作业。</span><span class="sxs-lookup"><span data-stu-id="e31bc-130">A print job that is queued for the destination printer.</span></span> |


## <a name="properties"></a><span data-ttu-id="e31bc-131">属性</span><span class="sxs-lookup"><span data-stu-id="e31bc-131">Properties</span></span>
|<span data-ttu-id="e31bc-132">属性</span><span class="sxs-lookup"><span data-stu-id="e31bc-132">Property</span></span>|<span data-ttu-id="e31bc-133">类型</span><span class="sxs-lookup"><span data-stu-id="e31bc-133">Type</span></span>|<span data-ttu-id="e31bc-134">说明</span><span class="sxs-lookup"><span data-stu-id="e31bc-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e31bc-135">id</span><span class="sxs-lookup"><span data-stu-id="e31bc-135">id</span></span>|<span data-ttu-id="e31bc-136">String</span><span class="sxs-lookup"><span data-stu-id="e31bc-136">String</span></span>|<span data-ttu-id="e31bc-137">打印机的 GUID。</span><span class="sxs-lookup"><span data-stu-id="e31bc-137">The printer's GUID.</span></span> <span data-ttu-id="e31bc-138">只读。</span><span class="sxs-lookup"><span data-stu-id="e31bc-138">Read-only.</span></span>|
|<span data-ttu-id="e31bc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e31bc-139">createdDateTime</span></span>|<span data-ttu-id="e31bc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e31bc-140">DateTimeOffset</span></span>|<span data-ttu-id="e31bc-141">创建作业时的日期时间Offset。</span><span class="sxs-lookup"><span data-stu-id="e31bc-141">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="e31bc-142">只读。</span><span class="sxs-lookup"><span data-stu-id="e31bc-142">Read-only.</span></span>|
|<span data-ttu-id="e31bc-143">状态</span><span class="sxs-lookup"><span data-stu-id="e31bc-143">status</span></span>|[<span data-ttu-id="e31bc-144">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="e31bc-144">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="e31bc-145">打印作业的状态。</span><span class="sxs-lookup"><span data-stu-id="e31bc-145">The status of the print job.</span></span> <span data-ttu-id="e31bc-146">只读。</span><span class="sxs-lookup"><span data-stu-id="e31bc-146">Read-only.</span></span>|
|<span data-ttu-id="e31bc-147">configuration</span><span class="sxs-lookup"><span data-stu-id="e31bc-147">configuration</span></span>|[<span data-ttu-id="e31bc-148">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="e31bc-148">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="e31bc-149">打印机用于打印作业的一组设置。</span><span class="sxs-lookup"><span data-stu-id="e31bc-149">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="e31bc-150">isFetchable</span><span class="sxs-lookup"><span data-stu-id="e31bc-150">isFetchable</span></span>|<span data-ttu-id="e31bc-151">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="e31bc-151">Edm.Boolean</span></span>|<span data-ttu-id="e31bc-152">如果为 true，则打印机可以提取文档。</span><span class="sxs-lookup"><span data-stu-id="e31bc-152">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="e31bc-153">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="e31bc-153">redirectedFrom</span></span>|<span data-ttu-id="e31bc-154">Edm.String</span><span class="sxs-lookup"><span data-stu-id="e31bc-154">Edm.String</span></span>|<span data-ttu-id="e31bc-155">如果作业已从另一台打印机重定向，则包含源作业 URL。</span><span class="sxs-lookup"><span data-stu-id="e31bc-155">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="e31bc-156">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="e31bc-156">redirectedTo</span></span>|<span data-ttu-id="e31bc-157">Edm.String</span><span class="sxs-lookup"><span data-stu-id="e31bc-157">Edm.String</span></span>|<span data-ttu-id="e31bc-158">如果作业已重定向到另一台打印机，则包含目标作业 URL。</span><span class="sxs-lookup"><span data-stu-id="e31bc-158">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|
|<span data-ttu-id="e31bc-159">createdBy</span><span class="sxs-lookup"><span data-stu-id="e31bc-159">createdBy</span></span>|[<span data-ttu-id="e31bc-160">userIdentity</span><span class="sxs-lookup"><span data-stu-id="e31bc-160">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="e31bc-161">只读。</span><span class="sxs-lookup"><span data-stu-id="e31bc-161">Read-only.</span></span> <span data-ttu-id="e31bc-162">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e31bc-162">Nullable.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e31bc-163">关系</span><span class="sxs-lookup"><span data-stu-id="e31bc-163">Relationships</span></span>
|<span data-ttu-id="e31bc-164">关系</span><span class="sxs-lookup"><span data-stu-id="e31bc-164">Relationship</span></span>|<span data-ttu-id="e31bc-165">类型</span><span class="sxs-lookup"><span data-stu-id="e31bc-165">Type</span></span>|<span data-ttu-id="e31bc-166">Description</span><span class="sxs-lookup"><span data-stu-id="e31bc-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e31bc-167">documents</span><span class="sxs-lookup"><span data-stu-id="e31bc-167">documents</span></span>|<span data-ttu-id="e31bc-168">[printDocument](printdocument.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e31bc-168">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="e31bc-169">只读。</span><span class="sxs-lookup"><span data-stu-id="e31bc-169">Read-only.</span></span>|
|<span data-ttu-id="e31bc-170">tasks</span><span class="sxs-lookup"><span data-stu-id="e31bc-170">tasks</span></span>|<span data-ttu-id="e31bc-171">[printTask](printtask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e31bc-171">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="e31bc-172">此打印作业触发的 [printTasks](printtask.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="e31bc-172">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e31bc-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e31bc-173">JSON representation</span></span>
<span data-ttu-id="e31bc-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e31bc-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printJob",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJob",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "status": {
    "@odata.type": "microsoft.graph.printJobStatus"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "configuration": {
    "@odata.type": "microsoft.graph.printJobConfiguration"
  },
  "redirectedTo": "String",
  "redirectedFrom": "String",
  "isFetchable": "Boolean"
}
```

