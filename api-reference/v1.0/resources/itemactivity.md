---
author: daspek
ms.author: dspektor
title: itemActivity 资源类型
description: ItemActivity 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f1ffbcc84f3cb399b131ae40c46cae9230e4cac8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447673"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="45fae-103">itemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="45fae-103">itemActivity resource type</span></span>

<span data-ttu-id="45fae-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="45fae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45fae-105">**ItemActivity**资源提供有关在项目或容器中发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="45fae-105">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="45fae-106">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="45fae-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="45fae-107">在 itemActivity 中发生的操作将在[itemActionSet][]属性中进行详细说明。</span><span class="sxs-lookup"><span data-stu-id="45fae-107">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="45fae-108">**注意：** **itemActivity**目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="45fae-108">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="45fae-110">属性</span><span class="sxs-lookup"><span data-stu-id="45fae-110">Properties</span></span>

| <span data-ttu-id="45fae-111">属性</span><span class="sxs-lookup"><span data-stu-id="45fae-111">Property</span></span> | <span data-ttu-id="45fae-112">类型</span><span class="sxs-lookup"><span data-stu-id="45fae-112">Type</span></span>                    | <span data-ttu-id="45fae-113">说明</span><span class="sxs-lookup"><span data-stu-id="45fae-113">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="45fae-114">id</span><span class="sxs-lookup"><span data-stu-id="45fae-114">id</span></span>       | <span data-ttu-id="45fae-115">string</span><span class="sxs-lookup"><span data-stu-id="45fae-115">string</span></span>                  | <span data-ttu-id="45fae-116">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="45fae-116">The unique identifier of the activity.</span></span> <span data-ttu-id="45fae-117">只读。</span><span class="sxs-lookup"><span data-stu-id="45fae-117">Read-only.</span></span>
| <span data-ttu-id="45fae-118">访问</span><span class="sxs-lookup"><span data-stu-id="45fae-118">access</span></span>   | <span data-ttu-id="45fae-119">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="45fae-119">[accessAction][]</span></span>        | <span data-ttu-id="45fae-120">访问了项目。</span><span class="sxs-lookup"><span data-stu-id="45fae-120">An item was accessed.</span></span>
| <span data-ttu-id="45fae-121">actor</span><span class="sxs-lookup"><span data-stu-id="45fae-121">actor</span></span>    | <span data-ttu-id="45fae-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="45fae-122">[identitySet][]</span></span>         | <span data-ttu-id="45fae-123">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="45fae-123">Identity of who performed the action.</span></span> <span data-ttu-id="45fae-124">只读。</span><span class="sxs-lookup"><span data-stu-id="45fae-124">Read-only.</span></span>
| <span data-ttu-id="45fae-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="45fae-125">activityDateTime</span></span>    | <span data-ttu-id="45fae-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45fae-126">DateTimeOffset</span></span> | <span data-ttu-id="45fae-127">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="45fae-127">Details about when the activity took place.</span></span> <span data-ttu-id="45fae-128">只读。</span><span class="sxs-lookup"><span data-stu-id="45fae-128">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="45fae-131">关系</span><span class="sxs-lookup"><span data-stu-id="45fae-131">Relationships</span></span>

| <span data-ttu-id="45fae-132">关系名称</span><span class="sxs-lookup"><span data-stu-id="45fae-132">Relationship name</span></span> | <span data-ttu-id="45fae-133">类型</span><span class="sxs-lookup"><span data-stu-id="45fae-133">Type</span></span>          | <span data-ttu-id="45fae-134">说明</span><span class="sxs-lookup"><span data-stu-id="45fae-134">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="45fae-135">driveItem</span><span class="sxs-lookup"><span data-stu-id="45fae-135">driveItem</span></span>         | <span data-ttu-id="45fae-136">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="45fae-136">[driveItem][]</span></span> | <span data-ttu-id="45fae-137">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="45fae-137">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="45fae-138">listItem</span><span class="sxs-lookup"><span data-stu-id="45fae-138">listItem</span></span>          | <span data-ttu-id="45fae-139">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="45fae-139">[listItem][]</span></span>  | <span data-ttu-id="45fae-140">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="45fae-140">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="45fae-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45fae-143">JSON representation</span></span>

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
