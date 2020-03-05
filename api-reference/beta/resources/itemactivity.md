---
author: daspek
description: ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4cac403e44abaf9ae69f78005555772b9979046f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523119"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="89498-103">ItemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="89498-103">ItemActivity resource type</span></span>

<span data-ttu-id="89498-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="89498-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89498-105">\*\*\*\* ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="89498-105">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="89498-106">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="89498-106">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89498-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89498-107">JSON representation</span></span>

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
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a><span data-ttu-id="89498-108">属性</span><span class="sxs-lookup"><span data-stu-id="89498-108">Properties</span></span>

| <span data-ttu-id="89498-109">属性</span><span class="sxs-lookup"><span data-stu-id="89498-109">Property</span></span> | <span data-ttu-id="89498-110">类型</span><span class="sxs-lookup"><span data-stu-id="89498-110">Type</span></span>                    | <span data-ttu-id="89498-111">说明</span><span class="sxs-lookup"><span data-stu-id="89498-111">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="89498-112">id</span><span class="sxs-lookup"><span data-stu-id="89498-112">id</span></span>       | <span data-ttu-id="89498-113">string</span><span class="sxs-lookup"><span data-stu-id="89498-113">string</span></span>                  | <span data-ttu-id="89498-114">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="89498-114">The unique identifier of the activity.</span></span> <span data-ttu-id="89498-115">只读。</span><span class="sxs-lookup"><span data-stu-id="89498-115">Read-only.</span></span>
| <span data-ttu-id="89498-116">访问</span><span class="sxs-lookup"><span data-stu-id="89498-116">access</span></span>   | <span data-ttu-id="89498-117">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-117">[accessAction][]</span></span>        | <span data-ttu-id="89498-118">访问了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-118">An item was accessed.</span></span>
| <span data-ttu-id="89498-119">action</span><span class="sxs-lookup"><span data-stu-id="89498-119">action</span></span>   | <span data-ttu-id="89498-120">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="89498-120">[itemActionSet][]</span></span>       | <span data-ttu-id="89498-121">有关发生的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="89498-121">Details about the action that took place.</span></span> <span data-ttu-id="89498-122">只读。</span><span class="sxs-lookup"><span data-stu-id="89498-122">Read-only.</span></span>
| <span data-ttu-id="89498-123">actor</span><span class="sxs-lookup"><span data-stu-id="89498-123">actor</span></span>    | <span data-ttu-id="89498-124">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="89498-124">[identitySet][]</span></span>         | <span data-ttu-id="89498-125">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="89498-125">Identity of who performed the action.</span></span> <span data-ttu-id="89498-126">只读。</span><span class="sxs-lookup"><span data-stu-id="89498-126">Read-only.</span></span>
| <span data-ttu-id="89498-127">location</span><span class="sxs-lookup"><span data-stu-id="89498-127">location</span></span> | <span data-ttu-id="89498-128">[位置][]</span><span class="sxs-lookup"><span data-stu-id="89498-128">[location][]</span></span>            | <span data-ttu-id="89498-129">执行操作的物理位置。</span><span class="sxs-lookup"><span data-stu-id="89498-129">Physical location where the action was performed.</span></span> <span data-ttu-id="89498-130">只读。</span><span class="sxs-lookup"><span data-stu-id="89498-130">Read-only.</span></span>
| <span data-ttu-id="89498-131">times</span><span class="sxs-lookup"><span data-stu-id="89498-131">times</span></span>    | <span data-ttu-id="89498-132">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="89498-132">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="89498-133">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="89498-133">Details about when the activity took place.</span></span> <span data-ttu-id="89498-134">只读。</span><span class="sxs-lookup"><span data-stu-id="89498-134">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="89498-138">关系</span><span class="sxs-lookup"><span data-stu-id="89498-138">Relationships</span></span>

| <span data-ttu-id="89498-139">关系名称</span><span class="sxs-lookup"><span data-stu-id="89498-139">Relationship name</span></span> | <span data-ttu-id="89498-140">类型</span><span class="sxs-lookup"><span data-stu-id="89498-140">Type</span></span>          | <span data-ttu-id="89498-141">说明</span><span class="sxs-lookup"><span data-stu-id="89498-141">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="89498-142">driveItem</span><span class="sxs-lookup"><span data-stu-id="89498-142">driveItem</span></span>         | <span data-ttu-id="89498-143">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="89498-143">[driveItem][]</span></span> | <span data-ttu-id="89498-144">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="89498-144">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="89498-145">listItem</span><span class="sxs-lookup"><span data-stu-id="89498-145">listItem</span></span>          | <span data-ttu-id="89498-146">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="89498-146">[listItem][]</span></span>  | <span data-ttu-id="89498-147">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="89498-147">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="89498-150">操作</span><span class="sxs-lookup"><span data-stu-id="89498-150">Actions</span></span>

