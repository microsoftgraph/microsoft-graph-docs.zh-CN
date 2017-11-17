# <a name="assignedplan-resource-type"></a><span data-ttu-id="7416d-101">assignedPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="7416d-101">assignedPlan resource type</span></span>

<span data-ttu-id="7416d-102">[用户](user.md) 实体和 [组织](organization.md) 实体的 **AssignedPlans** 属性都是一个 **assignedPlan** 集合。</span><span class="sxs-lookup"><span data-stu-id="7416d-102">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="7416d-103">属性</span><span class="sxs-lookup"><span data-stu-id="7416d-103">Properties</span></span>
| <span data-ttu-id="7416d-104">属性</span><span class="sxs-lookup"><span data-stu-id="7416d-104">Property</span></span>     | <span data-ttu-id="7416d-105">类型</span><span class="sxs-lookup"><span data-stu-id="7416d-105">Type</span></span>   |<span data-ttu-id="7416d-106">说明</span><span class="sxs-lookup"><span data-stu-id="7416d-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7416d-107">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="7416d-107">assignedDateTime</span></span>|<span data-ttu-id="7416d-108">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7416d-108">DateTimeOffset</span></span>|<span data-ttu-id="7416d-p101">分配计划的日期和时间；例如：2013-01-02T19:32:30Z。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7416d-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7416d-112">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="7416d-112">capabilityStatus</span></span>|<span data-ttu-id="7416d-113">String</span><span class="sxs-lookup"><span data-stu-id="7416d-113">String</span></span>|<span data-ttu-id="7416d-114">例如，“Enabled”。</span><span class="sxs-lookup"><span data-stu-id="7416d-114">For example, “Enabled”.</span></span>|
|<span data-ttu-id="7416d-115">服务</span><span class="sxs-lookup"><span data-stu-id="7416d-115">service</span></span>|<span data-ttu-id="7416d-116">String</span><span class="sxs-lookup"><span data-stu-id="7416d-116">String</span></span>|<span data-ttu-id="7416d-117">服务名称；例如，“Exchange”。</span><span class="sxs-lookup"><span data-stu-id="7416d-117">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="7416d-118">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="7416d-118">servicePlanId</span></span>|<span data-ttu-id="7416d-119">Guid</span><span class="sxs-lookup"><span data-stu-id="7416d-119">Guid</span></span>|<span data-ttu-id="7416d-120">用于标识服务计划的 GUID。</span><span class="sxs-lookup"><span data-stu-id="7416d-120">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7416d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7416d-121">JSON representation</span></span>

<span data-ttu-id="7416d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7416d-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
