---
title: todoTaskList 资源类型
description: Microsoft 中的一个列表，其中包含一个或多个 todoTask 资源。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0523404e836223f8a59e191d1e7040a279433795
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073381"
---
# <a name="todotasklist-resource-type"></a><span data-ttu-id="a70f6-103">todoTaskList 资源类型</span><span class="sxs-lookup"><span data-stu-id="a70f6-103">todoTaskList resource type</span></span>

<span data-ttu-id="a70f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a70f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a70f6-105">Microsoft 中的一个列表，其中包含一个或多个 [todoTask](./todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="a70f6-105">A list in Microsoft To Do that contains one or more [todoTask](./todotask.md) resources.</span></span> 

<span data-ttu-id="a70f6-106">在中，有一些内置的任务列表（如已 **标记的电子邮件** 和 **任务** ），无法重命名或删除。</span><span class="sxs-lookup"><span data-stu-id="a70f6-106">In To Do, there are built-in task lists such as **Flagged emails** and **Tasks** which cannot be renamed or deleted.</span></span>  <span data-ttu-id="a70f6-107">不过，您可以创建其他任务列表。</span><span class="sxs-lookup"><span data-stu-id="a70f6-107">You can, however, create additional task lists.</span></span>

<span data-ttu-id="a70f6-108">此资源支持</span><span class="sxs-lookup"><span data-stu-id="a70f6-108">This resource supports</span></span>
* <span data-ttu-id="a70f6-109">将数据作为[开放扩展](/graph/extensibility-overview)添加到自定义属性</span><span class="sxs-lookup"><span data-stu-id="a70f6-109">Adding your data to custom properties as [open extensions](/graph/extensibility-overview)</span></span>
* <span data-ttu-id="a70f6-110">使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="a70f6-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="a70f6-111">方法</span><span class="sxs-lookup"><span data-stu-id="a70f6-111">Methods</span></span>
|<span data-ttu-id="a70f6-112">方法</span><span class="sxs-lookup"><span data-stu-id="a70f6-112">Method</span></span>|<span data-ttu-id="a70f6-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="a70f6-113">Return type</span></span>|<span data-ttu-id="a70f6-114">说明</span><span class="sxs-lookup"><span data-stu-id="a70f6-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a70f6-115">列出列表</span><span class="sxs-lookup"><span data-stu-id="a70f6-115">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="a70f6-116">[todoTaskList](todotasklist.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a70f6-116">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="a70f6-117">获取用户邮箱中的所有 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="a70f6-117">Get all the [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="a70f6-118">创建 todoTaskList</span><span class="sxs-lookup"><span data-stu-id="a70f6-118">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="a70f6-119">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="a70f6-119">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="a70f6-120">在用户的邮箱中创建 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="a70f6-120">Create a [todoTaskList](todotasklist.md) in the user's mailbox.</span></span> |
|[<span data-ttu-id="a70f6-121">获取任务列表</span><span class="sxs-lookup"><span data-stu-id="a70f6-121">Get task list</span></span>](../api/todotasklist-get.md)|[<span data-ttu-id="a70f6-122">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="a70f6-122">todoTaskList</span></span>](todotasklist.md)|<span data-ttu-id="a70f6-123">读取指定 [todoTaskList](todotasklist.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a70f6-123">Read the properties and relationships of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="a70f6-124">更新任务列表</span><span class="sxs-lookup"><span data-stu-id="a70f6-124">Update task list</span></span>](../api/todotasklist-update.md)|[<span data-ttu-id="a70f6-125">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="a70f6-125">todoTaskList</span></span>](todotasklist.md)| <span data-ttu-id="a70f6-126">更新指定 [todoTaskList](todotasklist.md)的可写属性。</span><span class="sxs-lookup"><span data-stu-id="a70f6-126">Update the writable properties of the specified [todoTaskList](todotasklist.md).</span></span>|
|[<span data-ttu-id="a70f6-127">删除任务列表</span><span class="sxs-lookup"><span data-stu-id="a70f6-127">Delete task list</span></span>](../api/todotasklist-delete.md)|<span data-ttu-id="a70f6-128">无</span><span class="sxs-lookup"><span data-stu-id="a70f6-128">None</span></span>| <span data-ttu-id="a70f6-129">删除指定的 [todoTaskList](todotasklist.md) 。</span><span class="sxs-lookup"><span data-stu-id="a70f6-129">Delete the specified [todoTaskList](todotasklist.md) .</span></span>|
|[<span data-ttu-id="a70f6-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="a70f6-130">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="a70f6-131">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a70f6-131">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="a70f6-132">获取指定列表中的所有 [todoTask](todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="a70f6-132">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="a70f6-133">创建任务</span><span class="sxs-lookup"><span data-stu-id="a70f6-133">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="a70f6-134">todoTask</span><span class="sxs-lookup"><span data-stu-id="a70f6-134">todoTask</span></span>](todotask.md)| <span data-ttu-id="a70f6-135">在指定的任务列表中创建 [todoTask](todotask.md) 。</span><span class="sxs-lookup"><span data-stu-id="a70f6-135">Create a [todoTask](todotask.md) in the specified task list.</span></span>|

## <a name="properties"></a><span data-ttu-id="a70f6-136">属性</span><span class="sxs-lookup"><span data-stu-id="a70f6-136">Properties</span></span>
|<span data-ttu-id="a70f6-137">属性</span><span class="sxs-lookup"><span data-stu-id="a70f6-137">Property</span></span>|<span data-ttu-id="a70f6-138">类型</span><span class="sxs-lookup"><span data-stu-id="a70f6-138">Type</span></span>|<span data-ttu-id="a70f6-139">说明</span><span class="sxs-lookup"><span data-stu-id="a70f6-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70f6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="a70f6-140">displayName</span></span>|<span data-ttu-id="a70f6-141">String</span><span class="sxs-lookup"><span data-stu-id="a70f6-141">String</span></span>|<span data-ttu-id="a70f6-142">任务列表的名称。</span><span class="sxs-lookup"><span data-stu-id="a70f6-142">The name of the task list.</span></span>|
|<span data-ttu-id="a70f6-143">id</span><span class="sxs-lookup"><span data-stu-id="a70f6-143">id</span></span>|<span data-ttu-id="a70f6-144">String</span><span class="sxs-lookup"><span data-stu-id="a70f6-144">String</span></span>| <span data-ttu-id="a70f6-145">任务列表的标识符，在用户的邮箱中是唯一的。</span><span class="sxs-lookup"><span data-stu-id="a70f6-145">The identifier of the task list, unique in the user's mailbox.</span></span> <span data-ttu-id="a70f6-146">只读。</span><span class="sxs-lookup"><span data-stu-id="a70f6-146">Read-only.</span></span> <span data-ttu-id="a70f6-147">继承自 [entity](entity.md)</span><span class="sxs-lookup"><span data-stu-id="a70f6-147">Inherited from [entity](entity.md)</span></span>|
|<span data-ttu-id="a70f6-148">isOwner</span><span class="sxs-lookup"><span data-stu-id="a70f6-148">isOwner</span></span>|<span data-ttu-id="a70f6-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="a70f6-149">Boolean</span></span>| <span data-ttu-id="a70f6-150">如果用户是给定任务列表的所有者，则为 True。</span><span class="sxs-lookup"><span data-stu-id="a70f6-150">True if the user is owner of the given task list.</span></span>|
|<span data-ttu-id="a70f6-151">isShared</span><span class="sxs-lookup"><span data-stu-id="a70f6-151">isShared</span></span>|<span data-ttu-id="a70f6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a70f6-152">Boolean</span></span>| <span data-ttu-id="a70f6-153">如果任务列表与其他用户共享，则为 True</span><span class="sxs-lookup"><span data-stu-id="a70f6-153">True if the task list is shared with other users</span></span>|
|<span data-ttu-id="a70f6-154">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="a70f6-154">wellknownListName</span></span>|<span data-ttu-id="a70f6-155">wellknownListName</span><span class="sxs-lookup"><span data-stu-id="a70f6-155">wellknownListName</span></span>| <span data-ttu-id="a70f6-156">指示已知列表名称的属性（如果给定列表是已知列表）。</span><span class="sxs-lookup"><span data-stu-id="a70f6-156">Property indicating the well-known list name if the given list is a well-known list.</span></span> <span data-ttu-id="a70f6-157">可取值为：`none`、`defaultList`、`flaggedEmails`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a70f6-157">Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a70f6-158">关系</span><span class="sxs-lookup"><span data-stu-id="a70f6-158">Relationships</span></span>
|<span data-ttu-id="a70f6-159">关系</span><span class="sxs-lookup"><span data-stu-id="a70f6-159">Relationship</span></span>|<span data-ttu-id="a70f6-160">类型</span><span class="sxs-lookup"><span data-stu-id="a70f6-160">Type</span></span>|<span data-ttu-id="a70f6-161">说明</span><span class="sxs-lookup"><span data-stu-id="a70f6-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70f6-162">extensions</span><span class="sxs-lookup"><span data-stu-id="a70f6-162">extensions</span></span>|<span data-ttu-id="a70f6-163">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="a70f6-163">[extension](extension.md) collection</span></span>| <span data-ttu-id="a70f6-164">为任务列表定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="a70f6-164">The collection of open extensions defined for the task list.</span></span> <span data-ttu-id="a70f6-165">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a70f6-165">Nullable.</span></span>|
|<span data-ttu-id="a70f6-166">任务</span><span class="sxs-lookup"><span data-stu-id="a70f6-166">tasks</span></span>|<span data-ttu-id="a70f6-167">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a70f6-167">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="a70f6-168">此任务列表中的任务。</span><span class="sxs-lookup"><span data-stu-id="a70f6-168">The tasks in this task list.</span></span> <span data-ttu-id="a70f6-169">只读。</span><span class="sxs-lookup"><span data-stu-id="a70f6-169">Read-only.</span></span> <span data-ttu-id="a70f6-170">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a70f6-170">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a70f6-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a70f6-171">JSON representation</span></span>
<span data-ttu-id="a70f6-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a70f6-172">The following is a JSON representation of the resource.</span></span>
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



