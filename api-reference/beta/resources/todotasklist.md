---
title: todoTaskList 资源类型
description: Microsoft 中的一个列表，其中包含一个或多个 todoTask 资源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bddf0b72173b2f37b3fdd8544bc777c87bb33ee3
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314592"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="5336e-103">todoTaskList 资源类型</span><span class="sxs-lookup"><span data-stu-id="5336e-103">todoTaskList resource type</span></span>

<span data-ttu-id="5336e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5336e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5336e-105">Microsoft 中的一个列表，其中包含一个或多个 [todoTask](./todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="5336e-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="5336e-106">在中，有一些内置的任务列表（如已 **标记的电子邮件** 和 **任务** ），无法重命名或删除。</span><span class="sxs-lookup"><span data-stu-id="5336e-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="5336e-107">不过，您可以创建其他任务列表。</span><span class="sxs-lookup"><span data-stu-id="5336e-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="5336e-108">此资源支持</span><span class="sxs-lookup"><span data-stu-id="5336e-108">This resource supports</span></span>
* <span data-ttu-id="5336e-109">将数据作为[开放扩展](/graph/extensibility-overview)添加到自定义属性</span><span class="sxs-lookup"><span data-stu-id="5336e-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="5336e-110">使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="5336e-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="5336e-111">方法</span><span class="sxs-lookup"><span data-stu-id="5336e-111">Methods</span></span>
|<span data-ttu-id="5336e-112">方法</span><span class="sxs-lookup"><span data-stu-id="5336e-112">Method</span></span>|<span data-ttu-id="5336e-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="5336e-113">Return type</span></span>|<span data-ttu-id="5336e-114">说明</span><span class="sxs-lookup"><span data-stu-id="5336e-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5336e-115">列出列表</span><span class="sxs-lookup"><span data-stu-id="5336e-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="5336e-116">[todoTaskList](todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5336e-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="5336e-117">获取用户邮箱中的所有 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="5336e-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="5336e-118">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5336e-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="5336e-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5336e-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="5336e-120">在用户的邮箱中创建 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="5336e-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="5336e-121">获取任务列表</span><span class="sxs-lookup"><span data-stu-id="5336e-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="5336e-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5336e-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="5336e-123">读取指定 [todoTaskList](todotasklist.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5336e-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="5336e-124">更新任务列表</span><span class="sxs-lookup"><span data-stu-id="5336e-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="5336e-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5336e-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="5336e-126">更新指定 [todoTaskList](todotasklist.md)的可写属性。</span><span class="sxs-lookup"><span data-stu-id="5336e-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="5336e-127">删除任务列表</span><span class="sxs-lookup"><span data-stu-id="5336e-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="5336e-128">无</span><span class="sxs-lookup"><span data-stu-id="5336e-128">None</span></span>| <span data-ttu-id="5336e-129">删除指定的 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="5336e-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="5336e-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="5336e-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="5336e-131">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5336e-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="5336e-132">获取指定列表中的所有 [todoTask](todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="5336e-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="5336e-133">创建任务</span><span class="sxs-lookup"><span data-stu-id="5336e-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="5336e-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="5336e-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="5336e-135">在指定的任务列表中创建 [todoTask](todotask.md) 。</span><span class="sxs-lookup"><span data-stu-id="5336e-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="5336e-136">属性</span><span class="sxs-lookup"><span data-stu-id="5336e-136">Properties</span></span>
|<span data-ttu-id="5336e-137">属性</span><span class="sxs-lookup"><span data-stu-id="5336e-137">Property</span></span>|<span data-ttu-id="5336e-138">类型</span><span class="sxs-lookup"><span data-stu-id="5336e-138">Type</span></span>|<span data-ttu-id="5336e-139">说明</span><span class="sxs-lookup"><span data-stu-id="5336e-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5336e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5336e-140">displayName</span></span>|<span data-ttu-id="5336e-141">字符串</span><span class="sxs-lookup"><span data-stu-id="5336e-141">String</span></span>|<span data-ttu-id="5336e-142">任务列表的名称。</span><span class="sxs-lookup"><span data-stu-id="5336e-142">The name of the task list.</span></span>|
|<span data-ttu-id="5336e-143">id</span><span class="sxs-lookup"><span data-stu-id="5336e-143">id</span></span>|<span data-ttu-id="5336e-144">字符串</span><span class="sxs-lookup"><span data-stu-id="5336e-144">String</span></span>| <span data-ttu-id="5336e-145">任务列表的标识符，在用户的邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="5336e-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="5336e-146">只读。</span><span class="sxs-lookup"><span data-stu-id="5336e-146">Read-only.</span></span> <span data-ttu-id="5336e-147">继承自 [entity](entity.md)</span><span class="sxs-lookup"><span data-stu-id="5336e-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="5336e-148">isOwner</span><span class="sxs-lookup"><span data-stu-id="5336e-148">isOwner</span></span>|<span data-ttu-id="5336e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5336e-149">Boolean</span></span>| <span data-ttu-id="5336e-150">如果用户是给定任务列表的所有者，则为 True。</span><span class="sxs-lookup"><span data-stu-id="5336e-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="5336e-151">isShared</span><span class="sxs-lookup"><span data-stu-id="5336e-151">isShared</span></span>|<span data-ttu-id="5336e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="5336e-152">Boolean</span></span>| <span data-ttu-id="5336e-153">如果任务列表与其他用户共享，则为 True</span><span class="sxs-lookup"><span data-stu-id="5336e-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="5336e-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="5336e-154">wellknownListName</span></span>|<span data-ttu-id="5336e-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="5336e-155">wellknownListName</span></span>| <span data-ttu-id="5336e-156">如果给定的列表是已知列表，则指示列表名称的属性。</span><span class="sxs-lookup"><span data-stu-id="5336e-156">Property indicating the list name if the given list is a well-known list.</span></span> <span data-ttu-id="5336e-157">可取值为：`none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5336e-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

### <a name="wellknownlistname-values"></a><span data-ttu-id="5336e-158">wellknownListName 值</span><span class="sxs-lookup"><span data-stu-id="5336e-158">wellknownListName values</span></span>
|<span data-ttu-id="5336e-159">成员</span><span class="sxs-lookup"><span data-stu-id="5336e-159">Member</span></span>|<span data-ttu-id="5336e-160">说明</span><span class="sxs-lookup"><span data-stu-id="5336e-160">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5336e-161">无</span><span class="sxs-lookup"><span data-stu-id="5336e-161">none</span></span>| <span data-ttu-id="5336e-162">用户创建的列表。</span><span class="sxs-lookup"><span data-stu-id="5336e-162">User created list.</span></span>|
|<span data-ttu-id="5336e-163">defaultList</span><span class="sxs-lookup"><span data-stu-id="5336e-163">defaultList</span></span>| <span data-ttu-id="5336e-164">内置 **任务** 列表。</span><span class="sxs-lookup"><span data-stu-id="5336e-164">Built-in **Tasks** list.</span></span>|
|<span data-ttu-id="5336e-165">flaggedEmails</span><span class="sxs-lookup"><span data-stu-id="5336e-165">flaggedEmails</span></span>| <span data-ttu-id="5336e-166">内置的已 **标记电子邮件** 列表。</span><span class="sxs-lookup"><span data-stu-id="5336e-166">Built-in **Flagged email** list.</span></span> <span data-ttu-id="5336e-167">此列表中存在已标记的电子邮件中的任务。</span><span class="sxs-lookup"><span data-stu-id="5336e-167">Tasks from flagged emails are present in this list.</span></span>|
|<span data-ttu-id="5336e-168">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="5336e-168">unknownFutureValue</span></span>| <span data-ttu-id="5336e-169">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="5336e-169">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="5336e-170">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="5336e-170">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5336e-171">关系</span><span class="sxs-lookup"><span data-stu-id="5336e-171">Relationships</span></span>
|<span data-ttu-id="5336e-172">关系</span><span class="sxs-lookup"><span data-stu-id="5336e-172">Relationship</span></span>|<span data-ttu-id="5336e-173">类型</span><span class="sxs-lookup"><span data-stu-id="5336e-173">Type</span></span>|<span data-ttu-id="5336e-174">说明</span><span class="sxs-lookup"><span data-stu-id="5336e-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5336e-175">extensions</span><span class="sxs-lookup"><span data-stu-id="5336e-175">extensions</span></span>|<span data-ttu-id="5336e-176">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="5336e-176">[extension](extension.md) collection</span></span>| <span data-ttu-id="5336e-177">为任务列表定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="5336e-177">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="5336e-178">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5336e-178">Nullable.</span></span>|
|<span data-ttu-id="5336e-179">任务</span><span class="sxs-lookup"><span data-stu-id="5336e-179">tasks</span></span>|<span data-ttu-id="5336e-180">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5336e-180">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="5336e-181">此任务列表中的任务。</span><span class="sxs-lookup"><span data-stu-id="5336e-181">The tasks in this task list.</span></span> <span data-ttu-id="5336e-182">只读。</span><span class="sxs-lookup"><span data-stu-id="5336e-182">Read-only.</span></span> <span data-ttu-id="5336e-183">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5336e-183">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5336e-184">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5336e-184">JSON representation</span></span>
<span data-ttu-id="5336e-185">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5336e-185">The following is a JSON representation of the resource.</span></span>
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



