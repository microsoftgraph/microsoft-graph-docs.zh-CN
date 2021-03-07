---
title: printTaskDefinition 资源类型
description: 表示在通用打印中发生各种事件时可以触发的任务。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a8a8c78d1e165dfe0f9417c5aa052f9f0b2383b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517313"
---
# <a name="printtaskdefinition-resource-type"></a><span data-ttu-id="5fa31-103">printTaskDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fa31-103">printTaskDefinition resource type</span></span>

<span data-ttu-id="5fa31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fa31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5fa31-105">表示在通用打印中发生各种事件时可以触发的任务的抽象定义。</span><span class="sxs-lookup"><span data-stu-id="5fa31-105">Represents an abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>

<span data-ttu-id="5fa31-106">有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="5fa31-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

<span data-ttu-id="5fa31-107">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="5fa31-107">This resource supports:</span></span>
* <span data-ttu-id="5fa31-108">[订阅更改通知](/graph/universal-print-webhook-notifications)。</span><span class="sxs-lookup"><span data-stu-id="5fa31-108">[Subscribing to change notifications](/graph/universal-print-webhook-notifications).</span></span>

## <a name="methods"></a><span data-ttu-id="5fa31-109">Methods</span><span class="sxs-lookup"><span data-stu-id="5fa31-109">Methods</span></span>
| <span data-ttu-id="5fa31-110">方法</span><span class="sxs-lookup"><span data-stu-id="5fa31-110">Method</span></span>       | <span data-ttu-id="5fa31-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fa31-111">Return Type</span></span> | <span data-ttu-id="5fa31-112">Description</span><span class="sxs-lookup"><span data-stu-id="5fa31-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5fa31-113">List</span><span class="sxs-lookup"><span data-stu-id="5fa31-113">List</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="5fa31-114">[printTaskDefinition](printtaskdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fa31-114">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="5fa31-115">获取在通用打印中创建的 printTaskDefinitions 的完整列表。</span><span class="sxs-lookup"><span data-stu-id="5fa31-115">Get a complete list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="5fa31-116">创建</span><span class="sxs-lookup"><span data-stu-id="5fa31-116">Create</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="5fa31-117">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5fa31-117">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="5fa31-118">创建新的 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="5fa31-118">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="5fa31-119">更新</span><span class="sxs-lookup"><span data-stu-id="5fa31-119">Update</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="5fa31-120">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="5fa31-120">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="5fa31-121">更新 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="5fa31-121">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="5fa31-122">删除</span><span class="sxs-lookup"><span data-stu-id="5fa31-122">Delete</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="5fa31-123">无</span><span class="sxs-lookup"><span data-stu-id="5fa31-123">None</span></span> | <span data-ttu-id="5fa31-124">删除 printTaskDefinition。</span><span class="sxs-lookup"><span data-stu-id="5fa31-124">Delete a printTaskDefinition.</span></span> |
| [<span data-ttu-id="5fa31-125">列出任务</span><span class="sxs-lookup"><span data-stu-id="5fa31-125">List tasks</span></span>](../api/printtaskdefinition-list-tasks.md) | [<span data-ttu-id="5fa31-126">printTask</span><span class="sxs-lookup"><span data-stu-id="5fa31-126">printTask</span></span>](printtask.md) | <span data-ttu-id="5fa31-127">获取已基于此定义创建的任务列表。</span><span class="sxs-lookup"><span data-stu-id="5fa31-127">Get a list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="5fa31-128">该列表包括当前运行的任务和最近完成的任务。</span><span class="sxs-lookup"><span data-stu-id="5fa31-128">The list includes currently running tasks and recently completed tasks.</span></span> |
| [<span data-ttu-id="5fa31-129">获取任务</span><span class="sxs-lookup"><span data-stu-id="5fa31-129">Get task</span></span>](../api/printtask-get.md) | [<span data-ttu-id="5fa31-130">printTask</span><span class="sxs-lookup"><span data-stu-id="5fa31-130">printTask</span></span>](printtask.md) | <span data-ttu-id="5fa31-131">获取已基于此定义创建的任务。</span><span class="sxs-lookup"><span data-stu-id="5fa31-131">Gets a task that has been created based on this definition.</span></span> |
| [<span data-ttu-id="5fa31-132">更新任务</span><span class="sxs-lookup"><span data-stu-id="5fa31-132">Update task</span></span>](../api/printtaskdefinition-update-task.md) | [<span data-ttu-id="5fa31-133">printTask</span><span class="sxs-lookup"><span data-stu-id="5fa31-133">printTask</span></span>](printtask.md) | <span data-ttu-id="5fa31-134">更新已基于此定义创建的任务。</span><span class="sxs-lookup"><span data-stu-id="5fa31-134">Update a task that has been created based on this definition.</span></span> <span data-ttu-id="5fa31-135">**注册任务触发器的应用程序负责在处理完成后更新任务状态，除非相关 printJob 已重定向到另一台打印机。**</span><span class="sxs-lookup"><span data-stu-id="5fa31-135">**Applications that register task triggers are responsible for updating task status when processing is finished, unless the related printJob has been redirected to another printer.**</span></span> <span data-ttu-id="5fa31-136">未能报告完成操作将导致相关打印作业被阻止打印并最终被删除。</span><span class="sxs-lookup"><span data-stu-id="5fa31-136">Failure to report completion will result in the related print job being blocked from printing and eventually deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="5fa31-137">属性</span><span class="sxs-lookup"><span data-stu-id="5fa31-137">Properties</span></span>
|<span data-ttu-id="5fa31-138">属性</span><span class="sxs-lookup"><span data-stu-id="5fa31-138">Property</span></span>|<span data-ttu-id="5fa31-139">类型</span><span class="sxs-lookup"><span data-stu-id="5fa31-139">Type</span></span>|<span data-ttu-id="5fa31-140">说明</span><span class="sxs-lookup"><span data-stu-id="5fa31-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fa31-141">id</span><span class="sxs-lookup"><span data-stu-id="5fa31-141">id</span></span>|<span data-ttu-id="5fa31-142">String</span><span class="sxs-lookup"><span data-stu-id="5fa31-142">String</span></span>|<span data-ttu-id="5fa31-143">printTaskDefinition 的标识符。</span><span class="sxs-lookup"><span data-stu-id="5fa31-143">The printTaskDefinition's identifier.</span></span> <span data-ttu-id="5fa31-144">只读。</span><span class="sxs-lookup"><span data-stu-id="5fa31-144">Read-only.</span></span>|
|<span data-ttu-id="5fa31-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5fa31-145">displayName</span></span>|<span data-ttu-id="5fa31-146">String</span><span class="sxs-lookup"><span data-stu-id="5fa31-146">String</span></span>|<span data-ttu-id="5fa31-147">printTaskDefinition 的名称。</span><span class="sxs-lookup"><span data-stu-id="5fa31-147">The name of the printTaskDefinition.</span></span>|
|<span data-ttu-id="5fa31-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="5fa31-148">createdBy</span></span>|[<span data-ttu-id="5fa31-149">appIdentity</span><span class="sxs-lookup"><span data-stu-id="5fa31-149">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="5fa31-150">创建 printTaskDefinition 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="5fa31-150">The application that created the printTaskDefinition.</span></span> <span data-ttu-id="5fa31-151">只读。</span><span class="sxs-lookup"><span data-stu-id="5fa31-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fa31-152">关系</span><span class="sxs-lookup"><span data-stu-id="5fa31-152">Relationships</span></span>
|<span data-ttu-id="5fa31-153">关系</span><span class="sxs-lookup"><span data-stu-id="5fa31-153">Relationship</span></span>|<span data-ttu-id="5fa31-154">类型</span><span class="sxs-lookup"><span data-stu-id="5fa31-154">Type</span></span>|<span data-ttu-id="5fa31-155">Description</span><span class="sxs-lookup"><span data-stu-id="5fa31-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fa31-156">tasks</span><span class="sxs-lookup"><span data-stu-id="5fa31-156">tasks</span></span>|<span data-ttu-id="5fa31-157">[printTask](printtask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fa31-157">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="5fa31-158">已基于此定义创建的任务列表。</span><span class="sxs-lookup"><span data-stu-id="5fa31-158">A list of tasks that have been created based on this definition.</span></span> <span data-ttu-id="5fa31-159">该列表包括当前运行的任务和最近完成的任务。</span><span class="sxs-lookup"><span data-stu-id="5fa31-159">The list includes currently running tasks and recently completed tasks.</span></span> <span data-ttu-id="5fa31-160">只读。</span><span class="sxs-lookup"><span data-stu-id="5fa31-160">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fa31-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fa31-161">JSON representation</span></span>
<span data-ttu-id="5fa31-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fa31-162">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.appIdentity"
  }
}
```

