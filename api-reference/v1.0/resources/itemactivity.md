---
author: daspek
ms.author: dspektor
title: itemActivity 资源类型
description: ItemActivity 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 98ae9e4881de18c94490469b10df43b2aaf58140
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536685"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="78494-103">itemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="78494-103">itemActivity resource type</span></span>

<span data-ttu-id="78494-104">**ItemActivity**资源提供有关在项目或容器中发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="78494-104">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="78494-105">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="78494-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="78494-106">在 itemActivity 中发生的操作将在[itemActionSet][]属性中进行详细说明。</span><span class="sxs-lookup"><span data-stu-id="78494-106">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="78494-107">**注意:\*\*\*\*itemActivity**目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="78494-107">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="78494-109">属性</span><span class="sxs-lookup"><span data-stu-id="78494-109">Properties</span></span>

| <span data-ttu-id="78494-110">属性</span><span class="sxs-lookup"><span data-stu-id="78494-110">Property</span></span> | <span data-ttu-id="78494-111">类型</span><span class="sxs-lookup"><span data-stu-id="78494-111">Type</span></span>                    | <span data-ttu-id="78494-112">说明</span><span class="sxs-lookup"><span data-stu-id="78494-112">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="78494-113">id</span><span class="sxs-lookup"><span data-stu-id="78494-113">id</span></span>       | <span data-ttu-id="78494-114">string</span><span class="sxs-lookup"><span data-stu-id="78494-114">string</span></span>                  | <span data-ttu-id="78494-115">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="78494-115">The unique identifier of the activity.</span></span> <span data-ttu-id="78494-116">只读。</span><span class="sxs-lookup"><span data-stu-id="78494-116">Read-only.</span></span>
| <span data-ttu-id="78494-117">访问</span><span class="sxs-lookup"><span data-stu-id="78494-117">access</span></span>   | <span data-ttu-id="78494-118">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="78494-118">[accessAction][]</span></span>        | <span data-ttu-id="78494-119">访问了项目。</span><span class="sxs-lookup"><span data-stu-id="78494-119">An item was accessed.</span></span>
| <span data-ttu-id="78494-120">actor</span><span class="sxs-lookup"><span data-stu-id="78494-120">actor</span></span>    | <span data-ttu-id="78494-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="78494-121">[identitySet][]</span></span>         | <span data-ttu-id="78494-122">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="78494-122">Identity of who performed the action.</span></span> <span data-ttu-id="78494-123">只读。</span><span class="sxs-lookup"><span data-stu-id="78494-123">Read-only.</span></span>
| <span data-ttu-id="78494-124">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="78494-124">activityDateTime</span></span>    | <span data-ttu-id="78494-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78494-125">DateTimeOffset</span></span> | <span data-ttu-id="78494-126">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="78494-126">Details about when the activity took place.</span></span> <span data-ttu-id="78494-127">只读。</span><span class="sxs-lookup"><span data-stu-id="78494-127">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="78494-130">关系</span><span class="sxs-lookup"><span data-stu-id="78494-130">Relationships</span></span>

| <span data-ttu-id="78494-131">关系名称</span><span class="sxs-lookup"><span data-stu-id="78494-131">Relationship name</span></span> | <span data-ttu-id="78494-132">类型</span><span class="sxs-lookup"><span data-stu-id="78494-132">Type</span></span>          | <span data-ttu-id="78494-133">说明</span><span class="sxs-lookup"><span data-stu-id="78494-133">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="78494-134">driveItem</span><span class="sxs-lookup"><span data-stu-id="78494-134">driveItem</span></span>         | <span data-ttu-id="78494-135">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="78494-135">[driveItem][]</span></span> | <span data-ttu-id="78494-136">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="78494-136">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="78494-137">listItem</span><span class="sxs-lookup"><span data-stu-id="78494-137">listItem</span></span>          | <span data-ttu-id="78494-138">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="78494-138">[listItem][]</span></span>  | <span data-ttu-id="78494-139">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="78494-139">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="78494-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78494-142">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->
