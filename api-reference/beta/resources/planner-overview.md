---
title: 使用 Planner REST API
description: 可以使用 Microsoft Graph 中的 Planner API 创建任务，并将其分配给 Microsoft 365 中某个群组的用户。
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 18c8f9a7bb418c849a5ac2255f8931ff3ec84a50
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695334"
---
# <a name="use-the-planner-rest-api"></a>使用 Planner REST API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以使用 Microsoft Graph 中的 Planner API 创建任务，并将其分配给 Microsoft 365 中某个群组的用户。

在开始使用 Planner API 之前，了解主对象相互之间以及与 Microsoft 365 组之间的关系将会有所帮助。

## <a name="plan-containers"></a>Plan 容器
在 Planner 中，计划总是包含在另一个资源中。 包含的资源决定了计划和其中所有任务的授权规则，以及计划的生命周期。 例如，对于 Microsoft 365 组包含的计划，组成员可以在计划中创建、编辑、解析和删除任务，还可以更改某些计划级属性（例如计划名称或标签名称）。 另外，删除组时，会自动删除组中的所有计划，如果恢复组，则会自动恢复所有计划。

最常见的容器类型是 Microsoft 365 组。

### <a name="container-type-microsoft-365-groups"></a>容器类型：Microsoft 365 组

计划通常包含在 Planner API 中的 Microsoft 365 组中。
若要[获取组所有的计划](../api/plannergroup-list-plans.md)，请发出以下 HTTP 请求。

``` http
GET /groups/{group-id}/planner/plans
```

[创建新计划](../api/planner-post-plans.md)时，通过在计划对象上设置 `container` 属性，可使组成为其容器。 计划必须包含在支持的资源中。

>**注意：** 正在创建计划的用户必须是将包含计划的组的成员。 使用“[创建组](../api/group-post-groups.md)”创建新组时，系统不会将你添加为组成员。 创建组后，使用“[组帖子成员](../api/group-post-members.md)”将自己添加为成员。

## <a name="plans"></a>计划

[计划](plannerplan.md)是[任务](plannertask.md)的容器。
若要[在计划中创建一个任务](../api/planner-post-tasks.md)，在创建任务时，将任务对象中的 `planId` 属性设置为计划的 ID。
目前无法在没有计划的情况下创建任务。
若要[检索计划的任务](../api/plannerplan-list-tasks.md)，请发出以下 HTTP 请求。

``` http
GET /planner/plans/{plan-id}/tasks
```

## <a name="tasks"></a>任务

可以通过在任务对象的 [assignments](plannerassignments.md) 属性中添加[分配](plannerassignment.md)将每个任务分配给一位用户。要分配任务的用户 ID 是 `assignments` 上的开放属性的名称，且必须指定分配上的 `orderHint` 属性。

## <a name="task-and-plan-details"></a>任务和计划详细信息

Planner 资源会排列到基本对象和详细对象中。基本对象提供对适合列表视图的资源的通用属性的访问权限，而详细对象提供对适合深化视图的资源的大型属性的访问权限。

## <a name="visualization"></a>可视化

除任务和计划数据外，Planner API 还能提供资源，以便跨客户端创建数据的常见可视化。 有几种类型的可视化数据可用于如下表中所列的任务。

| 任务如下所示                                                                        | 使用以下信息对任务进行排序                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| 简单列表（计划中的任务）                                                               | 任务的 `orderHint` 属性                                                   |
| 简单列表（分配给用户的任务）                                                      | 任务的 `assigneePriority` 属性                                            |
| 包含受理人列的板块视图（分配给任务板块）                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) 对象 |
| 包含针对完成情况的任务进度列的板块视图（进度任务板块） | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) 对象     |
| 包含任务自定义列的板块视图（存储桶任务板块）                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) 对象         |

存储桶任务板块中的自定义栏由 [bucket](plannerbucket.md) 对象表示，其顺序由对象的 `orderHint` 属性表示。

所有排序均由 [Planner 顺序提示](planner-order-hint-format.md)中介绍的原则指定。

## <a name=""></a><a name="delta">使用 delta 查询跟踪更改</a>

Planner 的 delta 查询功能支持查询用户订阅的对象。

用户订阅了以下对象。

| Planner 资源类型 | 已订阅的实例                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 任务                 | <ul><li>由用户创建</li><li>已分配给用户</li><li>属于用户拥有的计划</li><li>包含在通过计划的 **SharedWith** 集合与用户共享的计划中</li> |
| 计划                 | <ul><li>通过计划的 **SharedWith** 集合与用户共享</li></ul>                                                                                                                     |
| Buckets               | <ul><li>包含在通过计划的 **SharedWith** 集合与用户共享的计划中</li></ul>                                                                                                 |

### <a name=""></a><a name="objectcache">填充 delta 查询的对象缓存</a>

如果要使用 Planner delta 查询 API，请保留用户有兴趣查看的对象的本地缓存，以便应用 delta 响应源中的更改。

Planner delta 查询当前可以返回的 delta 有效负载对象将为以下类型：

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

使用资源中的相应 `GET` 方法获取要填充到本地缓存的对象初始状态。

### <a name="differentiating-between-object-creation-and-object-modification"></a>区分对象创建和对象修改

在某些情况下，调用方可能希望区分 Planner 的 delta 查询源中的对象创建和对象修改。

可使用以下准则推断对象创建：

* `createdBy` 属性仅出现在新创建的对象上。
* 新创建的 `plannerTask` 对象后面将跟随其对应的 `plannerTaskDetails` 对象。
* 新创建的 `plannerPlan` 对象后面将跟随其对应的 `plannerPlanDetails` 对象。

### <a name="usage"></a>用法

