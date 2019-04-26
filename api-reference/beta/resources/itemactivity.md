---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: bcb68f94574512fd7e952db036a86f242652851d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339852"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="e112b-102">ItemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="e112b-102">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e112b-103">\*\*\*\* ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="e112b-103">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="e112b-104">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="e112b-104">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e112b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e112b-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e112b-106">属性</span><span class="sxs-lookup"><span data-stu-id="e112b-106">Properties</span></span>

| <span data-ttu-id="e112b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e112b-107">Property</span></span> | <span data-ttu-id="e112b-108">类型</span><span class="sxs-lookup"><span data-stu-id="e112b-108">Type</span></span>                    | <span data-ttu-id="e112b-109">说明</span><span class="sxs-lookup"><span data-stu-id="e112b-109">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="e112b-110">id</span><span class="sxs-lookup"><span data-stu-id="e112b-110">id</span></span>       | <span data-ttu-id="e112b-111">string</span><span class="sxs-lookup"><span data-stu-id="e112b-111">string</span></span>                  | <span data-ttu-id="e112b-112">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e112b-112">The unique identifier of the activity.</span></span> <span data-ttu-id="e112b-113">只读。</span><span class="sxs-lookup"><span data-stu-id="e112b-113">Read-only.</span></span>
| <span data-ttu-id="e112b-114">访问</span><span class="sxs-lookup"><span data-stu-id="e112b-114">access</span></span>   | <span data-ttu-id="e112b-115">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-115">[accessAction][]</span></span>        | <span data-ttu-id="e112b-116">访问了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-116">An item was accessed.</span></span>
| <span data-ttu-id="e112b-117">action</span><span class="sxs-lookup"><span data-stu-id="e112b-117">action</span></span>   | <span data-ttu-id="e112b-118">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="e112b-118">[itemActionSet][]</span></span>       | <span data-ttu-id="e112b-119">有关发生的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e112b-119">Details about the action that took place.</span></span> <span data-ttu-id="e112b-120">只读。</span><span class="sxs-lookup"><span data-stu-id="e112b-120">Read-only.</span></span>
| <span data-ttu-id="e112b-121">actor</span><span class="sxs-lookup"><span data-stu-id="e112b-121">actor</span></span>    | <span data-ttu-id="e112b-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e112b-122">[identitySet][]</span></span>         | <span data-ttu-id="e112b-123">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="e112b-123">Identity of who performed the action.</span></span> <span data-ttu-id="e112b-124">只读。</span><span class="sxs-lookup"><span data-stu-id="e112b-124">Read-only.</span></span>
| <span data-ttu-id="e112b-125">location</span><span class="sxs-lookup"><span data-stu-id="e112b-125">location</span></span> | <span data-ttu-id="e112b-126">[位置][]</span><span class="sxs-lookup"><span data-stu-id="e112b-126">[location][]</span></span>            | <span data-ttu-id="e112b-127">执行操作的物理位置。</span><span class="sxs-lookup"><span data-stu-id="e112b-127">Physical location where the action was performed.</span></span> <span data-ttu-id="e112b-128">只读。</span><span class="sxs-lookup"><span data-stu-id="e112b-128">Read-only.</span></span>
| <span data-ttu-id="e112b-129">times</span><span class="sxs-lookup"><span data-stu-id="e112b-129">times</span></span>    | <span data-ttu-id="e112b-130">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="e112b-130">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="e112b-131">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e112b-131">Details about when the activity took place.</span></span> <span data-ttu-id="e112b-132">只读。</span><span class="sxs-lookup"><span data-stu-id="e112b-132">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="e112b-136">关系</span><span class="sxs-lookup"><span data-stu-id="e112b-136">Relationships</span></span>

| <span data-ttu-id="e112b-137">关系名称</span><span class="sxs-lookup"><span data-stu-id="e112b-137">Relationship name</span></span> | <span data-ttu-id="e112b-138">类型</span><span class="sxs-lookup"><span data-stu-id="e112b-138">Type</span></span>          | <span data-ttu-id="e112b-139">说明</span><span class="sxs-lookup"><span data-stu-id="e112b-139">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="e112b-140">driveItem</span><span class="sxs-lookup"><span data-stu-id="e112b-140">driveItem</span></span>         | <span data-ttu-id="e112b-141">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="e112b-141">[driveItem][]</span></span> | <span data-ttu-id="e112b-142">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="e112b-142">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="e112b-143">listItem</span><span class="sxs-lookup"><span data-stu-id="e112b-143">listItem</span></span>          | <span data-ttu-id="e112b-144">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="e112b-144">[listItem][]</span></span>  | <span data-ttu-id="e112b-145">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="e112b-145">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="e112b-148">操作</span><span class="sxs-lookup"><span data-stu-id="e112b-148">Actions</span></span>

