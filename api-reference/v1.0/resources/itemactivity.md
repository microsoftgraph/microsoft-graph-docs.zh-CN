---
author: daspek
ms.author: dspektor
title: itemActivity 资源类型
description: ItemActivity 对象提供有关项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4ae71056fccebcb372891124b01999004b1957c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009329"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="f2fb2-103">itemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2fb2-103">itemActivity resource type</span></span>

<span data-ttu-id="f2fb2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2fb2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f2fb2-105">**ItemActivity**资源提供有关在项目或容器中发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-105">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="f2fb2-106">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="f2fb2-107">在 itemActivity 中发生的操作将在 [itemActionSet][] 属性中进行详细说明。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-107">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="f2fb2-108">**注意：** **itemActivity** 目前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-108">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="f2fb2-110">属性</span><span class="sxs-lookup"><span data-stu-id="f2fb2-110">Properties</span></span>

| <span data-ttu-id="f2fb2-111">属性</span><span class="sxs-lookup"><span data-stu-id="f2fb2-111">Property</span></span> | <span data-ttu-id="f2fb2-112">类型</span><span class="sxs-lookup"><span data-stu-id="f2fb2-112">Type</span></span>                    | <span data-ttu-id="f2fb2-113">说明</span><span class="sxs-lookup"><span data-stu-id="f2fb2-113">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="f2fb2-114">id</span><span class="sxs-lookup"><span data-stu-id="f2fb2-114">id</span></span>       | <span data-ttu-id="f2fb2-115">string</span><span class="sxs-lookup"><span data-stu-id="f2fb2-115">string</span></span>                  | <span data-ttu-id="f2fb2-116">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-116">The unique identifier of the activity.</span></span> <span data-ttu-id="f2fb2-117">只读。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-117">Read-only.</span></span>
| <span data-ttu-id="f2fb2-118">访问</span><span class="sxs-lookup"><span data-stu-id="f2fb2-118">access</span></span>   | <span data-ttu-id="f2fb2-119">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="f2fb2-119">[accessAction][]</span></span>        | <span data-ttu-id="f2fb2-120">访问了项目。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-120">An item was accessed.</span></span>
| <span data-ttu-id="f2fb2-121">actor</span><span class="sxs-lookup"><span data-stu-id="f2fb2-121">actor</span></span>    | <span data-ttu-id="f2fb2-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f2fb2-122">[identitySet][]</span></span>         | <span data-ttu-id="f2fb2-123">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-123">Identity of who performed the action.</span></span> <span data-ttu-id="f2fb2-124">只读。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-124">Read-only.</span></span>
| <span data-ttu-id="f2fb2-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="f2fb2-125">activityDateTime</span></span>    | <span data-ttu-id="f2fb2-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2fb2-126">DateTimeOffset</span></span> | <span data-ttu-id="f2fb2-127">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-127">Details about when the activity took place.</span></span> <span data-ttu-id="f2fb2-128">只读。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-128">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="f2fb2-131">关系</span><span class="sxs-lookup"><span data-stu-id="f2fb2-131">Relationships</span></span>

| <span data-ttu-id="f2fb2-132">关系名称</span><span class="sxs-lookup"><span data-stu-id="f2fb2-132">Relationship name</span></span> | <span data-ttu-id="f2fb2-133">类型</span><span class="sxs-lookup"><span data-stu-id="f2fb2-133">Type</span></span>          | <span data-ttu-id="f2fb2-134">说明</span><span class="sxs-lookup"><span data-stu-id="f2fb2-134">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="f2fb2-135">driveItem</span><span class="sxs-lookup"><span data-stu-id="f2fb2-135">driveItem</span></span>         | <span data-ttu-id="f2fb2-136">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="f2fb2-136">[driveItem][]</span></span> | <span data-ttu-id="f2fb2-137">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-137">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="f2fb2-138">listItem</span><span class="sxs-lookup"><span data-stu-id="f2fb2-138">listItem</span></span>          | <span data-ttu-id="f2fb2-139">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="f2fb2-139">[listItem][]</span></span>  | <span data-ttu-id="f2fb2-140">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="f2fb2-140">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="f2fb2-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2fb2-143">JSON representation</span></span>

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

