---
title: 使用进度表 REST API
description: 可以使用在 Microsoft Graph 计划程序 API 创建任务并将其分配给 Office 365 中的某个组中的用户。
ms.openlocfilehash: 264a196a24dde21b57ff3627c7c39c1951a02ce6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041447"
---
# <a name="use-the-planner-rest-api"></a><span data-ttu-id="15a43-103">使用进度表 REST API</span><span class="sxs-lookup"><span data-stu-id="15a43-103">Use the Planner REST API</span></span>

> <span data-ttu-id="15a43-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="15a43-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15a43-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="15a43-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15a43-106">可以使用在 Microsoft Graph 计划程序 API 创建任务并将其分配给 Office 365 中的某个组中的用户。</span><span class="sxs-lookup"><span data-stu-id="15a43-106">You can use the Planner API in Microsoft Graph to create tasks and assign them to users in a group in Office 365.</span></span>

<span data-ttu-id="15a43-107">在开始使用规划器 API 之前，值得的了解如何的主要对象相互以及来对 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="15a43-107">Before you get started with Planner API, it is worth understanding how the main objects relate to each other as well as to Office 365 groups.</span></span>

## <a name="groups"></a><span data-ttu-id="15a43-108">Groups</span><span class="sxs-lookup"><span data-stu-id="15a43-108">Groups</span></span>

<span data-ttu-id="15a43-109">Office 365 组都是计划工具 API 中计划的所有者。</span><span class="sxs-lookup"><span data-stu-id="15a43-109">Office 365 groups are the owners of the plans in the Planner API.</span></span>
<span data-ttu-id="15a43-110">为[获取一组由拥有的计划](../api/plannergroup-list-plans.md)，进行以下的 HTTP 请求。</span><span class="sxs-lookup"><span data-stu-id="15a43-110">To [get the plans owned by a group](../api/plannergroup-list-plans.md), make the following HTTP request.</span></span>

``` http
GET /groups/{id}/planner/plans
```

<span data-ttu-id="15a43-111">当[创建新的计划](../api/planner-post-plans.md)，通过设置指定给计划组所有者`owner`计划对象的属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-111">When [creating a new plan](../api/planner-post-plans.md), give the plan a group owner by setting the `owner` property on a plan object.</span></span> <span data-ttu-id="15a43-112">必须由组拥有计划。</span><span class="sxs-lookup"><span data-stu-id="15a43-112">A plan must be owned by a group.</span></span> <span data-ttu-id="15a43-113">组可以拥有多个计划。</span><span class="sxs-lookup"><span data-stu-id="15a43-113">A group can own multiple plans.</span></span>

><span data-ttu-id="15a43-114">**注意：** 正在创建计划的用户必须将拥有计划的组的成员。</span><span class="sxs-lookup"><span data-stu-id="15a43-114">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="15a43-115">当使用[创建组](../api/group-post-groups.md)创建一个新的组时，您不是添加到组，作为成员。</span><span class="sxs-lookup"><span data-stu-id="15a43-115">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="15a43-116">创建组后，将自己添加为成员使用[组发布成员](../api/group-post-members.md)。</span><span class="sxs-lookup"><span data-stu-id="15a43-116">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="plans"></a><span data-ttu-id="15a43-117">计划</span><span class="sxs-lookup"><span data-stu-id="15a43-117">Plans</span></span>

<span data-ttu-id="15a43-118">[计划](plannerplan.md)的[任务](plannertask.md)的容器。</span><span class="sxs-lookup"><span data-stu-id="15a43-118">[Plans](plannerplan.md) are the containers of [tasks](plannertask.md).</span></span> <span data-ttu-id="15a43-119">对[创建在计划任务](../api/planner-post-tasks.md)，请设置`planId`task 对象创建任务时计划的 id 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-119">To [create a task in a plan](../api/planner-post-tasks.md), set the `planId` property on the task object to the ID of the plan while creating the task.</span></span>
<span data-ttu-id="15a43-120">当前无法不带计划创建任务。</span><span class="sxs-lookup"><span data-stu-id="15a43-120">Tasks currently cannot be created without plans.</span></span>
<span data-ttu-id="15a43-121">对[检索计划中的任务](../api/plannerplan-list-tasks.md)，请进行以下的 HTTP 请求。</span><span class="sxs-lookup"><span data-stu-id="15a43-121">To [retrieve the tasks in a plan](../api/plannerplan-list-tasks.md), make the following HTTP request.</span></span>

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a><span data-ttu-id="15a43-122">任务</span><span class="sxs-lookup"><span data-stu-id="15a43-122">Tasks</span></span>

