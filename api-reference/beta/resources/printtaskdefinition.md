---
title: printTaskDefinition 资源类型
description: 表示在通用打印中发生各种事件时可触发的任务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 013d2756455abebc0f20bbe5a1d186a0a4d65648
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091576"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="e515a-103">printTaskDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="e515a-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="e515a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e515a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e515a-105">表示在通用打印中发生各种事件时可触发的任务的抽象定义。</span><span class="sxs-lookup"><span data-stu-id="e515a-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="e515a-106">有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="e515a-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="e515a-107">方法</span><span class="sxs-lookup"><span data-stu-id="e515a-107">Methods</span></span>

| <span data-ttu-id="e515a-108">方法</span><span class="sxs-lookup"><span data-stu-id="e515a-108">Method</span></span>       | <span data-ttu-id="e515a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e515a-109">Return Type</span></span> | <span data-ttu-id="e515a-110">说明</span><span class="sxs-lookup"><span data-stu-id="e515a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e515a-111">List</span><span class="sxs-lookup"><span data-stu-id="e515a-111">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="e515a-112">[printTaskDefinition](printtaskdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="e515a-112">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="e515a-113">获取在通用打印中创建的 printTaskDefinitions 的完整列表。</span><span class="sxs-lookup"><span data-stu-id="e515a-113">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="e515a-114">创建</span><span class="sxs-lookup"><span data-stu-id="e515a-114">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="e515a-115">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="e515a-115">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="e515a-116">创建新的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="e515a-116">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="e515a-117">更新</span><span class="sxs-lookup"><span data-stu-id="e515a-117">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="e515a-118">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="e515a-118">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="e515a-119">更新 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="e515a-119">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="e515a-120">删除</span><span class="sxs-lookup"><span data-stu-id="e515a-120">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="e515a-121">无</span><span class="sxs-lookup"><span data-stu-id="e515a-121">None</span></span> | <span data-ttu-id="e515a-122">删除 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="e515a-122">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="e515a-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="e515a-123">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="e515a-124">printTask</span><span class="sxs-lookup"><span data-stu-id="e515a-124">printTask</span></span>](printtask.md) | <span data-ttu-id="e515a-125">获取基于此定义创建的任务的列表。</span><span class="sxs-lookup"><span data-stu-id="e515a-125">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="e515a-126">该列表包含当前正在运行的任务和最近完成的任务。</span><span class="sxs-lookup"><span data-stu-id="e515a-126">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="e515a-127">获取任务</span><span class="sxs-lookup"><span data-stu-id="e515a-127">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="e515a-128">printTask</span><span class="sxs-lookup"><span data-stu-id="e515a-128">printTask</span></span>](printtask.md) | <span data-ttu-id="e515a-129">获取已基于此定义创建的任务。</span><span class="sxs-lookup"><span data-stu-id="e515a-129">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="e515a-130">更新任务</span><span class="sxs-lookup"><span data-stu-id="e515a-130">Update task</span></span>](../api/printtaskdefinition-update-task.md) | <span data-ttu-id="e515a-131">无</span><span class="sxs-lookup"><span data-stu-id="e515a-131">None</span></span> | <span data-ttu-id="e515a-132">更新基于此定义创建的任务。</span><span class="sxs-lookup"><span data-stu-id="e515a-132">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="e515a-133">**注册任务触发器的应用程序负责在处理完成后更新任务状态，除非相关的 printJob 已重定向到另一台打印机。**</span><span class="sxs-lookup"><span data-stu-id="e515a-133">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="e515a-134">若未能报告完成，则会导致相关打印作业被阻止打印，并最终删除。</span><span class="sxs-lookup"><span data-stu-id="e515a-134">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="e515a-135">属性</span><span class="sxs-lookup"><span data-stu-id="e515a-135">Properties</span></span>
| <span data-ttu-id="e515a-136">属性</span><span class="sxs-lookup"><span data-stu-id="e515a-136">Property</span></span>     | <span data-ttu-id="e515a-137">类型</span><span class="sxs-lookup"><span data-stu-id="e515a-137">Type</span></span>        | <span data-ttu-id="e515a-138">说明</span><span class="sxs-lookup"><span data-stu-id="e515a-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e515a-139">id</span><span class="sxs-lookup"><span data-stu-id="e515a-139">id</span></span>|<span data-ttu-id="e515a-140">String</span><span class="sxs-lookup"><span data-stu-id="e515a-140">String</span></span>|<span data-ttu-id="e515a-141">PrintTaskDefinition 的标识符。</span><span class="sxs-lookup"><span data-stu-id="e515a-141">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="e515a-142">只读。</span><span class="sxs-lookup"><span data-stu-id="e515a-142">Read-only.</span></span>|
|<span data-ttu-id="e515a-143">displayName</span><span class="sxs-lookup"><span data-stu-id="e515a-143">displayName</span></span>|<span data-ttu-id="e515a-144">String</span><span class="sxs-lookup"><span data-stu-id="e515a-144">String</span></span>|<span data-ttu-id="e515a-145">PrintTaskDefinition 的名称。</span><span class="sxs-lookup"><span data-stu-id="e515a-145">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="e515a-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="e515a-146">createdBy</span></span>|[<span data-ttu-id="e515a-147">appIdentity</span><span class="sxs-lookup"><span data-stu-id="e515a-147">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="e515a-148">创建 printTaskDefinition 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e515a-148">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="e515a-149">只读。</span><span class="sxs-lookup"><span data-stu-id="e515a-149">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e515a-150">关系</span><span class="sxs-lookup"><span data-stu-id="e515a-150">Relationships</span></span>
| <span data-ttu-id="e515a-151">关系</span><span class="sxs-lookup"><span data-stu-id="e515a-151">Relationship</span></span> | <span data-ttu-id="e515a-152">类型</span><span class="sxs-lookup"><span data-stu-id="e515a-152">Type</span></span>        | <span data-ttu-id="e515a-153">说明</span><span class="sxs-lookup"><span data-stu-id="e515a-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e515a-154">tasks</span><span class="sxs-lookup"><span data-stu-id="e515a-154">tasks</span></span>|<span data-ttu-id="e515a-155">[printTask](printtask.md)集合</span><span class="sxs-lookup"><span data-stu-id="e515a-155">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="e515a-156">基于此定义创建的任务的列表。</span><span class="sxs-lookup"><span data-stu-id="e515a-156">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="e515a-157">该列表包含当前正在运行的任务和最近完成的任务。</span><span class="sxs-lookup"><span data-stu-id="e515a-157">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="e515a-158">只读。</span><span class="sxs-lookup"><span data-stu-id="e515a-158">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e515a-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e515a-159">JSON representation</span></span>

<span data-ttu-id="e515a-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e515a-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {"@odata.type": "microsoft.graph.appIdentity"},
  "tasks": [{"@odata.type": "microsoft.graph.printTask"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->