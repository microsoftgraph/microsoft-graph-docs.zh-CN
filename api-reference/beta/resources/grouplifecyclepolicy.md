---
title: groupLifecyclePolicy 资源类型
description: 表示 Office 365 组的生命周期策略。 使用组生命周期策略，管理员可以为组设置到期期限。 例如，组在 180 天后到期。 如果组到期，组的所有者必须在管理员定义的时间段内续订组。 续订后，组的有效期就会延长策略中定义的天数。 例如，续订后，组的新到期时间是在 180 天后。 如果不续订组，组就会到期并被删除。 可以在删除后的 30 天内还原组。
ms.openlocfilehash: c4a4d5b495f3bbb0d0c55b61a259f2105d0fea9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044915"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="e7a68-110">groupLifecyclePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7a68-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="e7a68-111">表示 Office 365 组的生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="e7a68-111">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="e7a68-112">使用组生命周期策略，管理员可以为组设置到期期限。</span><span class="sxs-lookup"><span data-stu-id="e7a68-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="e7a68-113">例如，组在 180 天后到期。</span><span class="sxs-lookup"><span data-stu-id="e7a68-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="e7a68-114">如果组到期，组的所有者必须在管理员定义的时间段内续订组。</span><span class="sxs-lookup"><span data-stu-id="e7a68-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="e7a68-115">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="e7a68-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="e7a68-116">例如，续订后，组的新到期时间是在 180 天后。</span><span class="sxs-lookup"><span data-stu-id="e7a68-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="e7a68-117">如果不续订组，组就会到期并被删除。</span><span class="sxs-lookup"><span data-stu-id="e7a68-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="e7a68-118">可以在删除后的 30 天内还原组。</span><span class="sxs-lookup"><span data-stu-id="e7a68-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="e7a68-119">方法</span><span class="sxs-lookup"><span data-stu-id="e7a68-119">Methods</span></span>

| <span data-ttu-id="e7a68-120">方法</span><span class="sxs-lookup"><span data-stu-id="e7a68-120">Method</span></span> | <span data-ttu-id="e7a68-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7a68-121">Return Type</span></span> | <span data-ttu-id="e7a68-122">说明</span><span class="sxs-lookup"><span data-stu-id="e7a68-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7a68-123">获取 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="e7a68-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="e7a68-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="e7a68-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="e7a68-125">读取 groupLifecyclePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7a68-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="e7a68-126">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="e7a68-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="e7a68-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7a68-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="e7a68-128">列出所有 groupLifecyclePolicy。</span><span class="sxs-lookup"><span data-stu-id="e7a68-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="e7a68-129">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="e7a68-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="e7a68-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="e7a68-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="e7a68-131">更新 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e7a68-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="e7a68-132">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="e7a68-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="e7a68-133">无</span><span class="sxs-lookup"><span data-stu-id="e7a68-133">None</span></span> | <span data-ttu-id="e7a68-134">删除 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e7a68-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="e7a68-135">向 groupLifecyclePolicy 添加组</span><span class="sxs-lookup"><span data-stu-id="e7a68-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="e7a68-136">无</span><span class="sxs-lookup"><span data-stu-id="e7a68-136">None</span></span>| <span data-ttu-id="e7a68-137">向生命周期策略添加组</span><span class="sxs-lookup"><span data-stu-id="e7a68-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="e7a68-138">从 groupLifecyclePolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="e7a68-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="e7a68-139">无</span><span class="sxs-lookup"><span data-stu-id="e7a68-139">None</span></span>| <span data-ttu-id="e7a68-140">从生命周期策略中删除组</span><span class="sxs-lookup"><span data-stu-id="e7a68-140">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="e7a68-141">续订组</span><span class="sxs-lookup"><span data-stu-id="e7a68-141">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="e7a68-142">无</span><span class="sxs-lookup"><span data-stu-id="e7a68-142">None</span></span>| <span data-ttu-id="e7a68-143">续订组的到期日期。</span><span class="sxs-lookup"><span data-stu-id="e7a68-143">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7a68-144">属性</span><span class="sxs-lookup"><span data-stu-id="e7a68-144">Properties</span></span>

| <span data-ttu-id="e7a68-145">属性</span><span class="sxs-lookup"><span data-stu-id="e7a68-145">Property</span></span> | <span data-ttu-id="e7a68-146">类型</span><span class="sxs-lookup"><span data-stu-id="e7a68-146">Type</span></span> | <span data-ttu-id="e7a68-147">说明</span><span class="sxs-lookup"><span data-stu-id="e7a68-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e7a68-148">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="e7a68-148">alternateNotificationEmails</span></span>|<span data-ttu-id="e7a68-149">String</span><span class="sxs-lookup"><span data-stu-id="e7a68-149">String</span></span>| <span data-ttu-id="e7a68-150">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="e7a68-150">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="e7a68-151">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e7a68-151">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="e7a68-152">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="e7a68-152">groupLifetimeInDays</span></span>|<span data-ttu-id="e7a68-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e7a68-153">Int32</span></span>| <span data-ttu-id="e7a68-154">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="e7a68-154">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="e7a68-155">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="e7a68-155">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="e7a68-156">id</span><span class="sxs-lookup"><span data-stu-id="e7a68-156">id</span></span>|<span data-ttu-id="e7a68-157">Guid</span><span class="sxs-lookup"><span data-stu-id="e7a68-157">Guid</span></span>| <span data-ttu-id="e7a68-158">策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e7a68-158">A unique identifier for a policy.</span></span> <span data-ttu-id="e7a68-159">只读。</span><span class="sxs-lookup"><span data-stu-id="e7a68-159">Read-only.</span></span>|
|<span data-ttu-id="e7a68-160">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="e7a68-160">managedGroupTypes</span></span>|<span data-ttu-id="e7a68-161">String</span><span class="sxs-lookup"><span data-stu-id="e7a68-161">String</span></span>| <span data-ttu-id="e7a68-162">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="e7a68-162">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="e7a68-163">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="e7a68-163">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e7a68-164">关系</span><span class="sxs-lookup"><span data-stu-id="e7a68-164">Relationships</span></span>

<span data-ttu-id="e7a68-165">无。</span><span class="sxs-lookup"><span data-stu-id="e7a68-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7a68-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7a68-166">JSON representation</span></span>

<span data-ttu-id="e7a68-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7a68-167">Here is a JSON representation of the resource.</span></span>

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