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
# <a name="use-the-planner-rest-api"></a>使用进度表 REST API

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

可以使用在 Microsoft Graph 计划程序 API 创建任务并将其分配给 Office 365 中的某个组中的用户。

在开始使用规划器 API 之前，值得的了解如何的主要对象相互以及来对 Office 365 组。

## <a name="groups"></a>Groups

Office 365 组都是计划工具 API 中计划的所有者。
为[获取一组由拥有的计划](../api/plannergroup-list-plans.md)，进行以下的 HTTP 请求。

``` http
GET /groups/{id}/planner/plans
```

当[创建新的计划](../api/planner-post-plans.md)，通过设置指定给计划组所有者`owner`计划对象的属性。 必须由组拥有计划。 组可以拥有多个计划。

>**注意：** 正在创建计划的用户必须将拥有计划的组的成员。 当使用[创建组](../api/group-post-groups.md)创建一个新的组时，您不是添加到组，作为成员。 创建组后，将自己添加为成员使用[组发布成员](../api/group-post-members.md)。

## <a name="plans"></a>计划

[计划](plannerplan.md)的[任务](plannertask.md)的容器。 对[创建在计划任务](../api/planner-post-tasks.md)，请设置`planId`task 对象创建任务时计划的 id 属性。
当前无法不带计划创建任务。
对[检索计划中的任务](../api/plannerplan-list-tasks.md)，请进行以下的 HTTP 请求。

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>任务

可以通过在任务对象的 [assignments](plannerassignments.md) 属性中添加[分配](plannerassignment.md)将每个任务分配给一位用户。要分配任务的用户 ID 是 `assignments` 上的开放属性的名称，且必须指定分配上的 `orderHint` 属性。

## <a name="task-and-plan-details"></a>任务和计划详细信息 

计划工具资源排列到基本任务和计划对象和详细任务和计划对象。 基本对象提供的资源，适用于列表视图的详细信息对象提供对适用于深化视图的资源的大型属性访问时的常见属性的访问权限。

## <a name="visualization"></a>可视化

除任务和计划数据外，Planner API 还能提供资源，以便跨客户端提供数据的常见可视化。有几种类型的可视化数据可用于任务：

| 任务如下所示                                                                        | 使用以下信息对任务进行排序                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| 简单列表（计划中的任务）                                                               | 任务的 `orderHint` 属性                                                   |
| 简单列表（分配给用户的任务）                                                      | 任务的 `assigneePriority` 属性                                            |
| 包含受理人列的板块视图（分配给任务板块）                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) 对象 |
| 包含针对完成情况的任务进度列的板块视图（进度任务板块） | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) 对象     |
| 包含任务自定义列的板块视图（存储桶任务板块）                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) 对象         |

存储桶任务板块中的自定义栏由 [bucket](plannerbucket.md) 对象表示，其顺序由对象的 `orderHint` 属性表示。

所有排序均由 [Planner 顺序提示](planner-order-hint-format.md)中的原则指定。

## <a name="delta">使用增量查询的修订</a>

计划工具的增量查询支持用户订阅的查询对象。

用户已订阅的下列对象。

| 计划工具资源类型 | 已订阅的实例                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 任务                 | <ul><li>创建用户</li><li>分配给用户</li><li>属于用户拥有的计划</li><li>包含在用户通过计划的**SharedWith**集合与共享的计划</li> |
| 计划                 | <ul><li>用户通过计划的**SharedWith**集合与共享</li></ul>                                                                                                                     |
| 存储桶               | <ul><li>包含在用户通过计划的**SharedWith**集合与共享的计划</li></ul>                                                                                                 |  |

### <a name="objectcache">填充增量查询的对象缓存</a>

如果您想要使用的计划程序增量查询 API，维护本地缓存的用户感兴趣观察以应用所做的更改增量响应动态订阅源中的对象。

计划增量查询当前可返回的增量负载对象将为下列类型的：

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

使用相应`GET`上要获取要填充到本地缓存的对象的初始状态的资源的方法。

### <a name="differentiating-between-object-creation-and-object-modification"></a>区分对象创建和修改对象

在某些情况下，呼叫者可能想要区分对象创建和计划程序的源的增量查询中的对象修改。

可以使用这些准则推断对象创建：