<span data-ttu-id="15a43-p106">可以通过在任务对象的 [assignments](plannerassignments.md) 属性中添加[分配](plannerassignment.md)将每个任务分配给一位用户。要分配任务的用户 ID 是 `assignments` 上的开放属性的名称，且必须指定分配上的 `orderHint` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p106">Each task can be assigned to a user by adding an [assignment](plannerassignment.md) in the [assignments](plannerassignments.md) property on the task object. The ID of the user to assign the task is the name of the open property on `assignments`, and the `orderHint` property on the assignment must be specified.</span></span>

## <a name="task-and-plan-details"></a><span data-ttu-id="15a43-125">任务和计划详细信息</span><span class="sxs-lookup"><span data-stu-id="15a43-125">Task and plan details</span></span> 

<span data-ttu-id="15a43-126">计划工具资源排列到基本任务和计划对象和详细任务和计划对象。</span><span class="sxs-lookup"><span data-stu-id="15a43-126">Planner resources are arranged into basic task and plan objects and detail task and plan objects.</span></span> <span data-ttu-id="15a43-127">基本对象提供的资源，适用于列表视图的详细信息对象提供对适用于深化视图的资源的大型属性访问时的常见属性的访问权限。</span><span class="sxs-lookup"><span data-stu-id="15a43-127">Basic objects provide access to common properties of the resources, suitable for list views, while the detail objects provide access to large properties of the resources suitable for drill down views.</span></span>

## <a name="visualization"></a><span data-ttu-id="15a43-128">可视化</span><span class="sxs-lookup"><span data-stu-id="15a43-128">Visualization</span></span>

<span data-ttu-id="15a43-p108">除任务和计划数据外，Planner API 还能提供资源，以便跨客户端提供数据的常见可视化。有几种类型的可视化数据可用于任务：</span><span class="sxs-lookup"><span data-stu-id="15a43-p108">Aside from task and plan data, the Planner API also provides resources to provide common visualization of data across clients. Several types of visualization data are available for tasks:</span></span>

| <span data-ttu-id="15a43-131">任务如下所示</span><span class="sxs-lookup"><span data-stu-id="15a43-131">Tasks are shown as</span></span>                                                                        | <span data-ttu-id="15a43-132">使用以下信息对任务进行排序</span><span class="sxs-lookup"><span data-stu-id="15a43-132">Tasks are ordered with information from</span></span>                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| <span data-ttu-id="15a43-133">简单列表（计划中的任务）</span><span class="sxs-lookup"><span data-stu-id="15a43-133">Flat list (tasks in a plan)</span></span>                                                               | <span data-ttu-id="15a43-134">任务的 `orderHint` 属性</span><span class="sxs-lookup"><span data-stu-id="15a43-134">`orderHint` property on tasks</span></span>                                                   |
| <span data-ttu-id="15a43-135">简单列表（分配给用户的任务）</span><span class="sxs-lookup"><span data-stu-id="15a43-135">Flat list (tasks assigned to a user)</span></span>                                                      | <span data-ttu-id="15a43-136">任务的 `assigneePriority` 属性</span><span class="sxs-lookup"><span data-stu-id="15a43-136">`assigneePriority` property on tasks</span></span>                                            |
| <span data-ttu-id="15a43-137">包含受理人列的板块视图（分配给任务板块）</span><span class="sxs-lookup"><span data-stu-id="15a43-137">Board view with columns for assignees (assigned to task board)</span></span>                            | <span data-ttu-id="15a43-138">[assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) 对象</span><span class="sxs-lookup"><span data-stu-id="15a43-138">[assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) object</span></span> |
| <span data-ttu-id="15a43-139">包含针对完成情况的任务进度列的板块视图（进度任务板块）</span><span class="sxs-lookup"><span data-stu-id="15a43-139">Board view with columns for progress of the task towards completion (progress task board)</span></span> | <span data-ttu-id="15a43-140">[progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) 对象</span><span class="sxs-lookup"><span data-stu-id="15a43-140">[progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) object</span></span>     |
| <span data-ttu-id="15a43-141">包含任务自定义列的板块视图（存储桶任务板块）</span><span class="sxs-lookup"><span data-stu-id="15a43-141">Board view with custom columns of tasks (bucket task board):</span></span>                              | <span data-ttu-id="15a43-142">[bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) 对象</span><span class="sxs-lookup"><span data-stu-id="15a43-142">[bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) object</span></span>         |

