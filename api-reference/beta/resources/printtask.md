---
title: printTask 资源类型
description: 表示由于通用 Print 事件而正在执行或已执行的任务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c684ff64aa4c3667214b61b70a422690381525b3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766299"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="a4fe2-103">printTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4fe2-103">printTask resource type</span></span>

<span data-ttu-id="a4fe2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4fe2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4fe2-105">表示由于通用 Print 事件而正在执行或已执行的任务。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="a4fe2-106">有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="a4fe2-107">方法</span><span class="sxs-lookup"><span data-stu-id="a4fe2-107">Methods</span></span>

| <span data-ttu-id="a4fe2-108">方法</span><span class="sxs-lookup"><span data-stu-id="a4fe2-108">Method</span></span>       | <span data-ttu-id="a4fe2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a4fe2-109">Return Type</span></span> | <span data-ttu-id="a4fe2-110">说明</span><span class="sxs-lookup"><span data-stu-id="a4fe2-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a4fe2-111">列出 (printTaskDefintion) </span><span class="sxs-lookup"><span data-stu-id="a4fe2-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="a4fe2-112">printTask</span><span class="sxs-lookup"><span data-stu-id="a4fe2-112">printTask</span></span>](printtask.md) | <span data-ttu-id="a4fe2-113">获取基于特定 printTaskDefinition 创建的任务列表。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="a4fe2-114">该列表包括当前运行的任务和最近完成的任务。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-114">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="a4fe2-115">Get</span><span class="sxs-lookup"><span data-stu-id="a4fe2-115">Get</span></span>](../api/printtask-get.md) | [<span data-ttu-id="a4fe2-116">printTask</span><span class="sxs-lookup"><span data-stu-id="a4fe2-116">printTask</span></span>](printtask.md) | <span data-ttu-id="a4fe2-117">获取有关打印任务的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-117">Get details about a print task.</span></span> |
| [<span data-ttu-id="a4fe2-118">更新</span><span class="sxs-lookup"><span data-stu-id="a4fe2-118">Update</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="a4fe2-119">printTask</span><span class="sxs-lookup"><span data-stu-id="a4fe2-119">printTask</span></span>](printtask.md) | <span data-ttu-id="a4fe2-120">更新打印任务。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-120">Updates a print task.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4fe2-121">属性</span><span class="sxs-lookup"><span data-stu-id="a4fe2-121">Properties</span></span>
| <span data-ttu-id="a4fe2-122">属性</span><span class="sxs-lookup"><span data-stu-id="a4fe2-122">Property</span></span>     | <span data-ttu-id="a4fe2-123">类型</span><span class="sxs-lookup"><span data-stu-id="a4fe2-123">Type</span></span>        | <span data-ttu-id="a4fe2-124">说明</span><span class="sxs-lookup"><span data-stu-id="a4fe2-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4fe2-125">id</span><span class="sxs-lookup"><span data-stu-id="a4fe2-125">id</span></span>|<span data-ttu-id="a4fe2-126">String</span><span class="sxs-lookup"><span data-stu-id="a4fe2-126">String</span></span>|<span data-ttu-id="a4fe2-127">printTask 的标识符。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-127">The printTask's identifier.</span></span> <span data-ttu-id="a4fe2-128">只读。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-128">Read-only.</span></span>|
|<span data-ttu-id="a4fe2-129">状态</span><span class="sxs-lookup"><span data-stu-id="a4fe2-129">status</span></span>|[<span data-ttu-id="a4fe2-130">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="a4fe2-130">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="a4fe2-131">此 printTask 的当前执行状态。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-131">The current execution status of this printTask.</span></span> <span data-ttu-id="a4fe2-132">**除非相关 printJob 已重定向到另一台打印机，否则调用应用程序负责在处理完成时更新此状态。**</span><span class="sxs-lookup"><span data-stu-id="a4fe2-132">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="a4fe2-133">如果未能报告完成，将导致相关打印作业被阻止打印并最终被删除。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-133">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="a4fe2-134">parentUrl</span><span class="sxs-lookup"><span data-stu-id="a4fe2-134">parentUrl</span></span>|<span data-ttu-id="a4fe2-135">String</span><span class="sxs-lookup"><span data-stu-id="a4fe2-135">String</span></span>|<span data-ttu-id="a4fe2-136">触发此任务的打印实体的 URL。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-136">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="a4fe2-137">例如，`https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-137">For example, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="a4fe2-138">只读。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4fe2-139">关系</span><span class="sxs-lookup"><span data-stu-id="a4fe2-139">Relationships</span></span>
| <span data-ttu-id="a4fe2-140">关系</span><span class="sxs-lookup"><span data-stu-id="a4fe2-140">Relationship</span></span> | <span data-ttu-id="a4fe2-141">类型</span><span class="sxs-lookup"><span data-stu-id="a4fe2-141">Type</span></span>        | <span data-ttu-id="a4fe2-142">说明</span><span class="sxs-lookup"><span data-stu-id="a4fe2-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4fe2-143">trigger</span><span class="sxs-lookup"><span data-stu-id="a4fe2-143">trigger</span></span>|[<span data-ttu-id="a4fe2-144">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="a4fe2-144">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="a4fe2-145">触发此任务执行的 printTaskTrigger。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-145">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="a4fe2-146">只读。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-146">Read-only.</span></span>|
|<span data-ttu-id="a4fe2-147">definition</span><span class="sxs-lookup"><span data-stu-id="a4fe2-147">definition</span></span>|[<span data-ttu-id="a4fe2-148">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="a4fe2-148">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="a4fe2-149">用于创建此任务的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-149">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="a4fe2-150">只读。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-150">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4fe2-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4fe2-151">JSON representation</span></span>

<span data-ttu-id="a4fe2-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4fe2-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTask",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.printTaskStatus"},
  "parentUrl": "String",
  "trigger": {"@odata.type": "microsoft.graph.printTaskTrigger"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


