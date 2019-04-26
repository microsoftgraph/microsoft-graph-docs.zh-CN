---
title: groupLifecyclePolicy 资源类型
description: 表示 Office 365 组的生命周期策略。 使用组生命周期策略，管理员可以为组设置到期期限。 例如，组在 180 天后到期。 如果组到期，组的所有者必须在管理员定义的时间段内续订组。 续订后，组的有效期就会延长策略中定义的天数。 例如，续订后，组的新到期时间是在 180 天后。 如果不续订组，组就会到期并被删除。 可以在删除后的 30 天内还原组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 65cf8d5d06262f1d5700de26b4c4f62b005020d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570839"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="b4d3f-110">groupLifecyclePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4d3f-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="b4d3f-111">表示 Office 365 组的生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-111">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="b4d3f-112">使用组生命周期策略，管理员可以为组设置到期期限。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="b4d3f-113">例如，组在 180 天后到期。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="b4d3f-114">如果组到期，组的所有者必须在管理员定义的时间段内续订组。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="b4d3f-115">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="b4d3f-116">例如，续订后，组的新到期时间是在 180 天后。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="b4d3f-117">如果不续订组，组就会到期并被删除。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="b4d3f-118">可以在删除后的 30 天内还原组。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="b4d3f-119">方法</span><span class="sxs-lookup"><span data-stu-id="b4d3f-119">Methods</span></span>

| <span data-ttu-id="b4d3f-120">方法</span><span class="sxs-lookup"><span data-stu-id="b4d3f-120">Method</span></span> | <span data-ttu-id="b4d3f-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="b4d3f-121">Return Type</span></span> | <span data-ttu-id="b4d3f-122">说明</span><span class="sxs-lookup"><span data-stu-id="b4d3f-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="b4d3f-123">获取 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b4d3f-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="b4d3f-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b4d3f-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="b4d3f-125">读取 groupLifecyclePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="b4d3f-126">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b4d3f-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="b4d3f-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4d3f-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="b4d3f-128">列出所有 groupLifecyclePolicy。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="b4d3f-129">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b4d3f-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="b4d3f-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b4d3f-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="b4d3f-131">更新 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="b4d3f-132">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b4d3f-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="b4d3f-133">无</span><span class="sxs-lookup"><span data-stu-id="b4d3f-133">None</span></span> | <span data-ttu-id="b4d3f-134">删除 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="b4d3f-135">向 groupLifecyclePolicy 添加组</span><span class="sxs-lookup"><span data-stu-id="b4d3f-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="b4d3f-136">无</span><span class="sxs-lookup"><span data-stu-id="b4d3f-136">None</span></span>| <span data-ttu-id="b4d3f-137">向生命周期策略添加组</span><span class="sxs-lookup"><span data-stu-id="b4d3f-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="b4d3f-138">从 groupLifecyclePolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="b4d3f-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="b4d3f-139">无</span><span class="sxs-lookup"><span data-stu-id="b4d3f-139">None</span></span>| <span data-ttu-id="b4d3f-140">从生命周期策略中删除组</span><span class="sxs-lookup"><span data-stu-id="b4d3f-140">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="b4d3f-141">属性</span><span class="sxs-lookup"><span data-stu-id="b4d3f-141">Properties</span></span>

| <span data-ttu-id="b4d3f-142">属性</span><span class="sxs-lookup"><span data-stu-id="b4d3f-142">Property</span></span> | <span data-ttu-id="b4d3f-143">类型</span><span class="sxs-lookup"><span data-stu-id="b4d3f-143">Type</span></span> | <span data-ttu-id="b4d3f-144">说明</span><span class="sxs-lookup"><span data-stu-id="b4d3f-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b4d3f-145">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="b4d3f-145">alternateNotificationEmails</span></span>|<span data-ttu-id="b4d3f-146">String</span><span class="sxs-lookup"><span data-stu-id="b4d3f-146">String</span></span>| <span data-ttu-id="b4d3f-147">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-147">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="b4d3f-148">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-148">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="b4d3f-149">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="b4d3f-149">groupLifetimeInDays</span></span>|<span data-ttu-id="b4d3f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d3f-150">Int32</span></span>| <span data-ttu-id="b4d3f-151">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-151">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="b4d3f-152">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-152">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="b4d3f-153">id</span><span class="sxs-lookup"><span data-stu-id="b4d3f-153">id</span></span>|<span data-ttu-id="b4d3f-154">Guid</span><span class="sxs-lookup"><span data-stu-id="b4d3f-154">Guid</span></span>| <span data-ttu-id="b4d3f-155">策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-155">A unique identifier for a policy.</span></span> <span data-ttu-id="b4d3f-156">只读。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-156">Read-only.</span></span>|
|<span data-ttu-id="b4d3f-157">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="b4d3f-157">managedGroupTypes</span></span>|<span data-ttu-id="b4d3f-158">String</span><span class="sxs-lookup"><span data-stu-id="b4d3f-158">String</span></span>| <span data-ttu-id="b4d3f-159">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-159">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="b4d3f-160">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-160">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b4d3f-161">关系</span><span class="sxs-lookup"><span data-stu-id="b4d3f-161">Relationships</span></span>

<span data-ttu-id="b4d3f-162">无。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4d3f-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4d3f-163">JSON representation</span></span>

<span data-ttu-id="b4d3f-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4d3f-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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