<span data-ttu-id="15a43-143">存储桶任务板块中的自定义栏由 [bucket](plannerbucket.md) 对象表示，其顺序由对象的 `orderHint` 属性表示。</span><span class="sxs-lookup"><span data-stu-id="15a43-143">The custom columns in the bucket task board are represented by [bucket](plannerbucket.md) objects, and their order by `orderHint` property on the object.</span></span>

<span data-ttu-id="15a43-144">所有排序均由 [Planner 顺序提示](planner-order-hint-format.md)中的原则指定。</span><span class="sxs-lookup"><span data-stu-id="15a43-144">All the ordering is controlled by the principles identified in [Planner order hints](planner-order-hint-format.md).</span></span>

## <span data-ttu-id="15a43-145"><a name="delta">使用增量查询的修订</a></span><span class="sxs-lookup"><span data-stu-id="15a43-145"><a name="delta">Track changes using delta query</a></span></span>

<span data-ttu-id="15a43-146">计划工具的增量查询支持用户订阅的查询对象。</span><span class="sxs-lookup"><span data-stu-id="15a43-146">Planner's delta query supports querying objects that the user is subscribed to.</span></span>

<span data-ttu-id="15a43-147">用户已订阅的下列对象。</span><span class="sxs-lookup"><span data-stu-id="15a43-147">Users are subscribed to the following objects.</span></span>

| <span data-ttu-id="15a43-148">计划工具资源类型</span><span class="sxs-lookup"><span data-stu-id="15a43-148">Planner resource type</span></span> | <span data-ttu-id="15a43-149">已订阅的实例</span><span class="sxs-lookup"><span data-stu-id="15a43-149">Subscribed instances</span></span>                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="15a43-150">任务</span><span class="sxs-lookup"><span data-stu-id="15a43-150">Tasks</span></span>                 | <ul><li><span data-ttu-id="15a43-151">创建用户</span><span class="sxs-lookup"><span data-stu-id="15a43-151">Created by the user</span></span></li><li><span data-ttu-id="15a43-152">分配给用户</span><span class="sxs-lookup"><span data-stu-id="15a43-152">Assigned to the user</span></span></li><li><span data-ttu-id="15a43-153">属于用户拥有的计划</span><span class="sxs-lookup"><span data-stu-id="15a43-153">Belong to a plan that the user owns</span></span></li><li><span data-ttu-id="15a43-154">包含在用户通过计划的**SharedWith**集合与共享的计划</span><span class="sxs-lookup"><span data-stu-id="15a43-154">Contained in a plan shared with the user through the plan's **SharedWith** collection</span></span></li> |
| <span data-ttu-id="15a43-155">计划</span><span class="sxs-lookup"><span data-stu-id="15a43-155">Plans</span></span>                 | <ul><li><span data-ttu-id="15a43-156">用户通过计划的**SharedWith**集合与共享</span><span class="sxs-lookup"><span data-stu-id="15a43-156">Shared with the user through the plan's **SharedWith** collection</span></span></li></ul>                                                                                                                     |
| <span data-ttu-id="15a43-157">存储桶</span><span class="sxs-lookup"><span data-stu-id="15a43-157">Buckets</span></span>               | <ul><li><span data-ttu-id="15a43-158">包含在用户通过计划的**SharedWith**集合与共享的计划</span><span class="sxs-lookup"><span data-stu-id="15a43-158">Contained in a plan shared with the user through the plan's **SharedWith** collection</span></span></li></ul>                                                                                                 |  |

### <span data-ttu-id="15a43-159"><a name="objectcache">填充增量查询的对象缓存</a></span><span class="sxs-lookup"><span data-stu-id="15a43-159"><a name="objectcache">Populate the object cache for delta queries</a></span></span>

<span data-ttu-id="15a43-160">如果您想要使用的计划程序增量查询 API，维护本地缓存的用户感兴趣观察以应用所做的更改增量响应动态订阅源中的对象。</span><span class="sxs-lookup"><span data-stu-id="15a43-160">If you want to use the Planner delta query API, maintain a local cache of objects that the user is interested in observing in order to apply the changes from the delta response feed.</span></span>

