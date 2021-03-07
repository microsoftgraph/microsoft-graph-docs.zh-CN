---
title: printTask 资源类型
description: 表示由于通用打印事件而正在执行或已执行的任务。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2026706ec46a2408d20231add8203d2f5a622c96
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516986"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="b76eb-103">printTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="b76eb-103">printTask resource type</span></span>

<span data-ttu-id="b76eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b76eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="b76eb-105">表示由于通用打印事件而正在执行或已执行的任务。</span><span class="sxs-lookup"><span data-stu-id="b76eb-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="b76eb-106">有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="b76eb-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="b76eb-107">Methods</span><span class="sxs-lookup"><span data-stu-id="b76eb-107">Methods</span></span>
|<span data-ttu-id="b76eb-108">方法</span><span class="sxs-lookup"><span data-stu-id="b76eb-108">Method</span></span>|<span data-ttu-id="b76eb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b76eb-109">Return type</span></span>|<span data-ttu-id="b76eb-110">Description</span><span class="sxs-lookup"><span data-stu-id="b76eb-110">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="b76eb-111">列出 (taskDefintion) </span><span class="sxs-lookup"><span data-stu-id="b76eb-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="b76eb-112">printTask</span><span class="sxs-lookup"><span data-stu-id="b76eb-112">printTask</span></span>](printtask.md) | <span data-ttu-id="b76eb-113">获取基于特定 printTaskDefinition 创建的任务列表。</span><span class="sxs-lookup"><span data-stu-id="b76eb-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="b76eb-114">该列表包括当前运行的任务和最近完成的任务。</span><span class="sxs-lookup"><span data-stu-id="b76eb-114">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="b76eb-115">获取</span><span class="sxs-lookup"><span data-stu-id="b76eb-115">Get</span></span>](../api/printtask-get.md) | [<span data-ttu-id="b76eb-116">printTask</span><span class="sxs-lookup"><span data-stu-id="b76eb-116">printTask</span></span>](printtask.md) | <span data-ttu-id="b76eb-117">获取有关打印任务的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b76eb-117">Get details about a print task.</span></span> |
| [<span data-ttu-id="b76eb-118">更新</span><span class="sxs-lookup"><span data-stu-id="b76eb-118">Update</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="b76eb-119">printTask</span><span class="sxs-lookup"><span data-stu-id="b76eb-119">printTask</span></span>](printtask.md) | <span data-ttu-id="b76eb-120">更新打印任务。</span><span class="sxs-lookup"><span data-stu-id="b76eb-120">Updates a print task.</span></span> |

## <a name="properties"></a><span data-ttu-id="b76eb-121">属性</span><span class="sxs-lookup"><span data-stu-id="b76eb-121">Properties</span></span>
|<span data-ttu-id="b76eb-122">属性</span><span class="sxs-lookup"><span data-stu-id="b76eb-122">Property</span></span>|<span data-ttu-id="b76eb-123">类型</span><span class="sxs-lookup"><span data-stu-id="b76eb-123">Type</span></span>|<span data-ttu-id="b76eb-124">说明</span><span class="sxs-lookup"><span data-stu-id="b76eb-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76eb-125">id</span><span class="sxs-lookup"><span data-stu-id="b76eb-125">id</span></span>|<span data-ttu-id="b76eb-126">String</span><span class="sxs-lookup"><span data-stu-id="b76eb-126">String</span></span>|<span data-ttu-id="b76eb-127">printTask 的标识符。</span><span class="sxs-lookup"><span data-stu-id="b76eb-127">The printTask's identifier.</span></span> <span data-ttu-id="b76eb-128">只读。</span><span class="sxs-lookup"><span data-stu-id="b76eb-128">Read-only.</span></span>|
|<span data-ttu-id="b76eb-129">状态</span><span class="sxs-lookup"><span data-stu-id="b76eb-129">status</span></span>|[<span data-ttu-id="b76eb-130">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="b76eb-130">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="b76eb-131">此 printTask 的当前执行状态。</span><span class="sxs-lookup"><span data-stu-id="b76eb-131">The current execution status of this printTask.</span></span> <span data-ttu-id="b76eb-132">**除非相关 printJob 已重定向到另一台打印机，否则调用应用程序负责在处理完成时更新此状态。**</span><span class="sxs-lookup"><span data-stu-id="b76eb-132">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="b76eb-133">未能报告完成操作将导致相关打印作业被阻止打印并最终被删除。</span><span class="sxs-lookup"><span data-stu-id="b76eb-133">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="b76eb-134">parentUrl</span><span class="sxs-lookup"><span data-stu-id="b76eb-134">parentUrl</span></span>|<span data-ttu-id="b76eb-135">String</span><span class="sxs-lookup"><span data-stu-id="b76eb-135">String</span></span>|<span data-ttu-id="b76eb-136">触发此任务的打印实体的 URL。</span><span class="sxs-lookup"><span data-stu-id="b76eb-136">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="b76eb-137">例如，`https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`。</span><span class="sxs-lookup"><span data-stu-id="b76eb-137">For example, `https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="b76eb-138">只读。</span><span class="sxs-lookup"><span data-stu-id="b76eb-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b76eb-139">关系</span><span class="sxs-lookup"><span data-stu-id="b76eb-139">Relationships</span></span>
|<span data-ttu-id="b76eb-140">关系</span><span class="sxs-lookup"><span data-stu-id="b76eb-140">Relationship</span></span>|<span data-ttu-id="b76eb-141">类型</span><span class="sxs-lookup"><span data-stu-id="b76eb-141">Type</span></span>|<span data-ttu-id="b76eb-142">Description</span><span class="sxs-lookup"><span data-stu-id="b76eb-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76eb-143">trigger</span><span class="sxs-lookup"><span data-stu-id="b76eb-143">trigger</span></span>|[<span data-ttu-id="b76eb-144">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="b76eb-144">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="b76eb-145">触发此任务执行的 printTaskTrigger。</span><span class="sxs-lookup"><span data-stu-id="b76eb-145">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="b76eb-146">只读。</span><span class="sxs-lookup"><span data-stu-id="b76eb-146">Read-only.</span></span>|
|<span data-ttu-id="b76eb-147">definition</span><span class="sxs-lookup"><span data-stu-id="b76eb-147">definition</span></span>|[<span data-ttu-id="b76eb-148">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="b76eb-148">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="b76eb-149">用于创建此任务的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="b76eb-149">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="b76eb-150">只读。</span><span class="sxs-lookup"><span data-stu-id="b76eb-150">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b76eb-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b76eb-151">JSON representation</span></span>
<span data-ttu-id="b76eb-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b76eb-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTask",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTask",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printTaskStatus"
  },
  "parentUrl": "String"
}
```

