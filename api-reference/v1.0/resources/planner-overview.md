---
title: 使用 Planner REST API
description: 可以使用 Microsoft Graph 中的 Planner API 创建任务，并将其分配给 Microsoft 365 中某个群组的用户。
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: cf17b796f8689467b04d1ea814192d1f499b15cc
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420703"
---
# <a name="use-the-planner-rest-api"></a>使用 Planner REST API

可以使用 Microsoft Graph 中的 Planner API 创建任务，并将其分配给 Microsoft 365 中某个群组的用户。

在开始使用 Planner API 之前，了解主对象相互之间以及与 Microsoft 365 组之间的关系将会有所帮助。

## <a name="plan-containers"></a>Plan 容器
在 Microsoft Planner 中，计划始终被包含在另一个资源中。 包含该计划的资源决定了该计划和其中所有任务的授权规则，以及该计划的生命周期。 例如，对于 Microsoft 365 组包含的计划，组成员可以在计划中创建、编辑、解析和删除任务，还可以更改某些计划级属性（例如计划名称或标签名称）。 另外，删除组时，会自动删除组中的所有计划，如果恢复组，则会自动恢复所有计划。

最常见的容器类型是 Microsoft 365 组。

### <a name="container-type-microsoft-365-groups"></a>容器类型：Microsoft 365 组

计划通常包含在 Planner API 中的 Microsoft 365 组中。
若要[获取组所有的计划](../api/plannergroup-list-plans.md)，请发出以下 HTTP 请求。

``` http
GET /groups/{group-id}/planner/plans
```

[创建新计划](../api/planner-post-plans.md)时，请在计划对象上设置 **容器** 属性，使组成为其容器。 计划必须包含在支持的资源中。

>**注意：** 正在创建计划的用户必须是将包含计划的组的成员。 使用“[创建组](../api/group-post-groups.md)”创建新组时，系统不会将你添加为组成员。 创建组后，使用“[组帖子成员](../api/group-post-members.md)”将自己添加为成员。

## <a name="plans"></a>计划

[计划](plannerplan.md)是[任务](plannertask.md)的容器。
若要 [在计划中创建任务](../api/planner-post-tasks.md)，请在创建任务时将任务对象上的 **planId** 属性设置为计划的 ID。
目前无法在没有计划的情况下创建任务。
若要[检索计划的任务](../api/plannerplan-list-tasks.md)，请发出以下 HTTP 请求。

``` http
GET /planner/plans/{plan-id}/tasks
```

## <a name="tasks"></a>任务

通过在任务对象的 [assignments](plannerassignments.md) 属性中添加 [分配](plannerassignment.md)，可以将每个任务分配给用户。要分配任务的用户 ID 是 **分配** 时打开属性的名称，且必须指定分配的 **orderHint** 属性。

## <a name="task-and-plan-details"></a>任务和计划详细信息 

Planner 资源会排列到基本对象和详细对象中。基本对象提供对适合列表视图的资源的通用属性的访问权限，而详细对象提供对适合深化视图的资源的大型属性的访问权限。

## <a name="visualization"></a>可视化

除任务和计划数据外，Planner API 还能提供资源，以便跨客户端创建数据的常见可视化。 有几种类型的可视化数据可用于如下表中所列的任务。

| 任务如下所示                                                                        | 使用以下信息对任务进行排序                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| 简单列表（计划中的任务）                                                               | 任务的 **orderHint** 属性                                                   |
| 简单列表（分配给用户的任务）                                                      | 任务的 **assigneePriority** 属性                                            |
| 包含受理人列的板块视图（分配给任务板块）                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) 对象 |
| 包含针对完成情况的任务进度列的板块视图（进度任务板块） | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) 对象     |
| 包含任务自定义列的板块视图（存储桶任务板块）                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) 对象         |

存储桶任务板中的自定义列由 [存储桶](plannerbucket.md) 对象表示，其顺序由对象的 **orderHint** 属性表示。

所有排序均由 [Planner 顺序提示](planner-order-hint-format.md)中介绍的原则指定。

## <a name="planner-resource-versioning"></a>Planner 资源版本控制

