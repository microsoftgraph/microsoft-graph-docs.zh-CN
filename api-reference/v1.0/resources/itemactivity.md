---
author: daspek
title: itemActivity 资源类型
description: itemActivity 对象提供有关在项目上发生的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ef213dd50e5a6be8a96880ccd1a64f15f183f54b
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238685"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="d8839-103">itemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8839-103">itemActivity resource type</span></span>

<span data-ttu-id="d8839-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8839-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8839-105">**itemActivity** 资源提供有关在项目上或容器中发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="d8839-105">The **itemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="d8839-106">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="d8839-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

<span data-ttu-id="d8839-107">itemActionSet 属性中详细说明 [了 itemActivity 中][] 发生的操作。</span><span class="sxs-lookup"><span data-stu-id="d8839-107">The actions that took place within an itemActivity are detailed in the [itemActionSet][] property.</span></span>

><span data-ttu-id="d8839-108">**注意\*\*\*\*：itemActivity** 当前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="d8839-108">**Note:** **itemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a><span data-ttu-id="d8839-110">属性</span><span class="sxs-lookup"><span data-stu-id="d8839-110">Properties</span></span>

| <span data-ttu-id="d8839-111">属性</span><span class="sxs-lookup"><span data-stu-id="d8839-111">Property</span></span> | <span data-ttu-id="d8839-112">类型</span><span class="sxs-lookup"><span data-stu-id="d8839-112">Type</span></span>                    | <span data-ttu-id="d8839-113">说明</span><span class="sxs-lookup"><span data-stu-id="d8839-113">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="d8839-114">id</span><span class="sxs-lookup"><span data-stu-id="d8839-114">id</span></span>       | <span data-ttu-id="d8839-115">string</span><span class="sxs-lookup"><span data-stu-id="d8839-115">string</span></span>                  | <span data-ttu-id="d8839-116">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d8839-116">The unique identifier of the activity.</span></span> <span data-ttu-id="d8839-117">只读。</span><span class="sxs-lookup"><span data-stu-id="d8839-117">Read-only.</span></span>
| <span data-ttu-id="d8839-118">access</span><span class="sxs-lookup"><span data-stu-id="d8839-118">access</span></span>   | <span data-ttu-id="d8839-119">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="d8839-119">[accessAction][]</span></span>        | <span data-ttu-id="d8839-120">已访问项目。</span><span class="sxs-lookup"><span data-stu-id="d8839-120">An item was accessed.</span></span>
| <span data-ttu-id="d8839-121">actor</span><span class="sxs-lookup"><span data-stu-id="d8839-121">actor</span></span>    | <span data-ttu-id="d8839-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d8839-122">[identitySet][]</span></span>         | <span data-ttu-id="d8839-123">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="d8839-123">Identity of who performed the action.</span></span> <span data-ttu-id="d8839-124">只读。</span><span class="sxs-lookup"><span data-stu-id="d8839-124">Read-only.</span></span>
| <span data-ttu-id="d8839-125">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d8839-125">activityDateTime</span></span>    | <span data-ttu-id="d8839-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8839-126">DateTimeOffset</span></span> | <span data-ttu-id="d8839-127">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d8839-127">Details about when the activity took place.</span></span> <span data-ttu-id="d8839-128">只读。</span><span class="sxs-lookup"><span data-stu-id="d8839-128">Read-only.</span></span>

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a><span data-ttu-id="d8839-131">关系</span><span class="sxs-lookup"><span data-stu-id="d8839-131">Relationships</span></span>

| <span data-ttu-id="d8839-132">关系名称</span><span class="sxs-lookup"><span data-stu-id="d8839-132">Relationship name</span></span> | <span data-ttu-id="d8839-133">类型</span><span class="sxs-lookup"><span data-stu-id="d8839-133">Type</span></span>          | <span data-ttu-id="d8839-134">说明</span><span class="sxs-lookup"><span data-stu-id="d8839-134">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="d8839-135">driveItem</span><span class="sxs-lookup"><span data-stu-id="d8839-135">driveItem</span></span>         | <span data-ttu-id="d8839-136">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="d8839-136">[driveItem][]</span></span> | <span data-ttu-id="d8839-137">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="d8839-137">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="d8839-138">listItem</span><span class="sxs-lookup"><span data-stu-id="d8839-138">listItem</span></span>          | <span data-ttu-id="d8839-139">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="d8839-139">[listItem][]</span></span>  | <span data-ttu-id="d8839-140">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="d8839-140">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="d8839-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8839-143">JSON representation</span></span>

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

