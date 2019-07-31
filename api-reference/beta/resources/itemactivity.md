---
author: daspek
description: ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab96c3169a2d2dc37e6b94ab325866e93fa4d6c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967092"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="2b0e1-103">ItemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b0e1-103">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b0e1-104">\*\*\*\* ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-104">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="2b0e1-105">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-105">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b0e1-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b0e1-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2b0e1-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b0e1-107">Properties</span></span>

| <span data-ttu-id="2b0e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b0e1-108">Property</span></span> | <span data-ttu-id="2b0e1-109">类型</span><span class="sxs-lookup"><span data-stu-id="2b0e1-109">Type</span></span>                    | <span data-ttu-id="2b0e1-110">说明</span><span class="sxs-lookup"><span data-stu-id="2b0e1-110">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="2b0e1-111">id</span><span class="sxs-lookup"><span data-stu-id="2b0e1-111">id</span></span>       | <span data-ttu-id="2b0e1-112">string</span><span class="sxs-lookup"><span data-stu-id="2b0e1-112">string</span></span>                  | <span data-ttu-id="2b0e1-113">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-113">The unique identifier of the activity.</span></span> <span data-ttu-id="2b0e1-114">只读。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-114">Read-only.</span></span>
| <span data-ttu-id="2b0e1-115">访问</span><span class="sxs-lookup"><span data-stu-id="2b0e1-115">access</span></span>   | <span data-ttu-id="2b0e1-116">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-116">[accessAction][]</span></span>        | <span data-ttu-id="2b0e1-117">访问了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-117">An item was accessed.</span></span>
| <span data-ttu-id="2b0e1-118">action</span><span class="sxs-lookup"><span data-stu-id="2b0e1-118">action</span></span>   | <span data-ttu-id="2b0e1-119">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-119">[itemActionSet][]</span></span>       | <span data-ttu-id="2b0e1-120">有关发生的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-120">Details about the action that took place.</span></span> <span data-ttu-id="2b0e1-121">只读。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-121">Read-only.</span></span>
| <span data-ttu-id="2b0e1-122">actor</span><span class="sxs-lookup"><span data-stu-id="2b0e1-122">actor</span></span>    | <span data-ttu-id="2b0e1-123">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-123">[identitySet][]</span></span>         | <span data-ttu-id="2b0e1-124">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-124">Identity of who performed the action.</span></span> <span data-ttu-id="2b0e1-125">只读。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-125">Read-only.</span></span>
| <span data-ttu-id="2b0e1-126">location</span><span class="sxs-lookup"><span data-stu-id="2b0e1-126">location</span></span> | <span data-ttu-id="2b0e1-127">[位置][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-127">[location][]</span></span>            | <span data-ttu-id="2b0e1-128">执行操作的物理位置。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-128">Physical location where the action was performed.</span></span> <span data-ttu-id="2b0e1-129">只读。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-129">Read-only.</span></span>
| <span data-ttu-id="2b0e1-130">times</span><span class="sxs-lookup"><span data-stu-id="2b0e1-130">times</span></span>    | <span data-ttu-id="2b0e1-131">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-131">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="2b0e1-132">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-132">Details about when the activity took place.</span></span> <span data-ttu-id="2b0e1-133">只读。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-133">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="2b0e1-137">关系</span><span class="sxs-lookup"><span data-stu-id="2b0e1-137">Relationships</span></span>

| <span data-ttu-id="2b0e1-138">关系名称</span><span class="sxs-lookup"><span data-stu-id="2b0e1-138">Relationship name</span></span> | <span data-ttu-id="2b0e1-139">类型</span><span class="sxs-lookup"><span data-stu-id="2b0e1-139">Type</span></span>          | <span data-ttu-id="2b0e1-140">说明</span><span class="sxs-lookup"><span data-stu-id="2b0e1-140">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="2b0e1-141">driveItem</span><span class="sxs-lookup"><span data-stu-id="2b0e1-141">driveItem</span></span>         | <span data-ttu-id="2b0e1-142">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-142">[driveItem][]</span></span> | <span data-ttu-id="2b0e1-143">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-143">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="2b0e1-144">listItem</span><span class="sxs-lookup"><span data-stu-id="2b0e1-144">listItem</span></span>          | <span data-ttu-id="2b0e1-145">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-145">[listItem][]</span></span>  | <span data-ttu-id="2b0e1-146">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-146">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="2b0e1-149">操作</span><span class="sxs-lookup"><span data-stu-id="2b0e1-149">Actions</span></span>

<span data-ttu-id="2b0e1-150">活动内发生的操作在 **action** 属性中有详细说明。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-150">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="2b0e1-151">以下是现在可执行的操作。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-151">Below are the actions that are available today.</span></span>
<span data-ttu-id="2b0e1-152">未来可能会记录新操作，因此确保应用程序允许在不了解任何操作的情况下便可处理 **itemActivity**。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-152">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="2b0e1-153">操作名</span><span class="sxs-lookup"><span data-stu-id="2b0e1-153">Action name</span></span> | <span data-ttu-id="2b0e1-154">类型</span><span class="sxs-lookup"><span data-stu-id="2b0e1-154">Type</span></span>              | <span data-ttu-id="2b0e1-155">说明</span><span class="sxs-lookup"><span data-stu-id="2b0e1-155">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="2b0e1-156">comment</span><span class="sxs-lookup"><span data-stu-id="2b0e1-156">comment</span></span>     | <span data-ttu-id="2b0e1-157">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-157">[commentAction][]</span></span> | <span data-ttu-id="2b0e1-158">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-158">A comment was added to the item.</span></span>
| <span data-ttu-id="2b0e1-159">create</span><span class="sxs-lookup"><span data-stu-id="2b0e1-159">create</span></span>      | <span data-ttu-id="2b0e1-160">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-160">[createAction][]</span></span>  | <span data-ttu-id="2b0e1-161">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-161">An item was created.</span></span>
| <span data-ttu-id="2b0e1-162">delete</span><span class="sxs-lookup"><span data-stu-id="2b0e1-162">delete</span></span>      | <span data-ttu-id="2b0e1-163">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-163">[deleteAction][]</span></span>  | <span data-ttu-id="2b0e1-164">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-164">An item was deleted.</span></span>
| <span data-ttu-id="2b0e1-165">edit</span><span class="sxs-lookup"><span data-stu-id="2b0e1-165">edit</span></span>        | <span data-ttu-id="2b0e1-166">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-166">[editAction][]</span></span>    | <span data-ttu-id="2b0e1-167">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-167">An item was edited.</span></span>
| <span data-ttu-id="2b0e1-168">mention</span><span class="sxs-lookup"><span data-stu-id="2b0e1-168">mention</span></span>     | <span data-ttu-id="2b0e1-169">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-169">[mentionAction][]</span></span> | <span data-ttu-id="2b0e1-170">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-170">A user was mentioned in the item.</span></span>
| <span data-ttu-id="2b0e1-171">move</span><span class="sxs-lookup"><span data-stu-id="2b0e1-171">move</span></span>        | <span data-ttu-id="2b0e1-172">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-172">[moveAction][]</span></span>    | <span data-ttu-id="2b0e1-173">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-173">An item was moved.</span></span>
| <span data-ttu-id="2b0e1-174">rename</span><span class="sxs-lookup"><span data-stu-id="2b0e1-174">rename</span></span>      | <span data-ttu-id="2b0e1-175">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-175">[renameAction][]</span></span>  | <span data-ttu-id="2b0e1-176">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-176">An item was renamed.</span></span>
| <span data-ttu-id="2b0e1-177">restore</span><span class="sxs-lookup"><span data-stu-id="2b0e1-177">restore</span></span>     | <span data-ttu-id="2b0e1-178">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-178">[restoreAction][]</span></span> | <span data-ttu-id="2b0e1-179">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-179">An item was restored.</span></span>
| <span data-ttu-id="2b0e1-180">share</span><span class="sxs-lookup"><span data-stu-id="2b0e1-180">share</span></span>       | <span data-ttu-id="2b0e1-181">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-181">[shareAction][]</span></span>   | <span data-ttu-id="2b0e1-182">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-182">An item was shared.</span></span>
| <span data-ttu-id="2b0e1-183">version</span><span class="sxs-lookup"><span data-stu-id="2b0e1-183">version</span></span>     | <span data-ttu-id="2b0e1-184">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="2b0e1-184">[versionAction][]</span></span> | <span data-ttu-id="2b0e1-185">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-185">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="2b0e1-198">注解</span><span class="sxs-lookup"><span data-stu-id="2b0e1-198">Remarks</span></span>

<span data-ttu-id="2b0e1-199">\*\*\*\* ItemActivity 目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="2b0e1-199">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

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
