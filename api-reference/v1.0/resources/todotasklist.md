---
title: todoTaskList 资源类型
description: Microsoft 中的一个列表，其中包含一个或多个 todoTask 资源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2e55d5122da02966fa89084c44f5447edccdf631
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797199"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="60af6-103">todoTaskList 资源类型</span><span class="sxs-lookup"><span data-stu-id="60af6-103">todoTaskList resource type</span></span>

<span data-ttu-id="60af6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60af6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60af6-105">Microsoft 中的一个列表，其中包含一个或多个 [todoTask](./todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="60af6-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="60af6-106">在中，有一些内置的任务列表（如已 **标记的电子邮件** 和 **任务** ），无法重命名或删除。</span><span class="sxs-lookup"><span data-stu-id="60af6-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="60af6-107">不过，您可以创建其他任务列表。</span><span class="sxs-lookup"><span data-stu-id="60af6-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="60af6-108">此资源支持</span><span class="sxs-lookup"><span data-stu-id="60af6-108">This resource supports</span></span>
* <span data-ttu-id="60af6-109">将数据作为[开放扩展](/graph/extensibility-overview)添加到自定义属性</span><span class="sxs-lookup"><span data-stu-id="60af6-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="60af6-110">使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="60af6-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="60af6-111">方法</span><span class="sxs-lookup"><span data-stu-id="60af6-111">Methods</span></span>
|<span data-ttu-id="60af6-112">方法</span><span class="sxs-lookup"><span data-stu-id="60af6-112">Method</span></span>|<span data-ttu-id="60af6-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="60af6-113">Return type</span></span>|<span data-ttu-id="60af6-114">说明</span><span class="sxs-lookup"><span data-stu-id="60af6-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60af6-115">列出列表</span><span class="sxs-lookup"><span data-stu-id="60af6-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="60af6-116">[todoTaskList](todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60af6-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="60af6-117">获取用户邮箱中的所有 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="60af6-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="60af6-118">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="60af6-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="60af6-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="60af6-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="60af6-120">在用户的邮箱中创建 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="60af6-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="60af6-121">获取任务列表</span><span class="sxs-lookup"><span data-stu-id="60af6-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="60af6-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="60af6-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="60af6-123">读取指定 [todoTaskList](todotasklist.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="60af6-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="60af6-124">更新任务列表</span><span class="sxs-lookup"><span data-stu-id="60af6-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="60af6-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="60af6-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="60af6-126">更新指定 [todoTaskList](todotasklist.md)的可写属性。</span><span class="sxs-lookup"><span data-stu-id="60af6-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="60af6-127">删除任务列表</span><span class="sxs-lookup"><span data-stu-id="60af6-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="60af6-128">无</span><span class="sxs-lookup"><span data-stu-id="60af6-128">None</span></span>| <span data-ttu-id="60af6-129">删除指定的 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="60af6-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="60af6-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="60af6-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="60af6-131">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60af6-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="60af6-132">获取指定列表中的所有 [todoTask](todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="60af6-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="60af6-133">创建任务</span><span class="sxs-lookup"><span data-stu-id="60af6-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="60af6-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="60af6-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="60af6-135">在指定的任务列表中创建 [todoTask](todotask.md) 。</span><span class="sxs-lookup"><span data-stu-id="60af6-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="60af6-136">属性</span><span class="sxs-lookup"><span data-stu-id="60af6-136">Properties</span></span>
|<span data-ttu-id="60af6-137">属性</span><span class="sxs-lookup"><span data-stu-id="60af6-137">Property</span></span>|<span data-ttu-id="60af6-138">类型</span><span class="sxs-lookup"><span data-stu-id="60af6-138">Type</span></span>|<span data-ttu-id="60af6-139">说明</span><span class="sxs-lookup"><span data-stu-id="60af6-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60af6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="60af6-140">displayName</span></span>|<span data-ttu-id="60af6-141">String</span><span class="sxs-lookup"><span data-stu-id="60af6-141">String</span></span>|<span data-ttu-id="60af6-142">任务列表的名称。</span><span class="sxs-lookup"><span data-stu-id="60af6-142">The name of the task list.</span></span>|
|<span data-ttu-id="60af6-143">id</span><span class="sxs-lookup"><span data-stu-id="60af6-143">id</span></span>|<span data-ttu-id="60af6-144">String</span><span class="sxs-lookup"><span data-stu-id="60af6-144">String</span></span>| <span data-ttu-id="60af6-145">任务列表的标识符，在用户的邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="60af6-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="60af6-146">只读。</span><span class="sxs-lookup"><span data-stu-id="60af6-146">Read-only.</span></span> <span data-ttu-id="60af6-147">继承自 [entity](entity.md)</span><span class="sxs-lookup"><span data-stu-id="60af6-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="60af6-148">isOwner</span><span class="sxs-lookup"><span data-stu-id="60af6-148">isOwner</span></span>|<span data-ttu-id="60af6-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="60af6-149">Boolean</span></span>| <span data-ttu-id="60af6-150">如果用户是给定任务列表的所有者，则为 True。</span><span class="sxs-lookup"><span data-stu-id="60af6-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="60af6-151">isShared</span><span class="sxs-lookup"><span data-stu-id="60af6-151">isShared</span></span>|<span data-ttu-id="60af6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="60af6-152">Boolean</span></span>| <span data-ttu-id="60af6-153">如果任务列表与其他用户共享，则为 True</span><span class="sxs-lookup"><span data-stu-id="60af6-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="60af6-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="60af6-154">wellknownListName</span></span>|<span data-ttu-id="60af6-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="60af6-155">wellknownListName</span></span>| <span data-ttu-id="60af6-156">如果给定的列表是已知列表，则指示列表名称的属性。</span><span class="sxs-lookup"><span data-stu-id="60af6-156">Property indicating the list name if the given list is a well-known list.</span></span> <span data-ttu-id="60af6-157">可取值为：`none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="60af6-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

### <a name="wellknownlistname-values"></a><span data-ttu-id="60af6-158">wellknownListName 值</span><span class="sxs-lookup"><span data-stu-id="60af6-158">wellknownListName values</span></span>
|<span data-ttu-id="60af6-159">成员</span><span class="sxs-lookup"><span data-stu-id="60af6-159">Member</span></span>|<span data-ttu-id="60af6-160">说明</span><span class="sxs-lookup"><span data-stu-id="60af6-160">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60af6-161">无</span><span class="sxs-lookup"><span data-stu-id="60af6-161">none</span></span>| <span data-ttu-id="60af6-162">用户创建的列表。</span><span class="sxs-lookup"><span data-stu-id="60af6-162">User created list.</span></span>|
|<span data-ttu-id="60af6-163">defaultList</span><span class="sxs-lookup"><span data-stu-id="60af6-163">defaultList</span></span>| <span data-ttu-id="60af6-164">内置 **任务** 列表。</span><span class="sxs-lookup"><span data-stu-id="60af6-164">Built-in **Tasks** list.</span></span>|
|<span data-ttu-id="60af6-165">flaggedEmails</span><span class="sxs-lookup"><span data-stu-id="60af6-165">flaggedEmails</span></span>| <span data-ttu-id="60af6-166">内置的已 **标记电子邮件** 列表。</span><span class="sxs-lookup"><span data-stu-id="60af6-166">Built-in **Flagged email** list.</span></span> <span data-ttu-id="60af6-167">此列表中存在已标记的电子邮件中的任务。</span><span class="sxs-lookup"><span data-stu-id="60af6-167">Tasks from flagged emails are present in this list.</span></span>|
|<span data-ttu-id="60af6-168">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="60af6-168">unknownFutureValue</span></span>| <span data-ttu-id="60af6-169">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="60af6-169">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="60af6-170">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="60af6-170">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60af6-171">关系</span><span class="sxs-lookup"><span data-stu-id="60af6-171">Relationships</span></span>
|<span data-ttu-id="60af6-172">关系</span><span class="sxs-lookup"><span data-stu-id="60af6-172">Relationship</span></span>|<span data-ttu-id="60af6-173">类型</span><span class="sxs-lookup"><span data-stu-id="60af6-173">Type</span></span>|<span data-ttu-id="60af6-174">说明</span><span class="sxs-lookup"><span data-stu-id="60af6-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60af6-175">extensions</span><span class="sxs-lookup"><span data-stu-id="60af6-175">extensions</span></span>|<span data-ttu-id="60af6-176">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="60af6-176">[extension](extension.md) collection</span></span>| <span data-ttu-id="60af6-177">为任务列表定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="60af6-177">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="60af6-178">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="60af6-178">Nullable.</span></span>|
|<span data-ttu-id="60af6-179">任务</span><span class="sxs-lookup"><span data-stu-id="60af6-179">tasks</span></span>|<span data-ttu-id="60af6-180">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60af6-180">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="60af6-181">此任务列表中的任务。</span><span class="sxs-lookup"><span data-stu-id="60af6-181">The tasks in this task list.</span></span> <span data-ttu-id="60af6-182">只读。</span><span class="sxs-lookup"><span data-stu-id="60af6-182">Read-only.</span></span> <span data-ttu-id="60af6-183">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="60af6-183">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60af6-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60af6-184">JSON representation</span></span>
<span data-ttu-id="60af6-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60af6-185">The following is a JSON representation of the resource.</span></span>
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



