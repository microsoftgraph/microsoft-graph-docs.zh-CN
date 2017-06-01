# <a name="planner"></a>Planner
Office 365 Planner API 让你可以创建任务并将其分配给 Office 365 中某个组的用户。

开始尝试 Planner API 之前，需要了解 Planner API 中主对象互相之间以及与 Office 365 组的关系。

## <a name="groups"></a>组
Office 365 组是 Planner API 中的计划的所有者。若要[获取组所有的计划](../api/plannergroup_list_plans.md)，请发出下面的 HTTP 请求。

```http
GET /groups/{id}/planner/plans
```

[创建新计划](../api/planner_post_plans.md)时，只需在计划对象上设置 `owner` 属性即可使组成为其所有者。计划必须归组所有。

>**注意：**正在创建计划的用户必须是组的成员。使用 API 创建新组时，系统不会将你自动添加为组成员。必须使用单独的 API 调用才能完成此操作。

## <a name="plans"></a>计划
[计划](plannerplan.md)是[任务](plannertask.md)的容器。若要[在计划中创建一个任务](../api/planner_post_tasks.md)，在创建任务时，将任务对象中的 `planId` 属性设置为计划的 ID。目前无法在没有计划的情况下创建任务。若要[检索计划的任务](../api/plannerplan_list_tasks.md)，请发出下面的 HTTP 请求。

```http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>任务
可以通过在任务对象的 [assignments](plannerassignments.md) 属性中添加[分配](plannerassignment.md)将每个任务分配给一位用户。要分配任务的用户 ID 是 `assignments` 上的开放属性的名称，且必须指定分配上的 `orderHint` 属性。

## <a name="task-and-plan-details"></a>任务和计划详细信息 
Planner 资源会排列到基本对象和详细对象中。基本对象提供对适合列表视图的资源的通用属性的访问权限，而详细对象提供对适合深化视图的资源的大型属性的访问权限。

## <a name="visualization"></a>可视化
除任务和计划数据外，Planner API 还能提供资源，以便跨客户端提供数据的常见可视化。有几种类型的可视化数据可用于任务：

| 任务如下所示      | 使用以下信息对任务进行排序|
|:------------------|:----------|
|简单列表（计划中的任务）| 任务的 `orderHint` 属性|
|简单列表（分配给用户的任务）| 任务的 `assigneePriority` 属性|
|包含受理人列的板块视图（分配给任务板块）| [assignedToTaskBoardTaskFormat](plannerassignedToTaskBoardTaskFormat.md) 对象|
|包含针对完成情况的任务进度列的板块视图（进度任务板块）| [progressTaskBoardTaskFormat](plannerprogressTaskBoardTaskFormat.md) 对象|
|包含任务自定义列的板块视图（存储桶任务板块）|[bucketTaskBoardTaskFormat](plannerbucketTaskBoardTaskFormat.md) 对象|

存储桶任务板块中的自定义栏由 [bucket](plannerbucket.md) 对象表示，其顺序由对象的 `orderHint` 属性表示。

所有排序均由 [Planner 顺序提示](planner_order_hint_format.md)中的原则指定。

## <a name="planner-resource-versioning"></a>Planner 资源版本控制

Planner 使用 etag 对所有资源进行版本控制。这些 etags 与每个资源的 `@odata.etag` 属性一起返回，且 `PATCH` 和 `DELETE` 请求需要使用 `If-Match` 标头指定客户端已知的最后一个 etag。如果目标更改与相同资源上的 Planner 服务接受的较新更改不冲突，则 Planner 允许对资源的旧版本进行更改。客户端可以通过计算顺序字符串比较中的较大 etag 值，确定在相同的资源中，哪个 etag 较新。每个资源都有单独的 etag。不同资源的 etag 值（包括具有包含关系的 etag 值）无法比较。按预期，客户端应用需要通过读取项的最新版本处理与错误状态代码 409 和 412 相关的两个版本控制，并解决冲突的更改。

## <a name="common-planner-error-conditions"></a>常见的 Planner 错误条件

除了适用于 Microsoft Graph 的[常规错误](../../../concepts/errors.md)外，某些错误条件特定于 Planner API。

### <a name="400-bad-request"></a>400 错误的请求

在几种常见情况下，`POST` 和 `PATCH` 请求可能收到 400 状态代码。常见问题包括：
* 开放类型属性的类型不正确，或该类型未指定，或它们不包含任何属性。例如，包含复杂值的 [plannerAssignments](plannerAssignments.md) 属性需要声明包含 `microsoft.graph.plannerAssignment` 值的 `@odata.type` 属性。
* 顺序提示值不具有[正确格式](planner_order_hint_format.md)。例如，顺序提示值被直接设置为返回到客户端的值。
* 数据在逻辑上不一致。例如，任务的开始日期晚于任务的到期日期。

### <a name="403-forbidden"></a>403 已禁止

除常规错误外，当超出服务定义的限制时，Planner API 还会返回此状态代码。如果出现这种情况，错误资源类型上的 `code` 属性将标识请求超出的限制类型。限制类型的可能值包括：

| 值  | 说明|
|:------------------|:----------|
|MaximumProjectsOwnedByUser|已超出组所有的最大 Plan 数限制。此限制基于 [plannerPlan](plannerPlan.md) 资源上的 `owner` 属性。|
|MaximumProjectsSharedWithUser|已超出与用户共享的最大 Plan 数限制。此限制基于 [plannerPlanDetails](plannerPlanDetails.md) 资源上的 `sharedWith` 属性。|
|MaximumTasksCreatedByUser|已超出用户创建的最大 Task 数限制。此限制基于 [plannerTask](plannerTask.md) 资源上的 `createdBy` 属性。|
|MaximumTasksAssignedToUser|已超出分配给用户的最大 Task 数限制。此限制基于 [plannerTask](plannerTask.md) 资源上的 `assignments` 属性。|
|MaximumTasksInProject|已超出 Plan 中的最大 Task 数限制。此限制基于 [plannerTask](plannerTask.md) 资源上的 `planId` 属性。|
|MaximumActiveTasksInProject|已超出 Plan 中未完成的最大 Task 数限制。此限制基于 [plannerTask](plannerTask.md) 资源上的 `planId` 和 `percentComplete` 属性。|
|MaximumBucketsInProject|已超出 Plan 中的最大 Bucket 数限制。此限制基于 [plannerBucket](plannerBucket.md) 资源上的 `planId` 属性。|
|MaximumUsersSharedWithProject|[plannerPlanDetails](plannerPlanDetails.md) 资源上的 `sharedWith` 属性包含的值过多。|
|MaximumReferencesOnTask|[plannerTaskDetails](plannerTaskDetails.md) 资源上的 `references` 属性包含的值过多。|
|MaximumChecklistItemsOnTask|[plannerTaskDetails](plannerTaskDetails.md) 资源上的 `checklist` 属性包含的值过多。|
|MaximumAssigneesInTasks|[plannerTask](plannerTask.md) 资源上的 `assignments` 属性包含的值过多。|

### <a name="412-precondition-failed"></a>412 前提条件不满足 (Precondition Failed) 

Planner API 中的所有 `POST`、`PATCH` 和 `DELETE` 请求需要使用受请求约束的资源中可见的最后一个 etag 值指定 `If-Match` 标头。此外，如果请求中指定的 etag 值不再匹配服务中资源的版本，可以返回 412 状态代码。在这种情况下，客户端应该再次读取资源并获取新的 etag。