<span data-ttu-id="e112b-149">活动内发生的操作在 **action** 属性中有详细说明。</span><span class="sxs-lookup"><span data-stu-id="e112b-149">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="e112b-150">以下是现在可执行的操作。</span><span class="sxs-lookup"><span data-stu-id="e112b-150">Below are the actions that are available today.</span></span>
<span data-ttu-id="e112b-151">未来可能会记录新操作，因此确保应用程序允许在不了解任何操作的情况下便可处理 **itemActivity**。</span><span class="sxs-lookup"><span data-stu-id="e112b-151">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="e112b-152">操作名</span><span class="sxs-lookup"><span data-stu-id="e112b-152">Action name</span></span> | <span data-ttu-id="e112b-153">类型</span><span class="sxs-lookup"><span data-stu-id="e112b-153">Type</span></span>              | <span data-ttu-id="e112b-154">说明</span><span class="sxs-lookup"><span data-stu-id="e112b-154">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="e112b-155">comment</span><span class="sxs-lookup"><span data-stu-id="e112b-155">comment</span></span>     | <span data-ttu-id="e112b-156">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-156">[commentAction][]</span></span> | <span data-ttu-id="e112b-157">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="e112b-157">A comment was added to the item.</span></span>
| <span data-ttu-id="e112b-158">create</span><span class="sxs-lookup"><span data-stu-id="e112b-158">create</span></span>      | <span data-ttu-id="e112b-159">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-159">[createAction][]</span></span>  | <span data-ttu-id="e112b-160">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-160">An item was created.</span></span>
| <span data-ttu-id="e112b-161">delete</span><span class="sxs-lookup"><span data-stu-id="e112b-161">delete</span></span>      | <span data-ttu-id="e112b-162">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-162">[deleteAction][]</span></span>  | <span data-ttu-id="e112b-163">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-163">An item was deleted.</span></span>
| <span data-ttu-id="e112b-164">edit</span><span class="sxs-lookup"><span data-stu-id="e112b-164">edit</span></span>        | <span data-ttu-id="e112b-165">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-165">[editAction][]</span></span>    | <span data-ttu-id="e112b-166">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-166">An item was edited.</span></span>
| <span data-ttu-id="e112b-167">mention</span><span class="sxs-lookup"><span data-stu-id="e112b-167">mention</span></span>     | <span data-ttu-id="e112b-168">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-168">[mentionAction][]</span></span> | <span data-ttu-id="e112b-169">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="e112b-169">A user was mentioned in the item.</span></span>
| <span data-ttu-id="e112b-170">move</span><span class="sxs-lookup"><span data-stu-id="e112b-170">move</span></span>        | <span data-ttu-id="e112b-171">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-171">[moveAction][]</span></span>    | <span data-ttu-id="e112b-172">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-172">An item was moved.</span></span>
| <span data-ttu-id="e112b-173">rename</span><span class="sxs-lookup"><span data-stu-id="e112b-173">rename</span></span>      | <span data-ttu-id="e112b-174">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-174">[renameAction][]</span></span>  | <span data-ttu-id="e112b-175">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-175">An item was renamed.</span></span>
| <span data-ttu-id="e112b-176">restore</span><span class="sxs-lookup"><span data-stu-id="e112b-176">restore</span></span>     | <span data-ttu-id="e112b-177">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-177">[restoreAction][]</span></span> | <span data-ttu-id="e112b-178">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-178">An item was restored.</span></span>
| <span data-ttu-id="e112b-179">share</span><span class="sxs-lookup"><span data-stu-id="e112b-179">share</span></span>       | <span data-ttu-id="e112b-180">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-180">[shareAction][]</span></span>   | <span data-ttu-id="e112b-181">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="e112b-181">An item was shared.</span></span>
| <span data-ttu-id="e112b-182">version</span><span class="sxs-lookup"><span data-stu-id="e112b-182">version</span></span>     | <span data-ttu-id="e112b-183">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="e112b-183">[versionAction][]</span></span> | <span data-ttu-id="e112b-184">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="e112b-184">An item was versioned.</span></span>

[accessAction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="e112b-197">注解</span><span class="sxs-lookup"><span data-stu-id="e112b-197">Remarks</span></span>

<span data-ttu-id="e112b-198">\*\*\*\* ItemActivity 目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="e112b-198">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

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
