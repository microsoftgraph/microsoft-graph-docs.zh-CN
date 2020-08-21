---
title: todoTaskList 资源类型
description: Microsoft To Do 中的一个或多个 todoTask 资源的列表。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34f90329fc6ca4d5e12ff2f2b191819b88f895b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849869"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="66341-103">todoTaskList 资源类型</span><span class="sxs-lookup"><span data-stu-id="66341-103">todoTaskList resource type</span></span>

<span data-ttu-id="66341-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66341-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66341-105">Microsoft To Do 中的一个或多个 [todoTask 资源](./todotask.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="66341-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="66341-106">In To Do， there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span><span class="sxs-lookup"><span data-stu-id="66341-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="66341-107">但是，你可以创建其他任务列表。</span><span class="sxs-lookup"><span data-stu-id="66341-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="66341-108">该资源支持</span><span class="sxs-lookup"><span data-stu-id="66341-108">This resource supports</span></span>
* <span data-ttu-id="66341-109">将数据作为开放扩展添加到 [自定义属性](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="66341-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="66341-110">使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="66341-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="66341-111">方法</span><span class="sxs-lookup"><span data-stu-id="66341-111">Methods</span></span>
|<span data-ttu-id="66341-112">方法</span><span class="sxs-lookup"><span data-stu-id="66341-112">Method</span></span>|<span data-ttu-id="66341-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="66341-113">Return type</span></span>|<span data-ttu-id="66341-114">说明</span><span class="sxs-lookup"><span data-stu-id="66341-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66341-115">列表列表</span><span class="sxs-lookup"><span data-stu-id="66341-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="66341-116">[todoTaskList](todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66341-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="66341-117">获取用户[邮箱中的所有 todoTaskList。](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="66341-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="66341-118">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="66341-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="66341-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="66341-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="66341-120">在[用户邮箱中创建 todoTaskList。](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="66341-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="66341-121">获取任务列表</span><span class="sxs-lookup"><span data-stu-id="66341-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="66341-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="66341-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="66341-123">读取指定的 [todoTaskList 的属性和关系](todotasklist.md)。</span><span class="sxs-lookup"><span data-stu-id="66341-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="66341-124">更新任务列表</span><span class="sxs-lookup"><span data-stu-id="66341-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="66341-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="66341-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="66341-126">更新指定的 [todoTaskList 的可写属性](todotasklist.md)。</span><span class="sxs-lookup"><span data-stu-id="66341-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="66341-127">删除任务列表</span><span class="sxs-lookup"><span data-stu-id="66341-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="66341-128">无</span><span class="sxs-lookup"><span data-stu-id="66341-128">None</span></span>| <span data-ttu-id="66341-129">删除指定的 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="66341-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="66341-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="66341-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="66341-131">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66341-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="66341-132">获取指定 [列表中的所有 todoTask](todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="66341-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="66341-133">创建任务</span><span class="sxs-lookup"><span data-stu-id="66341-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="66341-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="66341-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="66341-135">在指定[任务列表中创建 todoTask。](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="66341-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="66341-136">属性</span><span class="sxs-lookup"><span data-stu-id="66341-136">Properties</span></span>
|<span data-ttu-id="66341-137">属性</span><span class="sxs-lookup"><span data-stu-id="66341-137">Property</span></span>|<span data-ttu-id="66341-138">类型</span><span class="sxs-lookup"><span data-stu-id="66341-138">Type</span></span>|<span data-ttu-id="66341-139">说明</span><span class="sxs-lookup"><span data-stu-id="66341-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66341-140">displayName</span><span class="sxs-lookup"><span data-stu-id="66341-140">displayName</span></span>|<span data-ttu-id="66341-141">String</span><span class="sxs-lookup"><span data-stu-id="66341-141">String</span></span>|<span data-ttu-id="66341-142">任务列表的名称。</span><span class="sxs-lookup"><span data-stu-id="66341-142">The name of the task list.</span></span>|
|<span data-ttu-id="66341-143">id</span><span class="sxs-lookup"><span data-stu-id="66341-143">id</span></span>|<span data-ttu-id="66341-144">String</span><span class="sxs-lookup"><span data-stu-id="66341-144">String</span></span>| <span data-ttu-id="66341-145">任务列表的标识符，在用户邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="66341-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="66341-146">只读。</span><span class="sxs-lookup"><span data-stu-id="66341-146">Read-only.</span></span> <span data-ttu-id="66341-147">从实体 [继承](entity.md)</span><span class="sxs-lookup"><span data-stu-id="66341-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="66341-148">isOwner</span><span class="sxs-lookup"><span data-stu-id="66341-148">isOwner</span></span>|<span data-ttu-id="66341-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="66341-149">Boolean</span></span>| <span data-ttu-id="66341-150">如果用户是给定的任务列表的所有者，则为 True 。</span><span class="sxs-lookup"><span data-stu-id="66341-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="66341-151">isShared</span><span class="sxs-lookup"><span data-stu-id="66341-151">isShared</span></span>|<span data-ttu-id="66341-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="66341-152">Boolean</span></span>| <span data-ttu-id="66341-153">如此 如果任务列表与其他用户共享</span><span class="sxs-lookup"><span data-stu-id="66341-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="66341-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="66341-154">wellknownListName</span></span>|<span data-ttu-id="66341-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="66341-155">wellknownListName</span></span>| <span data-ttu-id="66341-156">指示给定列表是否是已知列表的已知列表名称的属性。</span><span class="sxs-lookup"><span data-stu-id="66341-156">Property indicating the well-known list name if the given list is a well-known list.</span></span> <span data-ttu-id="66341-157">可取值为：`none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="66341-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66341-158">关系</span><span class="sxs-lookup"><span data-stu-id="66341-158">Relationships</span></span>
|<span data-ttu-id="66341-159">关系</span><span class="sxs-lookup"><span data-stu-id="66341-159">Relationship</span></span>|<span data-ttu-id="66341-160">类型</span><span class="sxs-lookup"><span data-stu-id="66341-160">Type</span></span>|<span data-ttu-id="66341-161">说明</span><span class="sxs-lookup"><span data-stu-id="66341-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66341-162">extensions</span><span class="sxs-lookup"><span data-stu-id="66341-162">extensions</span></span>|<span data-ttu-id="66341-163">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="66341-163">[extension](extension.md) collection</span></span>| <span data-ttu-id="66341-164">为任务列表定义的开放扩展集合。</span><span class="sxs-lookup"><span data-stu-id="66341-164">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="66341-165">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="66341-165">Nullable.</span></span>|
|<span data-ttu-id="66341-166">任务</span><span class="sxs-lookup"><span data-stu-id="66341-166">tasks</span></span>|<span data-ttu-id="66341-167">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66341-167">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="66341-168">此任务列表中的任务。</span><span class="sxs-lookup"><span data-stu-id="66341-168">The tasks in this task list.</span></span> <span data-ttu-id="66341-169">只读。</span><span class="sxs-lookup"><span data-stu-id="66341-169">Read-only.</span></span> <span data-ttu-id="66341-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="66341-170">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66341-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66341-171">JSON representation</span></span>
<span data-ttu-id="66341-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66341-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTaskList",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "String (identifier)",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```

