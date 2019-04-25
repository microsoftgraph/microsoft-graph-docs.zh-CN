---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: 5e2be549c3e3e9e799449679b605577ecd782a94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561885"
---
# <a name="itemactivity-resource-type"></a><span data-ttu-id="6d03d-102">ItemActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d03d-102">ItemActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d03d-103">\*\*\*\* ItemActivity 资源提供有关在项目上或容器内发生的活动的信息。</span><span class="sxs-lookup"><span data-stu-id="6d03d-103">The **ItemActivity** resource provides information about activities that took place on an item or within a container.</span></span>
<span data-ttu-id="6d03d-104">目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="6d03d-104">Currently only available on SharePoint and OneDrive for Business.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d03d-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d03d-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6d03d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6d03d-106">Properties</span></span>

| <span data-ttu-id="6d03d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d03d-107">Property</span></span> | <span data-ttu-id="6d03d-108">类型</span><span class="sxs-lookup"><span data-stu-id="6d03d-108">Type</span></span>                    | <span data-ttu-id="6d03d-109">说明</span><span class="sxs-lookup"><span data-stu-id="6d03d-109">Description</span></span>
|:---------|:------------------------|:----------------------------------------
| <span data-ttu-id="6d03d-110">id</span><span class="sxs-lookup"><span data-stu-id="6d03d-110">id</span></span>       | <span data-ttu-id="6d03d-111">string</span><span class="sxs-lookup"><span data-stu-id="6d03d-111">string</span></span>                  | <span data-ttu-id="6d03d-112">活动的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6d03d-112">The unique identifier of the activity.</span></span> <span data-ttu-id="6d03d-113">只读。</span><span class="sxs-lookup"><span data-stu-id="6d03d-113">Read-only.</span></span>
| <span data-ttu-id="6d03d-114">访问</span><span class="sxs-lookup"><span data-stu-id="6d03d-114">access</span></span>   | <span data-ttu-id="6d03d-115">[accessAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-115">[accessAction][]</span></span>        | <span data-ttu-id="6d03d-116">访问了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-116">An item was accessed.</span></span>
| <span data-ttu-id="6d03d-117">action</span><span class="sxs-lookup"><span data-stu-id="6d03d-117">action</span></span>   | <span data-ttu-id="6d03d-118">[itemActionSet][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-118">[itemActionSet][]</span></span>       | <span data-ttu-id="6d03d-119">有关发生的操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6d03d-119">Details about the action that took place.</span></span> <span data-ttu-id="6d03d-120">只读。</span><span class="sxs-lookup"><span data-stu-id="6d03d-120">Read-only.</span></span>
| <span data-ttu-id="6d03d-121">actor</span><span class="sxs-lookup"><span data-stu-id="6d03d-121">actor</span></span>    | <span data-ttu-id="6d03d-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-122">[identitySet][]</span></span>         | <span data-ttu-id="6d03d-123">操作执行者的身份。</span><span class="sxs-lookup"><span data-stu-id="6d03d-123">Identity of who performed the action.</span></span> <span data-ttu-id="6d03d-124">只读。</span><span class="sxs-lookup"><span data-stu-id="6d03d-124">Read-only.</span></span>
| <span data-ttu-id="6d03d-125">location</span><span class="sxs-lookup"><span data-stu-id="6d03d-125">location</span></span> | <span data-ttu-id="6d03d-126">[位置][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-126">[location][]</span></span>            | <span data-ttu-id="6d03d-127">执行操作的物理位置。</span><span class="sxs-lookup"><span data-stu-id="6d03d-127">Physical location where the action was performed.</span></span> <span data-ttu-id="6d03d-128">只读。</span><span class="sxs-lookup"><span data-stu-id="6d03d-128">Read-only.</span></span>
| <span data-ttu-id="6d03d-129">times</span><span class="sxs-lookup"><span data-stu-id="6d03d-129">times</span></span>    | <span data-ttu-id="6d03d-130">[itemActivityTimeSet][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-130">[itemActivityTimeSet][]</span></span> | <span data-ttu-id="6d03d-131">有关活动何时发生的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6d03d-131">Details about when the activity took place.</span></span> <span data-ttu-id="6d03d-132">只读。</span><span class="sxs-lookup"><span data-stu-id="6d03d-132">Read-only.</span></span>

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a><span data-ttu-id="6d03d-136">关系</span><span class="sxs-lookup"><span data-stu-id="6d03d-136">Relationships</span></span>

| <span data-ttu-id="6d03d-137">关系名称</span><span class="sxs-lookup"><span data-stu-id="6d03d-137">Relationship name</span></span> | <span data-ttu-id="6d03d-138">类型</span><span class="sxs-lookup"><span data-stu-id="6d03d-138">Type</span></span>          | <span data-ttu-id="6d03d-139">说明</span><span class="sxs-lookup"><span data-stu-id="6d03d-139">Description</span></span>
|:------------------|:--------------|:-----------------------------------------
| <span data-ttu-id="6d03d-140">driveItem</span><span class="sxs-lookup"><span data-stu-id="6d03d-140">driveItem</span></span>         | <span data-ttu-id="6d03d-141">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-141">[driveItem][]</span></span> | <span data-ttu-id="6d03d-142">公开作为此活动目标的 **driveItem**。</span><span class="sxs-lookup"><span data-stu-id="6d03d-142">Exposes the **driveItem** that was the target of this activity.</span></span>
| <span data-ttu-id="6d03d-143">listItem</span><span class="sxs-lookup"><span data-stu-id="6d03d-143">listItem</span></span>          | <span data-ttu-id="6d03d-144">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-144">[listItem][]</span></span>  | <span data-ttu-id="6d03d-145">公开作为此活动目标的 **listItem**。</span><span class="sxs-lookup"><span data-stu-id="6d03d-145">Exposes the **listItem** that was the target of this activity.</span></span>

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a><span data-ttu-id="6d03d-148">操作</span><span class="sxs-lookup"><span data-stu-id="6d03d-148">Actions</span></span>

<span data-ttu-id="6d03d-149">活动内发生的操作在 **action** 属性中有详细说明。</span><span class="sxs-lookup"><span data-stu-id="6d03d-149">The actions that took place within an activity are detailed in the **action** property.</span></span>
<span data-ttu-id="6d03d-150">以下是现在可执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6d03d-150">Below are the actions that are available today.</span></span>
<span data-ttu-id="6d03d-151">未来可能会记录新操作，因此确保应用程序允许在不了解任何操作的情况下便可处理 **itemActivity**。</span><span class="sxs-lookup"><span data-stu-id="6d03d-151">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActivity** without any actions that your app understands.</span></span>

| <span data-ttu-id="6d03d-152">操作名</span><span class="sxs-lookup"><span data-stu-id="6d03d-152">Action name</span></span> | <span data-ttu-id="6d03d-153">类型</span><span class="sxs-lookup"><span data-stu-id="6d03d-153">Type</span></span>              | <span data-ttu-id="6d03d-154">说明</span><span class="sxs-lookup"><span data-stu-id="6d03d-154">Description</span></span>
|:------------|:------------------|:-------------------------------------------
| <span data-ttu-id="6d03d-155">comment</span><span class="sxs-lookup"><span data-stu-id="6d03d-155">comment</span></span>     | <span data-ttu-id="6d03d-156">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-156">[commentAction][]</span></span> | <span data-ttu-id="6d03d-157">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="6d03d-157">A comment was added to the item.</span></span>
| <span data-ttu-id="6d03d-158">create</span><span class="sxs-lookup"><span data-stu-id="6d03d-158">create</span></span>      | <span data-ttu-id="6d03d-159">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-159">[createAction][]</span></span>  | <span data-ttu-id="6d03d-160">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-160">An item was created.</span></span>
| <span data-ttu-id="6d03d-161">delete</span><span class="sxs-lookup"><span data-stu-id="6d03d-161">delete</span></span>      | <span data-ttu-id="6d03d-162">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-162">[deleteAction][]</span></span>  | <span data-ttu-id="6d03d-163">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-163">An item was deleted.</span></span>
| <span data-ttu-id="6d03d-164">edit</span><span class="sxs-lookup"><span data-stu-id="6d03d-164">edit</span></span>        | <span data-ttu-id="6d03d-165">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-165">[editAction][]</span></span>    | <span data-ttu-id="6d03d-166">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-166">An item was edited.</span></span>
| <span data-ttu-id="6d03d-167">mention</span><span class="sxs-lookup"><span data-stu-id="6d03d-167">mention</span></span>     | <span data-ttu-id="6d03d-168">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-168">[mentionAction][]</span></span> | <span data-ttu-id="6d03d-169">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="6d03d-169">A user was mentioned in the item.</span></span>
| <span data-ttu-id="6d03d-170">move</span><span class="sxs-lookup"><span data-stu-id="6d03d-170">move</span></span>        | <span data-ttu-id="6d03d-171">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-171">[moveAction][]</span></span>    | <span data-ttu-id="6d03d-172">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-172">An item was moved.</span></span>
| <span data-ttu-id="6d03d-173">rename</span><span class="sxs-lookup"><span data-stu-id="6d03d-173">rename</span></span>      | <span data-ttu-id="6d03d-174">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-174">[renameAction][]</span></span>  | <span data-ttu-id="6d03d-175">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-175">An item was renamed.</span></span>
| <span data-ttu-id="6d03d-176">restore</span><span class="sxs-lookup"><span data-stu-id="6d03d-176">restore</span></span>     | <span data-ttu-id="6d03d-177">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-177">[restoreAction][]</span></span> | <span data-ttu-id="6d03d-178">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-178">An item was restored.</span></span>
| <span data-ttu-id="6d03d-179">share</span><span class="sxs-lookup"><span data-stu-id="6d03d-179">share</span></span>       | <span data-ttu-id="6d03d-180">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-180">[shareAction][]</span></span>   | <span data-ttu-id="6d03d-181">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="6d03d-181">An item was shared.</span></span>
| <span data-ttu-id="6d03d-182">version</span><span class="sxs-lookup"><span data-stu-id="6d03d-182">version</span></span>     | <span data-ttu-id="6d03d-183">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="6d03d-183">[versionAction][]</span></span> | <span data-ttu-id="6d03d-184">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="6d03d-184">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="6d03d-197">注解</span><span class="sxs-lookup"><span data-stu-id="6d03d-197">Remarks</span></span>

<span data-ttu-id="6d03d-198">\*\*\*\* ItemActivity 目前仅适用于 SharePoint 和 OneDrive for Business。</span><span class="sxs-lookup"><span data-stu-id="6d03d-198">**ItemActivity** is currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
