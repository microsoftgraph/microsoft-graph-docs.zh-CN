---
title: groupLifecyclePolicy 资源类型
description: 表示 Microsoft 365 组的生命周期策略。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d95699781e0011f26093092ceba8048f14b8e740
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897622"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="9c677-103">groupLifecyclePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c677-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="9c677-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c677-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c677-105">表示 Microsoft 365 组的生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="9c677-105">Represents a lifecycle policy for a Microsoft 365 group.</span></span> <span data-ttu-id="9c677-106">使用组生命周期策略，管理员可以为组设置到期期限。</span><span class="sxs-lookup"><span data-stu-id="9c677-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="9c677-107">例如，组在 180 天后到期。</span><span class="sxs-lookup"><span data-stu-id="9c677-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="9c677-108">如果组到期，组的所有者必须在管理员定义的时间段内续订组。</span><span class="sxs-lookup"><span data-stu-id="9c677-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="9c677-109">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="9c677-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="9c677-110">例如，续订后，组的新到期时间是在 180 天后。</span><span class="sxs-lookup"><span data-stu-id="9c677-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="9c677-111">如果不续订组，组就会到期并被删除。</span><span class="sxs-lookup"><span data-stu-id="9c677-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="9c677-112">可以在删除后的 30 天内还原组。</span><span class="sxs-lookup"><span data-stu-id="9c677-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="9c677-113">方法</span><span class="sxs-lookup"><span data-stu-id="9c677-113">Methods</span></span>

| <span data-ttu-id="9c677-114">方法</span><span class="sxs-lookup"><span data-stu-id="9c677-114">Method</span></span> | <span data-ttu-id="9c677-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="9c677-115">Return Type</span></span> | <span data-ttu-id="9c677-116">说明</span><span class="sxs-lookup"><span data-stu-id="9c677-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c677-117">获取 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9c677-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="9c677-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9c677-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="9c677-119">读取 groupLifecyclePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c677-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="9c677-120">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9c677-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="9c677-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c677-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="9c677-122">列出所有 groupLifecyclePolicy。</span><span class="sxs-lookup"><span data-stu-id="9c677-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="9c677-123">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9c677-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="9c677-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9c677-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="9c677-125">更新 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="9c677-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="9c677-126">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9c677-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="9c677-127">无</span><span class="sxs-lookup"><span data-stu-id="9c677-127">None</span></span> | <span data-ttu-id="9c677-128">删除 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="9c677-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="9c677-129">向 groupLifecyclePolicy 添加组</span><span class="sxs-lookup"><span data-stu-id="9c677-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="9c677-130">无</span><span class="sxs-lookup"><span data-stu-id="9c677-130">None</span></span>| <span data-ttu-id="9c677-131">向生命周期策略添加组</span><span class="sxs-lookup"><span data-stu-id="9c677-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="9c677-132">从 groupLifecyclePolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="9c677-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="9c677-133">无</span><span class="sxs-lookup"><span data-stu-id="9c677-133">None</span></span>| <span data-ttu-id="9c677-134">从生命周期策略中删除组</span><span class="sxs-lookup"><span data-stu-id="9c677-134">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c677-135">属性</span><span class="sxs-lookup"><span data-stu-id="9c677-135">Properties</span></span>

| <span data-ttu-id="9c677-136">属性</span><span class="sxs-lookup"><span data-stu-id="9c677-136">Property</span></span> | <span data-ttu-id="9c677-137">类型</span><span class="sxs-lookup"><span data-stu-id="9c677-137">Type</span></span> | <span data-ttu-id="9c677-138">说明</span><span class="sxs-lookup"><span data-stu-id="9c677-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9c677-139">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="9c677-139">alternateNotificationEmails</span></span>|<span data-ttu-id="9c677-140">String</span><span class="sxs-lookup"><span data-stu-id="9c677-140">String</span></span>| <span data-ttu-id="9c677-141">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="9c677-141">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="9c677-142">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9c677-142">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="9c677-143">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="9c677-143">groupLifetimeInDays</span></span>|<span data-ttu-id="9c677-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9c677-144">Int32</span></span>| <span data-ttu-id="9c677-145">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="9c677-145">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="9c677-146">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="9c677-146">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="9c677-147">id</span><span class="sxs-lookup"><span data-stu-id="9c677-147">id</span></span>|<span data-ttu-id="9c677-148">Guid</span><span class="sxs-lookup"><span data-stu-id="9c677-148">Guid</span></span>| <span data-ttu-id="9c677-149">策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9c677-149">A unique identifier for a policy.</span></span> <span data-ttu-id="9c677-150">只读。</span><span class="sxs-lookup"><span data-stu-id="9c677-150">Read-only.</span></span>|
|<span data-ttu-id="9c677-151">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="9c677-151">managedGroupTypes</span></span>|<span data-ttu-id="9c677-152">String</span><span class="sxs-lookup"><span data-stu-id="9c677-152">String</span></span>| <span data-ttu-id="9c677-153">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="9c677-153">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="9c677-154">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="9c677-154">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9c677-155">关系</span><span class="sxs-lookup"><span data-stu-id="9c677-155">Relationships</span></span>

<span data-ttu-id="9c677-156">无。</span><span class="sxs-lookup"><span data-stu-id="9c677-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c677-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c677-157">JSON representation</span></span>

<span data-ttu-id="9c677-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c677-158">Here is a JSON representation of the resource.</span></span>

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
