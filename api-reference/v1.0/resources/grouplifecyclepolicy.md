# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="d4810-101">groupLifecyclePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4810-101">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="d4810-102">表示 Office 365 组的生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="d4810-102">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="d4810-103">使用组生命周期策略，管理员可以为组设置到期期限。</span><span class="sxs-lookup"><span data-stu-id="d4810-103">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="d4810-104">例如，组在 180 天后到期。</span><span class="sxs-lookup"><span data-stu-id="d4810-104">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="d4810-105">如果组到期，组的所有者必须在管理员定义的时间段内续订组。</span><span class="sxs-lookup"><span data-stu-id="d4810-105">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="d4810-106">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="d4810-106">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="d4810-107">例如，续订后，组的新到期时间是在 180 天后。</span><span class="sxs-lookup"><span data-stu-id="d4810-107">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="d4810-108">如果不续订组，组就会到期并被删除。</span><span class="sxs-lookup"><span data-stu-id="d4810-108">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="d4810-109">可以在删除后的 30 天内还原组。</span><span class="sxs-lookup"><span data-stu-id="d4810-109">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="d4810-110">方法</span><span class="sxs-lookup"><span data-stu-id="d4810-110">Methods</span></span>

| <span data-ttu-id="d4810-111">方法</span><span class="sxs-lookup"><span data-stu-id="d4810-111">Method</span></span> | <span data-ttu-id="d4810-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4810-112">Return Type</span></span> | <span data-ttu-id="d4810-113">说明</span><span class="sxs-lookup"><span data-stu-id="d4810-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4810-114">获取 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4810-114">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_get.md) | [<span data-ttu-id="d4810-115">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4810-115">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="d4810-116">读取 groupLifecyclePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4810-116">Read properties and relationships of plannerPlan object.</span></span>|
|[<span data-ttu-id="d4810-117">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4810-117">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy_list.md) | <span data-ttu-id="d4810-118">[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4810-118">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="d4810-119">列出所有 groupLifecyclePolicy。</span><span class="sxs-lookup"><span data-stu-id="d4810-119">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="d4810-120">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4810-120">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_update.md) | [<span data-ttu-id="d4810-121">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4810-121">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="d4810-122">更新 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="d4810-122">Update a setting object.</span></span> |
|[<span data-ttu-id="d4810-123">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4810-123">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_delete.md) | <span data-ttu-id="d4810-124">无</span><span class="sxs-lookup"><span data-stu-id="d4810-124">None</span></span> | <span data-ttu-id="d4810-125">删除 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="d4810-125">Delete a device object.</span></span> |
|[<span data-ttu-id="d4810-126">向 groupLifecyclePolicy 添加组</span><span class="sxs-lookup"><span data-stu-id="d4810-126">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_addgroup.md)|<span data-ttu-id="d4810-127">无</span><span class="sxs-lookup"><span data-stu-id="d4810-127">None</span></span>| <span data-ttu-id="d4810-128">向生命周期策略添加组</span><span class="sxs-lookup"><span data-stu-id="d4810-128">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="d4810-129">从 groupLifecyclePolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="d4810-129">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_removegroup.md)|<span data-ttu-id="d4810-130">无</span><span class="sxs-lookup"><span data-stu-id="d4810-130">None</span></span>| <span data-ttu-id="d4810-131">从生命周期策略中删除组</span><span class="sxs-lookup"><span data-stu-id="d4810-131">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4810-132">属性</span><span class="sxs-lookup"><span data-stu-id="d4810-132">Properties</span></span>

| <span data-ttu-id="d4810-133">属性</span><span class="sxs-lookup"><span data-stu-id="d4810-133">Property</span></span> | <span data-ttu-id="d4810-134">类型</span><span class="sxs-lookup"><span data-stu-id="d4810-134">Type</span></span> | <span data-ttu-id="d4810-135">说明</span><span class="sxs-lookup"><span data-stu-id="d4810-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d4810-136">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="d4810-136">alternateNotificationEmails</span></span>|<span data-ttu-id="d4810-137">String</span><span class="sxs-lookup"><span data-stu-id="d4810-137">String</span></span>| <span data-ttu-id="d4810-138">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="d4810-138">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="d4810-139">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d4810-139">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="d4810-140">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="d4810-140">groupLifetimeInDays</span></span>|<span data-ttu-id="d4810-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d4810-141">Int32</span></span>| <span data-ttu-id="d4810-142">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="d4810-142">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="d4810-143">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="d4810-143">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="d4810-144">id</span><span class="sxs-lookup"><span data-stu-id="d4810-144">id</span></span>|<span data-ttu-id="d4810-145">Guid</span><span class="sxs-lookup"><span data-stu-id="d4810-145">Guid</span></span>| <span data-ttu-id="d4810-146">策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d4810-146">A unique identifier for a policy.</span></span> <span data-ttu-id="d4810-147">只读。</span><span class="sxs-lookup"><span data-stu-id="d4810-147">Read-only.</span></span>|
|<span data-ttu-id="d4810-148">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="d4810-148">managedGroupTypes</span></span>|<span data-ttu-id="d4810-149">String</span><span class="sxs-lookup"><span data-stu-id="d4810-149">String</span></span>| <span data-ttu-id="d4810-150">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="d4810-150">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="d4810-151">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="d4810-151">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d4810-152">关系</span><span class="sxs-lookup"><span data-stu-id="d4810-152">Relationships</span></span>

<span data-ttu-id="d4810-153">无。</span><span class="sxs-lookup"><span data-stu-id="d4810-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4810-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4810-154">JSON representation</span></span>

<span data-ttu-id="d4810-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4810-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->