<span data-ttu-id="89498-151">活动内发生的操作在 **action** 属性中有详细说明。</span><span class="sxs-lookup"><span data-stu-id="89498-151">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="89498-152">以下是现在可执行的操作。</span><span class="sxs-lookup"><span data-stu-id="89498-152">Below are the actions that are available today.</span></span>
<span data-ttu-id="89498-153">未来可能会记录新操作，因此确保应用程序允许在不了解任何操作的情况下便可处理 **itemActivity**。</span><span class="sxs-lookup"><span data-stu-id="89498-153">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="89498-154">操作名</span><span class="sxs-lookup"><span data-stu-id="89498-154">Action name</span></span> | <span data-ttu-id="89498-155">类型</span><span class="sxs-lookup"><span data-stu-id="89498-155">Type</span></span>              | <span data-ttu-id="89498-156">说明</span><span class="sxs-lookup"><span data-stu-id="89498-156">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="89498-157">comment</span><span class="sxs-lookup"><span data-stu-id="89498-157">comment</span></span>     | <span data-ttu-id="89498-158">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-158">[commentAction][]</span></span> | <span data-ttu-id="89498-159">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="89498-159">A comment was added to the item.</span></span>
| <span data-ttu-id="89498-160">create</span><span class="sxs-lookup"><span data-stu-id="89498-160">create</span></span>      | <span data-ttu-id="89498-161">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-161">[createAction][]</span></span>  | <span data-ttu-id="89498-162">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-162">An item was created.</span></span>
| <span data-ttu-id="89498-163">delete</span><span class="sxs-lookup"><span data-stu-id="89498-163">delete</span></span>      | <span data-ttu-id="89498-164">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-164">[deleteAction][]</span></span>  | <span data-ttu-id="89498-165">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-165">An item was deleted.</span></span>
| <span data-ttu-id="89498-166">edit</span><span class="sxs-lookup"><span data-stu-id="89498-166">edit</span></span>        | <span data-ttu-id="89498-167">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-167">[editAction][]</span></span>    | <span data-ttu-id="89498-168">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-168">An item was edited.</span></span>
| <span data-ttu-id="89498-169">mention</span><span class="sxs-lookup"><span data-stu-id="89498-169">mention</span></span>     | <span data-ttu-id="89498-170">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-170">[mentionAction][]</span></span> | <span data-ttu-id="89498-171">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="89498-171">A user was mentioned in the item.</span></span>
| <span data-ttu-id="89498-172">move</span><span class="sxs-lookup"><span data-stu-id="89498-172">move</span></span>        | <span data-ttu-id="89498-173">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-173">[moveAction][]</span></span>    | <span data-ttu-id="89498-174">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-174">An item was moved.</span></span>
| <span data-ttu-id="89498-175">rename</span><span class="sxs-lookup"><span data-stu-id="89498-175">rename</span></span>      | <span data-ttu-id="89498-176">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-176">[renameAction][]</span></span>  | <span data-ttu-id="89498-177">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-177">An item was renamed.</span></span>
| <span data-ttu-id="89498-178">restore</span><span class="sxs-lookup"><span data-stu-id="89498-178">restore</span></span>     | <span data-ttu-id="89498-179">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-179">[restoreAction][]</span></span> | <span data-ttu-id="89498-180">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-180">An item was restored.</span></span>
| <span data-ttu-id="89498-181">share</span><span class="sxs-lookup"><span data-stu-id="89498-181">share</span></span>       | <span data-ttu-id="89498-182">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-182">[shareAction][]</span></span>   | <span data-ttu-id="89498-183">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="89498-183">An item was shared.</span></span>
| <span data-ttu-id="89498-184">version</span><span class="sxs-lookup"><span data-stu-id="89498-184">version</span></span>     | <span data-ttu-id="89498-185">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="89498-185">[versionAction][]</span></span> | <span data-ttu-id="89498-186">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="89498-186">An item was versioned.</span></span>

[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[位置]: location.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="89498-199">注解</span><span class="sxs-lookup"><span data-stu-id="89498-199">Remarks</span></span>

<span data-ttu-id="89498-200">\*\*\*\* ItemActivity 目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="89498-200">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": []
}
-->
