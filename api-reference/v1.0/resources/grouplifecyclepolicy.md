---
title: groupLifecyclePolicy 资源类型
description: 表示组策略的Microsoft 365策略。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: da3fa558df864f3dd0683ae4aaa08234c9ebd158
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680094"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="0304b-103">groupLifecyclePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="0304b-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="0304b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0304b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0304b-105">表示组策略的Microsoft 365策略。</span><span class="sxs-lookup"><span data-stu-id="0304b-105">Represents a lifecycle policy for a Microsoft 365 group.</span></span> <span data-ttu-id="0304b-106">使用组生命周期策略，管理员可以为组设置到期期限。</span><span class="sxs-lookup"><span data-stu-id="0304b-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="0304b-107">例如，组在 180 天后到期。</span><span class="sxs-lookup"><span data-stu-id="0304b-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="0304b-108">如果组到期，组的所有者必须在管理员定义的时间段内续订组。</span><span class="sxs-lookup"><span data-stu-id="0304b-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="0304b-109">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="0304b-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="0304b-110">例如，续订后，组的新到期时间是在 180 天后。</span><span class="sxs-lookup"><span data-stu-id="0304b-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="0304b-111">如果不续订组，组就会到期并被删除。</span><span class="sxs-lookup"><span data-stu-id="0304b-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="0304b-112">可以在删除后的 30 天内还原组。</span><span class="sxs-lookup"><span data-stu-id="0304b-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="0304b-113">方法</span><span class="sxs-lookup"><span data-stu-id="0304b-113">Methods</span></span>

| <span data-ttu-id="0304b-114">方法</span><span class="sxs-lookup"><span data-stu-id="0304b-114">Method</span></span> | <span data-ttu-id="0304b-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="0304b-115">Return Type</span></span> | <span data-ttu-id="0304b-116">说明</span><span class="sxs-lookup"><span data-stu-id="0304b-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="0304b-117">获取 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0304b-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="0304b-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0304b-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="0304b-119">读取 groupLifecyclePolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0304b-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="0304b-120">列出 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0304b-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="0304b-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0304b-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="0304b-122">列出所有 groupLifecyclePolicy。</span><span class="sxs-lookup"><span data-stu-id="0304b-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="0304b-123">更新 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0304b-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="0304b-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0304b-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="0304b-125">更新 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="0304b-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="0304b-126">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0304b-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="0304b-127">无</span><span class="sxs-lookup"><span data-stu-id="0304b-127">None</span></span> | <span data-ttu-id="0304b-128">删除 groupLifecyclePolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="0304b-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="0304b-129">向 groupLifecyclePolicy 添加组</span><span class="sxs-lookup"><span data-stu-id="0304b-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="0304b-130">无</span><span class="sxs-lookup"><span data-stu-id="0304b-130">None</span></span>| <span data-ttu-id="0304b-131">向生命周期策略添加组</span><span class="sxs-lookup"><span data-stu-id="0304b-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="0304b-132">从 groupLifecyclePolicy 中删除组</span><span class="sxs-lookup"><span data-stu-id="0304b-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="0304b-133">无</span><span class="sxs-lookup"><span data-stu-id="0304b-133">None</span></span>| <span data-ttu-id="0304b-134">从生命周期策略中删除组</span><span class="sxs-lookup"><span data-stu-id="0304b-134">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="0304b-135">属性</span><span class="sxs-lookup"><span data-stu-id="0304b-135">Properties</span></span>

| <span data-ttu-id="0304b-136">属性</span><span class="sxs-lookup"><span data-stu-id="0304b-136">Property</span></span> | <span data-ttu-id="0304b-137">类型</span><span class="sxs-lookup"><span data-stu-id="0304b-137">Type</span></span> | <span data-ttu-id="0304b-138">说明</span><span class="sxs-lookup"><span data-stu-id="0304b-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0304b-139">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="0304b-139">alternateNotificationEmails</span></span>|<span data-ttu-id="0304b-140">String</span><span class="sxs-lookup"><span data-stu-id="0304b-140">String</span></span>| <span data-ttu-id="0304b-141">针对没有所有者的组向其发送通知的电子邮件地址列表。</span><span class="sxs-lookup"><span data-stu-id="0304b-141">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="0304b-142">可以用分号隔开电子邮件地址，从而定义多个电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0304b-142">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="0304b-143">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="0304b-143">groupLifetimeInDays</span></span>|<span data-ttu-id="0304b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0304b-144">Int32</span></span>| <span data-ttu-id="0304b-145">还剩多少天组就到期且需要续订。</span><span class="sxs-lookup"><span data-stu-id="0304b-145">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="0304b-146">续订后，组的有效期就会延长定义的天数。</span><span class="sxs-lookup"><span data-stu-id="0304b-146">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="0304b-147">id</span><span class="sxs-lookup"><span data-stu-id="0304b-147">id</span></span>|<span data-ttu-id="0304b-148">Guid</span><span class="sxs-lookup"><span data-stu-id="0304b-148">Guid</span></span>| <span data-ttu-id="0304b-149">策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0304b-149">A unique identifier for a policy.</span></span> <span data-ttu-id="0304b-150">只读。</span><span class="sxs-lookup"><span data-stu-id="0304b-150">Read-only.</span></span>|
|<span data-ttu-id="0304b-151">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="0304b-151">managedGroupTypes</span></span>|<span data-ttu-id="0304b-152">String</span><span class="sxs-lookup"><span data-stu-id="0304b-152">String</span></span>| <span data-ttu-id="0304b-153">到期策略适用的组类型。</span><span class="sxs-lookup"><span data-stu-id="0304b-153">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="0304b-154">可取值为 **All**、**Selected** 或 **None**。</span><span class="sxs-lookup"><span data-stu-id="0304b-154">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0304b-155">关系</span><span class="sxs-lookup"><span data-stu-id="0304b-155">Relationships</span></span>

<span data-ttu-id="0304b-156">无。</span><span class="sxs-lookup"><span data-stu-id="0304b-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0304b-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0304b-157">JSON representation</span></span>

<span data-ttu-id="0304b-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0304b-158">Here is a JSON representation of the resource.</span></span>

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