调用方期望有一个包含订阅对象的缓存。 有关如何填充订阅对象的本地缓存的详细信息，请参阅[填充 delta 查询的对象缓存](#populate-the-object-cache-for-delta-queries)。

Planner 的 delta 查询调用流如下所示：

1. 调用方启动 delta 同步查询，以便获取 `nextLink` 和空的更改集合。
2. 调用方必须使用用户订阅的对象[填充 delta 查询的对象缓存](#populate-the-object-cache-for-delta-queries)，从而更新其缓存。
3. 调用方遵循初始 delta 同步查询中提供的 `nextLink`，以便获得自上一步以来所做的任何更改的新 `deltaLink`。
4. 调用方将返回的 delta 响应中的更改应用于其缓存中的对象。
5. 调用方遵循新的 deltaLink 以获取下一个 deltaLink，以及自生成当前 `deltaLink` 以来所做的更改。
6. 调用方应用更改（如果有）并等待一小段时间，然后重新执行上一步和此步骤。

## <a name="planner-resource-versioning"></a>Planner 资源版本控制

Planner 使用 **etag** 对所有资源进行版本控制。 这些 **etag** 在每个资源上返回 `@odata.etag` 属性。 `PATCH` 和 `DELETE` 请求要求使用 `If-Match` 标头指定客户端已知的最后一个 **etag**。
如果目标更改与相同资源上的 Planner 服务接受的较新更改不冲突，则 Planner 允许对资源的旧版本进行更改。 客户端可以通过计算顺序字符串比较中的较大 **etag** 值，确定在相同的资源中，哪个 **etag** 较新。
每个资源都有唯一的 **etag**。 不同资源的 etag 值（包括具有包含关系的 etag 值）无法比较。
按预期，客户端应用程序需要通过读取项的最新版本处理与 [错误代码](/graph/errors) **409** 和 **412** 相关的版本控制，并解决冲突的更改。

## <a name="common-planner-error-conditions"></a>常见的 Planner 错误条件

除了适用于 Microsoft Graph 的[常规错误](/graph/errors)外，某些错误条件特定于 Planner API。

### <a name="400-bad-request"></a>400 错误的请求

在某些常见方案中，`POST` 和 `PATCH` 请求可能会返回 400 状态代码。 以下是一些常见原因：

* 开放类型属性的类型不正确，或该类型未指定，或它们不包含任何属性。例如，包含复杂值的 plannerAssignments 属性需要声明包含  值的  属性。
* 顺序提示值不具有正确格式。例如，顺序提示值被直接设置为返回到客户端的值。
* 数据在逻辑上不一致。例如，任务的开始日期晚于任务的到期日期。

### <a name="403-forbidden"></a>403 已禁止

除常规错误外，当超出服务定义的限制时，Planner API 也会返回 403 状态代码。 如果出现这种情况，错误资源类型上的 `code` 属性将标识请求超出的限制类型。
以下是限制类型的可能值。

| 值                         | 说明                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | 已超出组所有的最大 Plan 数限制。此限制基于 [plannerPlan](plannerplan.md) 资源上的 `owner` 属性。                                         |
| MaximumProjectsSharedWithUser | 已超出与用户共享的最大 Plan 数限制。此限制基于 [plannerPlanDetails](plannerplandetails.md) 资源上的 `sharedWith` 属性。                   |
| MaximumTasksCreatedByUser     | 已超出用户创建的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `createdBy` 属性。                                    |
| MaximumTasksAssignedToUser    | 已超出分配给用户的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `assignments` 属性。                                 |
| MaximumTasksInProject         | 已超出 Plan 中的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `planId` 属性。                                               |
| MaximumActiveTasksInProject   | 已超出 Plan 中未完成的最大 Task 数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 `planId` 和 `percentComplete` 属性。 |
| MaximumBucketsInProject       | 已超出 Plan 中的最大 Bucket 数限制。此限制基于 [plannerBucket](plannerbucket.md) 资源上的 `planId` 属性。                                         |
| MaximumUsersSharedWithProject | [plannerPlanDetails](plannerplandetails.md) 资源上的 `sharedWith` 属性包含的值过多。                                                                                          |
| MaximumReferencesOnTask       | [plannerTaskDetails](plannertaskdetails.md) 资源上的 `references` 属性包含的值过多。                                                                                          |
| MaximumChecklistItemsOnTask   | [plannerTaskDetails](plannertaskdetails.md) 资源上的 `checklist` 属性包含的值过多。                                                                                           |
| MaximumAssigneesInTasks       | [plannerTask](plannertask.md) 资源上的 `assignments` 属性包含的值过多。                                                                                                       |
| MaximumFavoritePlansForUser   | [plannerUser](planneruser.md) 资源上的 `favoritePlanReferences` 属性包含的值过多。                                                                                            |
| MaximumRecentPlansForUser     | [plannerUser](planneruser.md) 资源上的 `recentPlanReferences` 属性包含的值过多。                                                                                              |
| MaximumContextsOnPlan         | [plannerPlan](plannerplan.md) 资源上的 `contexts` 属性包含的值过多。                                                                                                          |
| MaximumPlannerPlans       | 组已包含一个计划。 目前，组只能包含一个计划。 **注意：** 某些 Microsoft 应用程序可能超出此限制。 将来，我们会将此功能扩展到所有应用程序。                                                                                                      |

### <a name="412-precondition-failed"></a>412 前提条件不满足

所有 Planer API `POST`、`PATCH` 和 `DELETE` 请求都需要使用受请求约束的资源的最后一个已知 etag 值指定 `If-Match` 标头。
如果请求中指定的 etag 值不再匹配服务中资源的版本，也会返回 412 状态代码。 在这种情况下，客户端应该再次读取资源并获取新的 etag。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