* `createdBy`属性才会显示在新创建的对象。
* 新创建的`plannerTask`对象的后面将带有由其对应`plannerTaskDetails`对象。
* 新创建的`plannerPlan`对象的后面将带有由其对应`plannerPlanDetails`对象。

### <a name="usage"></a>用法

呼叫者都应包含已订阅的对象缓存。 有关如何填充订阅对象的本地高速缓存的详细信息，请参阅[填充增量查询的对象缓存](#populate-the-object-cache-for-delta-queries)。

计划工具的增量查询呼叫流如下所示：

1. 呼叫者启动增量同步查询，获取`nextLink`和更改一个空集合。
2. 呼叫者必须[填充增量查询的对象缓存](#populate-the-object-cache-for-delta-queries)使用的对象的用户订阅，更新其缓存。
3. 呼叫者遵循`nextLink`中获取新的初始增量同步查询提供`deltaLink`到上一步后的任何更改。
4. 呼叫者应用其缓存中的对象的返回的增量响应中的更改。
5. 呼叫者获取下一个 deltaLink 新 deltaLink 并更改以来当前`deltaLink`生成。
6. 呼叫者应用所做的更改 （如果有），并在重新运行以前之前等待的短时间步骤和此步骤。

## <a name="planner-resource-versioning"></a>Planner 资源版本控制

计划工具版本使用**etag**的所有资源。 这些**etag**返回了`@odata.etag`有关每个资源的属性。 `PATCH`和`DELETE`请求需要已知由客户端使用指定的最后一个**etag** `If-Match`标头。
如果预期的更改不与更高版本上相同的资源的计划程序服务所接受的更改冲突，计划工具允许更改旧版本的资源。 客户端可以标识为相同的资源的**etag**较新的计算的**etag**值大于中的序号字符串比较。 每个资源具有唯一的**etag**。 有关不同的资源，包括那些具有内嵌关系的 Etag 值不能进行比较。
客户端应用程序应处理版本控制通过读取该项目的最新版本和解决冲突更改相关[错误代码](/graph/errors) **409**和**412** 。

## <a name="common-planner-error-conditions"></a>常见的 Planner 错误条件

除了适用于 Microsoft Graph 的[常规错误](/graph/errors)外，某些错误条件特定于 Planner API。

### <a name="400-bad-request"></a>400 错误的请求

在几种常见情况下，`POST` 和 `PATCH` 请求可能收到 400 状态代码。常见问题包括：

* 打开类型属性不是正确的类型。
* 不指定的类型。
* 请求不包含任何属性。

#### <a name="example"></a>示例

具有复杂的值的[plannerAssignments](plannerassignments.md)属性需要声明`@odata.type`属性值与`microsoft.graph.plannerAssignment`。

* 顺序提示值不具有[正确的格式](planner-order-hint-format.md)。

   例如，直接向返回到客户端的值设置顺序提示值。

* 数据是逻辑不一致。

   例如，任务的开始日期是晚于截止任务日期。

### <a name="planner-error-status-codes"></a>计划工具错误状态代码

常规错误状态代码，除了计划程序通过返回以下代码指示特殊的错误条件。

#### <a name="403-forbidden"></a>403 已禁止

计划工具 API 返回的**403**状态代码时已超出服务定义的限制。 在这种情况下，`code`错误资源类型上的属性，指示请求超过此限制的类型。
限制类型的可能值包括：

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
| MaximumFavoritePlansForUser   | `favoritePlanReferences`属性对[plannerUser](planneruser.md)资源包含值太多。                                                                                            |
| MaximumRecentPlansForUser     | `recentPlanReferences`属性对[plannerUser](planneruser.md)资源包含值太多。                                                                                              |
| MaximumContextsOnPlan         | `contexts`属性对[plannerPlan](plannerplan.md)资源包含值太多。                                                                                                          |

#### <a name="412-precondition-failed"></a>412 前提条件不满足 (Precondition Failed)

Planner API 中的所有 `POST`、`PATCH` 和 `DELETE` 请求需要使用受请求约束的资源中可见的最后一个 etag 值指定 `If-Match` 标头。此外，如果请求中指定的 etag 值不再匹配服务中资源的版本，可以返回 412 状态代码。在这种情况下，客户端应该再次读取资源并获取新的 etag。

