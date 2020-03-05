---
title: groupLifecyclePolicy 资源类型
description: 表示 Office 365 组的生命周期策略。 使用组生命周期策略，管理员可以为组设置到期期限。 例如，组在 180 天后到期。 如果组到期，组的所有者必须在管理员定义的时间段内续订组。 续订后，组的有效期就会延长策略中定义的天数。 例如，续订后，组的新到期时间是在 180 天后。 如果不续订组，组就会到期并被删除。 可以在删除后的 30 天内还原组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: bc98036c28deb67fdf6057d51ae075868a1d2d8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497075"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="14b90-110">groupLifecyclePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="14b90-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="14b90-111">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="14b90-111">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14b90-112">表示 Office 365 组的生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="14b90-112">Represents a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="14b90-113">使用组生命周期策略，管理员可以为组设置到期期限。</span><span class="sxs-lookup"><span data-stu-id="14b90-113">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="14b90-114">例如，组在 180 天后到期。</span><span class="sxs-lookup"><span data-stu-id="14b90-114">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="14b90-115">如果组到期，组的所有者必须在管理员定义的时间段内续订组。</span><span class="sxs-lookup"><span data-stu-id="14b90-115">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="14b90-116">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="14b90-116">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="14b90-117">例如，续订后，组的新到期时间是在 180 天后。</span><span class="sxs-lookup"><span data-stu-id="14b90-117">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="14b90-118">如果不续订组，组就会到期并被删除。</span><span class="sxs-lookup"><span data-stu-id="14b90-118">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="14b90-119">可以在删除后的 30 天内还原组。</span><span class="sxs-lookup"><span data-stu-id="14b90-119">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="14b90-120">方法</span><span class="sxs-lookup"><span data-stu-id="14b90-120">Methods</span></span>

| <span data-ttu-id="14b90-121">方法</span><span class="sxs-lookup"><span data-stu-id="14b90-121">Method</span></span> | <span data-ttu-id="14b90-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="14b90-122">Return Type</span></span> | <span data-ttu-id="14b90-123">说明</span><span class="sxs-lookup"><span data-stu-id="14b90-123">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="14b90-124">获取 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="14b90-124">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="14b90-125">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="14b90-125">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="14b90-126">读取 groupLifecyclePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="14b90-126">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="14b90-127">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="14b90-127">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="14b90-128">[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="14b90-128">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="14b90-129">列出所有 groupLifecyclePolicy。</span><span class="sxs-lookup"><span data-stu-id="14b90-129">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="14b90-130">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="14b90-130">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="14b90-131">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="14b90-131">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="14b90-132">更新 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="14b90-132">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="14b90-133">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="14b90-133">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="14b90-134">无</span><span class="sxs-lookup"><span data-stu-id="14b90-134">None</span></span> | <span data-ttu-id="14b90-135">删除 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="14b90-135">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="14b90-136">向 groupLifecyclePolicy 添加组</span><span class="sxs-lookup"><span data-stu-id="14b90-136">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="14b90-137">无</span><span class="sxs-lookup"><span data-stu-id="14b90-137">None</span></span>| <span data-ttu-id="14b90-138">向生命周期策略添加组</span><span class="sxs-lookup"><span data-stu-id="14b90-138">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="14b90-139">从 groupLifecyclePolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="14b90-139">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="14b90-140">无</span><span class="sxs-lookup"><span data-stu-id="14b90-140">None</span></span>| <span data-ttu-id="14b90-141">从生命周期策略中删除组</span><span class="sxs-lookup"><span data-stu-id="14b90-141">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="14b90-142">续订组</span><span class="sxs-lookup"><span data-stu-id="14b90-142">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="14b90-143">无</span><span class="sxs-lookup"><span data-stu-id="14b90-143">None</span></span>| <span data-ttu-id="14b90-144">续订组的到期日期。</span><span class="sxs-lookup"><span data-stu-id="14b90-144">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="14b90-145">属性</span><span class="sxs-lookup"><span data-stu-id="14b90-145">Properties</span></span>

| <span data-ttu-id="14b90-146">属性</span><span class="sxs-lookup"><span data-stu-id="14b90-146">Property</span></span> | <span data-ttu-id="14b90-147">类型</span><span class="sxs-lookup"><span data-stu-id="14b90-147">Type</span></span> | <span data-ttu-id="14b90-148">说明</span><span class="sxs-lookup"><span data-stu-id="14b90-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="14b90-149">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="14b90-149">alternateNotificationEmails</span></span>|<span data-ttu-id="14b90-150">String</span><span class="sxs-lookup"><span data-stu-id="14b90-150">String</span></span>| <span data-ttu-id="14b90-151">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="14b90-151">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="14b90-152">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="14b90-152">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="14b90-153">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="14b90-153">groupLifetimeInDays</span></span>|<span data-ttu-id="14b90-154">Int32</span><span class="sxs-lookup"><span data-stu-id="14b90-154">Int32</span></span>| <span data-ttu-id="14b90-155">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="14b90-155">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="14b90-156">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="14b90-156">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="14b90-157">id</span><span class="sxs-lookup"><span data-stu-id="14b90-157">id</span></span>|<span data-ttu-id="14b90-158">Guid</span><span class="sxs-lookup"><span data-stu-id="14b90-158">Guid</span></span>| <span data-ttu-id="14b90-159">策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="14b90-159">A unique identifier for a policy.</span></span> <span data-ttu-id="14b90-160">只读。</span><span class="sxs-lookup"><span data-stu-id="14b90-160">Read-only.</span></span>|
|<span data-ttu-id="14b90-161">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="14b90-161">managedGroupTypes</span></span>|<span data-ttu-id="14b90-162">String</span><span class="sxs-lookup"><span data-stu-id="14b90-162">String</span></span>| <span data-ttu-id="14b90-163">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="14b90-163">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="14b90-164">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="14b90-164">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="14b90-165">关系</span><span class="sxs-lookup"><span data-stu-id="14b90-165">Relationships</span></span>

<span data-ttu-id="14b90-166">无。</span><span class="sxs-lookup"><span data-stu-id="14b90-166">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14b90-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14b90-167">JSON representation</span></span>

<span data-ttu-id="14b90-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14b90-168">Here is a JSON representation of the resource.</span></span>

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
