---
title: printTask 资源类型
description: 表示正在执行或已作为通用 Print 事件的结果执行的任务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: fb41bc68112aa04e1eea825d45982f2f3f0db48c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973790"
---
# <a name="printtask-resource-type"></a><span data-ttu-id="ac15b-103">printTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac15b-103">printTask resource type</span></span>

<span data-ttu-id="ac15b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac15b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac15b-105">表示正在执行或已作为通用 Print 事件的结果执行的任务。</span><span class="sxs-lookup"><span data-stu-id="ac15b-105">Represents a task that is executing or has been executed as a result of a Universal Print event.</span></span>

<span data-ttu-id="ac15b-106">有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅 [扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="ac15b-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="ac15b-107">方法</span><span class="sxs-lookup"><span data-stu-id="ac15b-107">Methods</span></span>

| <span data-ttu-id="ac15b-108">方法</span><span class="sxs-lookup"><span data-stu-id="ac15b-108">Method</span></span>       | <span data-ttu-id="ac15b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ac15b-109">Return Type</span></span> | <span data-ttu-id="ac15b-110">说明</span><span class="sxs-lookup"><span data-stu-id="ac15b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ac15b-111">从 printTaskDefintion 中列出 () </span><span class="sxs-lookup"><span data-stu-id="ac15b-111">List (from printTaskDefintion)</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="ac15b-112">printTask</span><span class="sxs-lookup"><span data-stu-id="ac15b-112">printTask</span></span>](printtask.md) | <span data-ttu-id="ac15b-113">获取基于特定 printTaskDefinition 创建的任务的列表。</span><span class="sxs-lookup"><span data-stu-id="ac15b-113">Get a list of tasks that have been created based on a particular printTaskDefinition.</span></span> <span data-ttu-id="ac15b-114">该列表包含当前正在运行的任务和最近完成的任务。</span><span class="sxs-lookup"><span data-stu-id="ac15b-114">The list includes currently running tasks and recently completed tasks.</span></span> |

## <a name="properties"></a><span data-ttu-id="ac15b-115">属性</span><span class="sxs-lookup"><span data-stu-id="ac15b-115">Properties</span></span>
| <span data-ttu-id="ac15b-116">属性</span><span class="sxs-lookup"><span data-stu-id="ac15b-116">Property</span></span>     | <span data-ttu-id="ac15b-117">类型</span><span class="sxs-lookup"><span data-stu-id="ac15b-117">Type</span></span>        | <span data-ttu-id="ac15b-118">说明</span><span class="sxs-lookup"><span data-stu-id="ac15b-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac15b-119">id</span><span class="sxs-lookup"><span data-stu-id="ac15b-119">id</span></span>|<span data-ttu-id="ac15b-120">String</span><span class="sxs-lookup"><span data-stu-id="ac15b-120">String</span></span>|<span data-ttu-id="ac15b-121">PrintTask 的标识符。</span><span class="sxs-lookup"><span data-stu-id="ac15b-121">The printTask's identifier.</span></span> <span data-ttu-id="ac15b-122">只读。</span><span class="sxs-lookup"><span data-stu-id="ac15b-122">Read-only.</span></span>|
|<span data-ttu-id="ac15b-123">状态</span><span class="sxs-lookup"><span data-stu-id="ac15b-123">status</span></span>|[<span data-ttu-id="ac15b-124">printTaskStatus</span><span class="sxs-lookup"><span data-stu-id="ac15b-124">printTaskStatus</span></span>](printtaskstatus.md)|<span data-ttu-id="ac15b-125">此 printTask 的当前执行状态。</span><span class="sxs-lookup"><span data-stu-id="ac15b-125">The current execution status of this printTask.</span></span> <span data-ttu-id="ac15b-126">**在处理完成时，调用应用程序负责更新此状态，除非相关的 printJob 已重定向到另一台打印机。**</span><span class="sxs-lookup"><span data-stu-id="ac15b-126">**The calling application is responsible for updating this status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="ac15b-127">若未能报告完成，则会导致相关打印作业被阻止打印，并最终删除。</span><span class="sxs-lookup"><span data-stu-id="ac15b-127">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |
|<span data-ttu-id="ac15b-128">parentUrl</span><span class="sxs-lookup"><span data-stu-id="ac15b-128">parentUrl</span></span>|<span data-ttu-id="ac15b-129">String</span><span class="sxs-lookup"><span data-stu-id="ac15b-129">String</span></span>|<span data-ttu-id="ac15b-130">触发此任务的打印实体的 URL。</span><span class="sxs-lookup"><span data-stu-id="ac15b-130">The URL for the print entity that triggered this task.</span></span> <span data-ttu-id="ac15b-131">例如，`https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`。</span><span class="sxs-lookup"><span data-stu-id="ac15b-131">For example, `https://graph.microsoft.com/beta/print/printers/{printerId}/jobs/{jobId}`.</span></span> <span data-ttu-id="ac15b-132">只读。</span><span class="sxs-lookup"><span data-stu-id="ac15b-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac15b-133">关系</span><span class="sxs-lookup"><span data-stu-id="ac15b-133">Relationships</span></span>
| <span data-ttu-id="ac15b-134">关系</span><span class="sxs-lookup"><span data-stu-id="ac15b-134">Relationship</span></span> | <span data-ttu-id="ac15b-135">类型</span><span class="sxs-lookup"><span data-stu-id="ac15b-135">Type</span></span>        | <span data-ttu-id="ac15b-136">说明</span><span class="sxs-lookup"><span data-stu-id="ac15b-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac15b-137">触发</span><span class="sxs-lookup"><span data-stu-id="ac15b-137">trigger</span></span>|[<span data-ttu-id="ac15b-138">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="ac15b-138">printTaskTrigger</span></span>](printtasktrigger.md)|<span data-ttu-id="ac15b-139">触发此任务的执行的 printTaskTrigger。</span><span class="sxs-lookup"><span data-stu-id="ac15b-139">The printTaskTrigger that triggered this task's execution.</span></span> <span data-ttu-id="ac15b-140">只读。</span><span class="sxs-lookup"><span data-stu-id="ac15b-140">Read-only.</span></span>|
|<span data-ttu-id="ac15b-141">定义</span><span class="sxs-lookup"><span data-stu-id="ac15b-141">definition</span></span>|[<span data-ttu-id="ac15b-142">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="ac15b-142">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="ac15b-143">用于创建此任务的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="ac15b-143">The printTaskDefinition that was used to create this task.</span></span> <span data-ttu-id="ac15b-144">只读。</span><span class="sxs-lookup"><span data-stu-id="ac15b-144">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac15b-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac15b-145">JSON representation</span></span>

<span data-ttu-id="ac15b-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac15b-146">The following is a JSON representation of the resource.</span></span>

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