Planner 使用 etag 对所有资源进行版本控制。 这些 etag 在每个资源上返回 **@odata.etag** 属性。 `PATCH` 和 `DELETE` 请求要求使用 `If-Match` 标头指定客户端已知的最后一个 etag。
如果目标更改与相同资源上的 Planner 服务接受的较新更改不冲突，则 Planner 允许对资源的旧版本进行更改。 客户端可以通过计算顺序字符串比较中的较大 etag 值，确定在相同的资源中，哪个 etag 较新。 每个资源都有唯一的 etag。 不同资源的 etag 值（包括具有包含关系的 etag 值）无法比较。
按预期，客户端应用程序需要通过读取项的最新版本处理与[错误代码](/graph/errors) `409` 和 `412` 相关的版本控制，并解决冲突的更改。

## <a name="common-planner-error-conditions"></a>常见的 Planner 错误条件

除了适用于 Microsoft Graph 的[常规错误](/graph/errors)外，某些错误条件特定于 Planner API。

### <a name="400-bad-request"></a>400 错误的请求

在某些常见方案中，`POST` 和 `PATCH` 请求可能会返回 400 状态代码。 以下是一些常见原因：

* 开放类型属性的类型不正确，或该类型未指定，或它们不包含任何属性。例如，包含复杂值的 [plannerAssignments](plannerassignments.md) 属性需要声明包含 `microsoft.graph.plannerAssignment` 值的 **@odata.type** 属性。
* 顺序提示值不具有正确格式。例如，顺序提示值被直接设置为返回到客户端的值。
* 数据在逻辑上不一致。例如，任务的开始日期晚于任务的到期日期。

### <a name="403-forbidden"></a>403 已禁止

除常规错误外，当超出服务定义的限制时，Planner API 也会返回 `403` 状态代码。 如果出现这种情况，错误资源类型上的 **代码** 属性将标识请求超出的限制类型。
以下是限制类型的可能值。

| 值                         | 说明                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | 已超出组包含的最大 Plan 数限制。 此限制适用于基于 [plannerPlan](plannerplan.md) 资源的 **容器** 属性的组包含的计划。                                         |
| MaximumProjectsSharedWithUser | 已超出与用户共享的最大计划数限制。此限制基于 [plannerPlanDetails](plannerplandetails.md) 资源上的 **sharedWith** 属性。                   |
| MaximumTasksCreatedByUser     | 已超出用户创建的最大任务数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 **createdBy** 属性。                                    |
| MaximumTasksAssignedToUser    | 已超出分配给用户的最大任务数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 **assignments** 属性。                                 |
| MaximumTasksInProject         | 已超出计划中的最大任务数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 **planId** 属性。                                               |
| MaximumActiveTasksInProject   | 已超出计划中未完成的最大任务数限制。此限制基于 [plannerTask](plannertask.md) 资源上的 **planId** 和 **percentComplete** 属性。 |
| MaximumBucketsInProject       | 已超出计划中的最大存储桶数限制。此限制基于 [plannerBucket](plannerbucket.md) 资源上的 **planId** 属性。                                         |
| MaximumUsersSharedWithProject | [plannerPlanDetails](plannerplandetails.md) 资源上的 **sharedWith** 属性包含的值过多。                                                                                          |
| MaximumReferencesOnTask       | [plannerTaskDetails](plannertaskdetails.md) 资源上的 **references** 属性包含的值过多。                                                                                          |
| MaximumChecklistItemsOnTask   | [plannerTaskDetails](plannertaskdetails.md) 资源上的 **checklist** 属性包含的值过多。                                                                                           |
| MaximumAssigneesInTasks       | [plannerTask](plannertask.md) 资源上的 **assignments** 属性包含的值过多。                                                                                                       |
| MaximumPlannerPlans       | 组已包含一个 **计划**。 目前，组只能包含一个 **计划**。 **注意：** 某些 Microsoft 应用程序可能超出此限制。 将来，我们会将此功能扩展到所有应用程序。                                                                                                      |

### <a name="412-precondition-failed"></a>412 前提条件不满足 

所有 Planner API `POST`、`PATCH` 和 `DELETE` 请求都需要使用受请求约束的资源的最后一个已知 etag 值指定 `If-Match` 标头。
如果请求中指定的 etag 值不再匹配服务中资源的版本，也会返回 412 状态代码。 在这种情况下，客户端应该再次读取资源并获取新的 etag。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