<span data-ttu-id="15a43-161">计划增量查询当前可返回的增量负载对象将为下列类型的：</span><span class="sxs-lookup"><span data-stu-id="15a43-161">The delta payload objects that the Planner delta query can currently return will be of the following types:</span></span>

* [<span data-ttu-id="15a43-162">plannerTask</span><span class="sxs-lookup"><span data-stu-id="15a43-162">plannerTask</span></span>](plannertask.md)
* [<span data-ttu-id="15a43-163">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="15a43-163">plannerTaskDetails</span></span>](plannertaskdetails.md)
* [<span data-ttu-id="15a43-164">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="15a43-164">plannerPlan</span></span>](plannerplan.md)
* [<span data-ttu-id="15a43-165">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="15a43-165">plannerPlanDetails</span></span>](plannerplandetails.md)
* [<span data-ttu-id="15a43-166">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="15a43-166">plannerBucket</span></span>](plannerbucket.md)
* [<span data-ttu-id="15a43-167">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="15a43-167">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)
* [<span data-ttu-id="15a43-168">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="15a43-168">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)
* [<span data-ttu-id="15a43-169">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="15a43-169">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)

<span data-ttu-id="15a43-170">使用相应`GET`上要获取要填充到本地缓存的对象的初始状态的资源的方法。</span><span class="sxs-lookup"><span data-stu-id="15a43-170">Use the corresponding `GET` methods on the resource to obtain the initial state of objects to be populated into the local cache.</span></span>

### <a name="differentiating-between-object-creation-and-object-modification"></a><span data-ttu-id="15a43-171">区分对象创建和修改对象</span><span class="sxs-lookup"><span data-stu-id="15a43-171">Differentiating between object creation and object modification</span></span>

<span data-ttu-id="15a43-172">在某些情况下，呼叫者可能想要区分对象创建和计划程序的源的增量查询中的对象修改。</span><span class="sxs-lookup"><span data-stu-id="15a43-172">In certain scenarios, the caller might want to distinguish between object creation and object modification within Planner's delta query feed.</span></span>

<span data-ttu-id="15a43-173">可以使用这些准则推断对象创建：</span><span class="sxs-lookup"><span data-stu-id="15a43-173">These guidelines can be used to infer object creation:</span></span>

* <span data-ttu-id="15a43-174">`createdBy`属性才会显示在新创建的对象。</span><span class="sxs-lookup"><span data-stu-id="15a43-174">The `createdBy` property will only appear on newly created objects.</span></span>
* <span data-ttu-id="15a43-175">新创建的`plannerTask`对象的后面将带有由其对应`plannerTaskDetails`对象。</span><span class="sxs-lookup"><span data-stu-id="15a43-175">A newly created `plannerTask` object will be followed by its corresponding `plannerTaskDetails` object.</span></span>
* <span data-ttu-id="15a43-176">新创建的`plannerPlan`对象的后面将带有由其对应`plannerPlanDetails`对象。</span><span class="sxs-lookup"><span data-stu-id="15a43-176">A newly created `plannerPlan` object will be followed by its corresponding `plannerPlanDetails` object.</span></span>

### <a name="usage"></a><span data-ttu-id="15a43-177">用法</span><span class="sxs-lookup"><span data-stu-id="15a43-177">Usage</span></span>

