---
title: 使用进度表 REST API
description: 可以使用在 Microsoft Graph 计划程序 API 创建任务并将其分配给 Office 365 中的某个组中的用户。
author: TarkanSevilmis
localization_priority: Priority
ms.prod: planner
ms.openlocfilehash: 86d5c950b2e281a0af254d48a7d133d7e352341f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944087"
---
# <a name="use-the-planner-rest-api"></a>使用进度表 REST API

可以使用在 Microsoft Graph 计划程序 API 创建任务并将其分配给 Office 365 中的某个组中的用户。

在开始使用规划器 API 之前，您需要了解如何的主要对象相互以及来对 Office 365 组。

## <a name="office-365-groups"></a>Office 365 组

Office 365 组都是计划工具 API 中计划的所有者。
为[获取一组由拥有的计划](../api/plannergroup-list-plans.md)，进行以下的 HTTP 请求。

``` http
GET /groups/{id}/planner/plans
```

当[创建新的计划](../api/planner-post-plans.md)，通过设置使组所有者`owner`计划对象的属性。 必须按组拥有计划。

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

Planner 资源会排列到基本对象和详细对象中。基本对象提供对适合列表视图的资源的通用属性的访问权限，而详细对象提供对适合深化视图的资源的大型属性的访问权限。

## <a name="visualization"></a>可视化

除了任务和计划的数据，计划工具 API 还提供了资源创建客户端之间的数据的常见可视化。 下表中所列，为任务，提供了几种类型的可视化数据。

| 任务如下所示                                                                        | 使用以下信息对任务进行排序                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| 简单列表（计划中的任务）                                                               | 任务的 `orderHint` 属性                                                   |
| 简单列表（分配给用户的任务）                                                      | 任务的 `assigneePriority` 属性                                            |
| 包含受理人列的板块视图（分配给任务板块）                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) 对象 |
| 包含针对完成情况的任务进度列的板块视图（进度任务板块） | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) 对象     |
| 包含任务自定义列的板块视图（存储桶任务板块）                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) 对象         |

存储桶任务板块中的自定义栏由 [bucket](plannerbucket.md) 对象表示，其顺序由对象的 `orderHint` 属性表示。

[计划工具顺序提示](planner-order-hint-format.md)所述的原则由控制所有排序。

## <a name="planner-resource-versioning"></a>Planner 资源版本控制

计划工具版本使用**etag**的所有资源。 这些**etag**返回了`@odata.etag`有关每个资源的属性。 `PATCH`和`DELETE`请求需要已知由客户端使用指定的最后一个**etag** `If-Match`标头。
计划工具允许对较旧版本的资源，如果预期的更改不与更高版本上相同的资源的计划程序服务所接受的更改冲突。 客户端可以标识为相同的资源的**etag**较新的计算的**etag**值大于中的序号字符串比较。 每个资源具有唯一的**etag**。 有关不同的资源，包括那些具有内嵌关系的 Etag 值不能进行比较。
客户端应用程序应处理版本控制通过读取该项目的最新版本和解决冲突更改相关[错误代码](/graph/errors) **409**和**412** 。

## <a name="common-planner-error-conditions"></a>常见的 Planner 错误条件

除了适用于 Microsoft Graph 的[常规错误](/graph/errors)外，某些错误条件特定于 Planner API。

### <a name="400-bad-request"></a>400 错误的请求

在某些常见的情况下，`POST`和`PATCH`请求可返回一个 400 的状态代码。 下面是一些常见原因：

* 开放类型属性的类型不正确，或该类型未指定，或它们不包含任何属性。例如，包含复杂值的 [plannerAssignments](plannerassignments.md) 属性需要声明包含 `microsoft.graph.plannerAssignment` 值的 `@odata.type` 属性。
* 顺序提示值不具有[正确格式](planner-order-hint-format.md)。例如，顺序提示值被直接设置为返回到客户端的值。
* 数据在逻辑上不一致。例如，任务的开始日期晚于任务的到期日期。

### <a name="403-forbidden"></a>403 已禁止

除了常规错误，计划工具 API 还返回 403 状态代码时已超出服务定义的限制。 如果是这样，`code`错误资源类型上的属性将指示请求超过此限制的类型。
以下是可能的限制类型的值。

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
| MaximumPlannerPlans       | 组已包含一个计划。 目前，组只能包含一个计划。 **注意：** 某些 Microsoft 应用程序可以超过此限制。 将来，我们将此功能扩展到所有应用程序。                                                                                                      |

### <a name="412-precondition-failed"></a>412 前提条件不满足 (Precondition Failed) 

所有平面 API `POST`， `PATCH`，和`DELETE`请求需要`If-Match`标头以指定受制请求的资源的最后一个已知的 etag 值。
如果请求中指定的 etag 值不再与服务中的资源的版本相匹配，也会返回 412 状态代码。 在这种情况下，客户端应再次阅读资源并获取新的 etag。