<span data-ttu-id="15a43-178">呼叫者都应包含已订阅的对象缓存。</span><span class="sxs-lookup"><span data-stu-id="15a43-178">The caller is expected to have a cache containing subscribed objects.</span></span> <span data-ttu-id="15a43-179">有关如何填充订阅对象的本地高速缓存的详细信息，请参阅[填充增量查询的对象缓存](#populate-the-object-cache-for-delta-queries)。</span><span class="sxs-lookup"><span data-stu-id="15a43-179">For details about how to fill the local cache of subscribed objects, see [Populate the object cache for delta queries](#populate-the-object-cache-for-delta-queries).</span></span>

<span data-ttu-id="15a43-180">计划工具的增量查询呼叫流如下所示：</span><span class="sxs-lookup"><span data-stu-id="15a43-180">Planner's delta query call flow is as follows:</span></span>

1. <span data-ttu-id="15a43-181">呼叫者启动增量同步查询，获取`nextLink`和更改一个空集合。</span><span class="sxs-lookup"><span data-stu-id="15a43-181">The caller initiates a delta sync query, obtaining a `nextLink` and an empty collection of changes.</span></span>
2. <span data-ttu-id="15a43-182">呼叫者必须[填充增量查询的对象缓存](#populate-the-object-cache-for-delta-queries)使用的对象的用户订阅，更新其缓存。</span><span class="sxs-lookup"><span data-stu-id="15a43-182">The caller must [populate the object cache for delta queries](#populate-the-object-cache-for-delta-queries) with objects that the user is subscribed to, updating its cache.</span></span>
3. <span data-ttu-id="15a43-183">呼叫者遵循`nextLink`中获取新的初始增量同步查询提供`deltaLink`到上一步后的任何更改。</span><span class="sxs-lookup"><span data-stu-id="15a43-183">The caller follows the `nextLink` provided in the initial delta sync query to obtain a new `deltaLink` to any changes since previous step.</span></span>
4. <span data-ttu-id="15a43-184">呼叫者应用其缓存中的对象的返回的增量响应中的更改。</span><span class="sxs-lookup"><span data-stu-id="15a43-184">The caller applies the changes in the returned delta response to the objects in its cache.</span></span>
5. <span data-ttu-id="15a43-185">呼叫者获取下一个 deltaLink 新 deltaLink 并更改以来当前`deltaLink`生成。</span><span class="sxs-lookup"><span data-stu-id="15a43-185">The caller follows the new deltaLink to obtain the next deltaLink and changes since the current `deltaLink` was generated.</span></span>
6. <span data-ttu-id="15a43-186">呼叫者应用所做的更改 （如果有），并在重新运行以前之前等待的短时间步骤和此步骤。</span><span class="sxs-lookup"><span data-stu-id="15a43-186">The caller applies the changes (if any) and waits a short time before rerunning the previous step and this step.</span></span>

## <a name="planner-resource-versioning"></a><span data-ttu-id="15a43-187">Planner 资源版本控制</span><span class="sxs-lookup"><span data-stu-id="15a43-187">Planner resource versioning</span></span>

<span data-ttu-id="15a43-188">计划工具版本使用**etag**的所有资源。</span><span class="sxs-lookup"><span data-stu-id="15a43-188">Planner versions all resources using **etags**.</span></span> <span data-ttu-id="15a43-189">这些**etag**返回了`@odata.etag`有关每个资源的属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-189">These **etags** are returned with `@odata.etag` property on each resource.</span></span> <span data-ttu-id="15a43-190">`PATCH`和`DELETE`请求需要已知由客户端使用指定的最后一个**etag** `If-Match`标头。</span><span class="sxs-lookup"><span data-stu-id="15a43-190">`PATCH` and `DELETE` requests require the last **etag** known by the client to be specified with a `If-Match` header.</span></span>
<span data-ttu-id="15a43-191">如果预期的更改不与更高版本上相同的资源的计划程序服务所接受的更改冲突，计划工具允许更改旧版本的资源。</span><span class="sxs-lookup"><span data-stu-id="15a43-191">Planner allows changes to older versions of resources if the intended change does not conflict with newer changes accepted by the Planner service on the same resource.</span></span> <span data-ttu-id="15a43-192">客户端可以标识为相同的资源的**etag**较新的计算的**etag**值大于中的序号字符串比较。</span><span class="sxs-lookup"><span data-stu-id="15a43-192">The clients can identify which **etag** for the same resource is newer by calculating which **etag** value is greater in ordinal string comparison.</span></span> <span data-ttu-id="15a43-193">每个资源具有唯一的**etag**。</span><span class="sxs-lookup"><span data-stu-id="15a43-193">Each resource has a unique **etag**.</span></span> <span data-ttu-id="15a43-194">有关不同的资源，包括那些具有内嵌关系的 Etag 值不能进行比较。</span><span class="sxs-lookup"><span data-stu-id="15a43-194">Etag values for different resources, including those with containment relationships, cannot be compared.</span></span>
<span data-ttu-id="15a43-195">客户端应用程序应处理版本控制通过读取该项目的最新版本和解决冲突更改相关[错误代码](/graph/errors) **409**和**412** 。</span><span class="sxs-lookup"><span data-stu-id="15a43-195">The client apps are expected to handle versioning related [error codes](/graph/errors) **409** and **412** by reading the latest version of the item and resolving the conflicting changes.</span></span>

## <a name="common-planner-error-conditions"></a><span data-ttu-id="15a43-196">常见的 Planner 错误条件</span><span class="sxs-lookup"><span data-stu-id="15a43-196">Common Planner error conditions</span></span>

<span data-ttu-id="15a43-197">除了适用于 Microsoft Graph 的[常规错误](/graph/errors)外，某些错误条件特定于 Planner API。</span><span class="sxs-lookup"><span data-stu-id="15a43-197">In addition to [general errors](/graph/errors) that apply to Microsoft Graph, some error conditions are specific to the Planner API.</span></span>

### <a name="400-bad-request"></a><span data-ttu-id="15a43-198">400 错误的请求</span><span class="sxs-lookup"><span data-stu-id="15a43-198">400 Bad request</span></span>

<span data-ttu-id="15a43-p111">在几种常见情况下，`POST` 和 `PATCH` 请求可能收到 400 状态代码。常见问题包括：</span><span class="sxs-lookup"><span data-stu-id="15a43-p111">There are several common cases where the `POST` and `PATCH` requests can get a 400 status code. Common problems include:</span></span>

* <span data-ttu-id="15a43-201">打开类型属性不是正确的类型。</span><span class="sxs-lookup"><span data-stu-id="15a43-201">Open Type properties are not of correct types.</span></span>
* <span data-ttu-id="15a43-202">不指定的类型。</span><span class="sxs-lookup"><span data-stu-id="15a43-202">The type isn't specified.</span></span>
* <span data-ttu-id="15a43-203">请求不包含任何属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-203">The request does not contain any properties.</span></span>

#### <a name="example"></a><span data-ttu-id="15a43-204">示例</span><span class="sxs-lookup"><span data-stu-id="15a43-204">Example</span></span>

<span data-ttu-id="15a43-205">具有复杂的值的[plannerAssignments](plannerassignments.md)属性需要声明`@odata.type`属性值与`microsoft.graph.plannerAssignment`。</span><span class="sxs-lookup"><span data-stu-id="15a43-205">[plannerAssignments](plannerassignments.md) properties with complex values need to declare `@odata.type` property with value `microsoft.graph.plannerAssignment`.</span></span>

* <span data-ttu-id="15a43-206">顺序提示值不具有[正确的格式](planner-order-hint-format.md)。</span><span class="sxs-lookup"><span data-stu-id="15a43-206">Order hint values do not have the [correct format](planner-order-hint-format.md).</span></span>

   <span data-ttu-id="15a43-207">例如，直接向返回到客户端的值设置顺序提示值。</span><span class="sxs-lookup"><span data-stu-id="15a43-207">For example, an order hint value is being set directly to the value returned to the client.</span></span>

* <span data-ttu-id="15a43-208">数据是逻辑不一致。</span><span class="sxs-lookup"><span data-stu-id="15a43-208">The data is logically inconsistent.</span></span>

   <span data-ttu-id="15a43-209">例如，任务的开始日期是晚于截止任务日期。</span><span class="sxs-lookup"><span data-stu-id="15a43-209">For example, start date of task is later than due date of the task.</span></span>

### <a name="planner-error-status-codes"></a><span data-ttu-id="15a43-210">计划工具错误状态代码</span><span class="sxs-lookup"><span data-stu-id="15a43-210">Planner error status codes</span></span>

<span data-ttu-id="15a43-211">常规错误状态代码，除了计划程序通过返回以下代码指示特殊的错误条件。</span><span class="sxs-lookup"><span data-stu-id="15a43-211">In addition to general error status codes, Planner indicates special error conditions by returning the following codes.</span></span>

#### <a name="403-forbidden"></a><span data-ttu-id="15a43-212">403 已禁止</span><span class="sxs-lookup"><span data-stu-id="15a43-212">403 Forbidden</span></span>

<span data-ttu-id="15a43-213">计划工具 API 返回的**403**状态代码时已超出服务定义的限制。</span><span class="sxs-lookup"><span data-stu-id="15a43-213">The Planner API returns the **403** status code when a service-defined limit has been exceeded.</span></span> <span data-ttu-id="15a43-214">在这种情况下，`code`错误资源类型上的属性，指示请求超过此限制的类型。</span><span class="sxs-lookup"><span data-stu-id="15a43-214">In this case, the `code` property on the error resource type indicates the type of the limit exceeded by the request.</span></span>
<span data-ttu-id="15a43-215">限制类型的可能值包括：</span><span class="sxs-lookup"><span data-stu-id="15a43-215">The possible values for the limit types include:</span></span>

| <span data-ttu-id="15a43-216">值</span><span class="sxs-lookup"><span data-stu-id="15a43-216">Value</span></span>                         | <span data-ttu-id="15a43-217">说明</span><span class="sxs-lookup"><span data-stu-id="15a43-217">Description</span></span>                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="15a43-218">MaximumProjectsOwnedByUser</span><span class="sxs-lookup"><span data-stu-id="15a43-218">MaximumProjectsOwnedByUser</span></span>    | <span data-ttu-id="15a43-p113">已超出组所有的最大 Plan 数限制。此限制基于 [plannerPlan](plannerplan.md) 资源上的 `owner` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p113">The maximum number of Plans owned by a group limit has been exceeded. This limit is based on the `owner` property on the [plannerPlan](plannerplan.md) resource.</span></span>                                         |
| <span data-ttu-id="15a43-221">MaximumProjectsSharedWithUser</span><span class="sxs-lookup"><span data-stu-id="15a43-221">MaximumProjectsSharedWithUser</span></span> | <span data-ttu-id="15a43-p114">已超出与用户共享的最大 Plan 数限制。此限制基于 [plannerPlanDetails](plannerplandetails.md) 资源上的 `sharedWith` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p114">The maximum number of Plans shared with a user limit has been exceeded.  This limit is based on the `sharedWith` property on the [plannerPlanDetails](plannerplandetails.md) resource.</span></span>                   |
| <span data-ttu-id="15a43-224">MaximumTasksCreatedByUser</span><span class="sxs-lookup"><span data-stu-id="15a43-224">MaximumTasksCreatedByUser</span></span>     | <span data-ttu-id="15a43-p115">已超出用户创建的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `createdBy` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p115">The maximum number of Tasks created by a user limit has been exceeded. This limit is based on the `createdBy` property on the [plannerTask](plannertask.md) resource.</span></span>                                    |
| <span data-ttu-id="15a43-227">MaximumTasksAssignedToUser</span><span class="sxs-lookup"><span data-stu-id="15a43-227">MaximumTasksAssignedToUser</span></span>    | <span data-ttu-id="15a43-p116">已超出分配给用户的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `assignments` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p116">The maximum number of Tasks assigned to a user limit has been exceeded. This limit is based on the `assignments` property on the [plannerTask](plannertask.md) resource.</span></span>                                 |
| <span data-ttu-id="15a43-230">MaximumTasksInProject</span><span class="sxs-lookup"><span data-stu-id="15a43-230">MaximumTasksInProject</span></span>         | <span data-ttu-id="15a43-p117">已超出 Plan 中的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `planId` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p117">The maximum number of Tasks in a Plan limit has been exceeded. This limit is based on the `planId` property on the [plannerTask](plannertask.md) resource.</span></span>                                               |
| <span data-ttu-id="15a43-233">MaximumActiveTasksInProject</span><span class="sxs-lookup"><span data-stu-id="15a43-233">MaximumActiveTasksInProject</span></span>   | <span data-ttu-id="15a43-p118">已超出 Plan 中未完成的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `planId` 和 `percentComplete` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p118">The maximum number of Tasks that aren't completed in a Plan limit has been exceeded. This limit is based on the `planId` and `percentComplete` properties on the [plannerTask](plannertask.md) resource.</span></span> |
| <span data-ttu-id="15a43-236">MaximumBucketsInProject</span><span class="sxs-lookup"><span data-stu-id="15a43-236">MaximumBucketsInProject</span></span>       | <span data-ttu-id="15a43-p119">已超出 Plan 中的最大 Bucket 数限制。此限制基于 [plannerBucket](plannerbucket.md) 资源上的 `planId` 属性。</span><span class="sxs-lookup"><span data-stu-id="15a43-p119">The maximum number of Buckets in a Plan limit has been exceeded. This limit is based on the `planId` property on the [plannerBucket](plannerbucket.md) resource.</span></span>                                         |
| <span data-ttu-id="15a43-239">MaximumUsersSharedWithProject</span><span class="sxs-lookup"><span data-stu-id="15a43-239">MaximumUsersSharedWithProject</span></span> | <span data-ttu-id="15a43-240">[plannerPlanDetails](plannerplandetails.md) 资源上的 `sharedWith` 属性包含的值过多。</span><span class="sxs-lookup"><span data-stu-id="15a43-240">The `sharedWith` property on the [plannerPlanDetails](plannerplandetails.md) resource contains too many values.</span></span>                                                                                          |
| <span data-ttu-id="15a43-241">MaximumReferencesOnTask</span><span class="sxs-lookup"><span data-stu-id="15a43-241">MaximumReferencesOnTask</span></span>       | <span data-ttu-id="15a43-242">[plannerTaskDetails](plannertaskdetails.md) 资源上的 `references` 属性包含的值过多。</span><span class="sxs-lookup"><span data-stu-id="15a43-242">The `references` property on the [plannerTaskDetails](plannertaskdetails.md) resource contains too many values.</span></span>                                                                                          |
| <span data-ttu-id="15a43-243">MaximumChecklistItemsOnTask</span><span class="sxs-lookup"><span data-stu-id="15a43-243">MaximumChecklistItemsOnTask</span></span>   | <span data-ttu-id="15a43-244">[plannerTaskDetails](plannertaskdetails.md) 资源上的 `checklist` 属性包含的值过多。</span><span class="sxs-lookup"><span data-stu-id="15a43-244">The `checklist` property on the [plannerTaskDetails](plannertaskdetails.md) resource contains too many values.</span></span>                                                                                           |
| <span data-ttu-id="15a43-245">MaximumAssigneesInTasks</span><span class="sxs-lookup"><span data-stu-id="15a43-245">MaximumAssigneesInTasks</span></span>       | <span data-ttu-id="15a43-246">[plannerTask](plannertask.md) 资源上的 `assignments` 属性包含的值过多。</span><span class="sxs-lookup"><span data-stu-id="15a43-246">The `assignments` property on the [plannerTask](plannertask.md) resource contains too many values.</span></span>                                                                                                       |
| <span data-ttu-id="15a43-247">MaximumFavoritePlansForUser</span><span class="sxs-lookup"><span data-stu-id="15a43-247">MaximumFavoritePlansForUser</span></span>   | <span data-ttu-id="15a43-248">`favoritePlanReferences`属性对[plannerUser](planneruser.md)资源包含值太多。</span><span class="sxs-lookup"><span data-stu-id="15a43-248">The `favoritePlanReferences` property on the [plannerUser](planneruser.md) resource contains too many values.</span></span>                                                                                            |
| <span data-ttu-id="15a43-249">MaximumRecentPlansForUser</span><span class="sxs-lookup"><span data-stu-id="15a43-249">MaximumRecentPlansForUser</span></span>     | <span data-ttu-id="15a43-250">`recentPlanReferences`属性对[plannerUser](planneruser.md)资源包含值太多。</span><span class="sxs-lookup"><span data-stu-id="15a43-250">The `recentPlanReferences` property on the [plannerUser](planneruser.md) resource contains too many values.</span></span>                                                                                              |
| <span data-ttu-id="15a43-251">MaximumContextsOnPlan</span><span class="sxs-lookup"><span data-stu-id="15a43-251">MaximumContextsOnPlan</span></span>         | <span data-ttu-id="15a43-252">`contexts`属性对[plannerPlan](plannerplan.md)资源包含值太多。</span><span class="sxs-lookup"><span data-stu-id="15a43-252">The `contexts` property on the [plannerPlan](plannerplan.md) resource contains too many values.</span></span>                                                                                                          |

#### <a name="412-precondition-failed"></a><span data-ttu-id="15a43-253">412 前提条件不满足 (Precondition Failed)</span><span class="sxs-lookup"><span data-stu-id="15a43-253">412 Precondition Failed</span></span>

<span data-ttu-id="15a43-p120">Planner API 中的所有 `POST`、`PATCH` 和 `DELETE` 请求需要使用受请求约束的资源中可见的最后一个 etag 值指定 `If-Match` 标头。此外，如果请求中指定的 etag 值不再匹配服务中资源的版本，可以返回 412 状态代码。在这种情况下，客户端应该再次读取资源并获取新的 etag。</span><span class="sxs-lookup"><span data-stu-id="15a43-p120">All `POST`, `PATCH` and `DELETE` requests in Planner API require `If-Match` header to be specified with the last etag value seen of the resource that is subject to the request. Additionally, 412 status code can be returned if the etag value specified in the request no longer matches a version of the resource in the service. In this case, the clients should read the resource again and obtain a new etag.</span></span>

