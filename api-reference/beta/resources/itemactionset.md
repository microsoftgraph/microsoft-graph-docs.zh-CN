---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: b88f7514f7871e3c3850da91e4cd90b32f3a69c4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345405"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="98c13-102">ItemActionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="98c13-102">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98c13-103">**ItemActionSet** 资源提供有关构成项目上某个[活动][itemActivity]的操作信息。</span><span class="sxs-lookup"><span data-stu-id="98c13-103">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="98c13-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98c13-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

## <a name="properties"></a><span data-ttu-id="98c13-105">属性</span><span class="sxs-lookup"><span data-stu-id="98c13-105">Properties</span></span>

<span data-ttu-id="98c13-106">以下是目前可用的操作。</span><span class="sxs-lookup"><span data-stu-id="98c13-106">Below are the actions that are available today.</span></span>
<span data-ttu-id="98c13-107">可能会在将来记录新操作，因此，请确保你的应用程序允许处理 **itemActionSet**，而无需执行任何应用程序理解的操作。</span><span class="sxs-lookup"><span data-stu-id="98c13-107">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="98c13-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="98c13-108">Property name</span></span> | <span data-ttu-id="98c13-109">类型</span><span class="sxs-lookup"><span data-stu-id="98c13-109">Type</span></span>              | <span data-ttu-id="98c13-110">说明</span><span class="sxs-lookup"><span data-stu-id="98c13-110">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="98c13-111">comment</span><span class="sxs-lookup"><span data-stu-id="98c13-111">comment</span></span>       | <span data-ttu-id="98c13-112">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-112">[commentAction][]</span></span> | <span data-ttu-id="98c13-113">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="98c13-113">A comment was added to the item.</span></span>
| <span data-ttu-id="98c13-114">create</span><span class="sxs-lookup"><span data-stu-id="98c13-114">create</span></span>        | <span data-ttu-id="98c13-115">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-115">[createAction][]</span></span>  | <span data-ttu-id="98c13-116">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="98c13-116">An item was created.</span></span>
| <span data-ttu-id="98c13-117">delete</span><span class="sxs-lookup"><span data-stu-id="98c13-117">delete</span></span>        | <span data-ttu-id="98c13-118">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-118">[deleteAction][]</span></span>  | <span data-ttu-id="98c13-119">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="98c13-119">An item was deleted.</span></span>
| <span data-ttu-id="98c13-120">edit</span><span class="sxs-lookup"><span data-stu-id="98c13-120">edit</span></span>          | <span data-ttu-id="98c13-121">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-121">[editAction][]</span></span>    | <span data-ttu-id="98c13-122">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="98c13-122">An item was edited.</span></span>
| <span data-ttu-id="98c13-123">mention</span><span class="sxs-lookup"><span data-stu-id="98c13-123">mention</span></span>       | <span data-ttu-id="98c13-124">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-124">[mentionAction][]</span></span> | <span data-ttu-id="98c13-125">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="98c13-125">A user was mentioned in the item.</span></span>
| <span data-ttu-id="98c13-126">move</span><span class="sxs-lookup"><span data-stu-id="98c13-126">move</span></span>          | <span data-ttu-id="98c13-127">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-127">[moveAction][]</span></span>    | <span data-ttu-id="98c13-128">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="98c13-128">An item was moved.</span></span>
| <span data-ttu-id="98c13-129">rename</span><span class="sxs-lookup"><span data-stu-id="98c13-129">rename</span></span>        | <span data-ttu-id="98c13-130">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-130">[renameAction][]</span></span>  | <span data-ttu-id="98c13-131">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="98c13-131">An item was renamed.</span></span>
| <span data-ttu-id="98c13-132">restore</span><span class="sxs-lookup"><span data-stu-id="98c13-132">restore</span></span>       | <span data-ttu-id="98c13-133">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-133">[restoreAction][]</span></span> | <span data-ttu-id="98c13-134">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="98c13-134">An item was restored.</span></span>
| <span data-ttu-id="98c13-135">share</span><span class="sxs-lookup"><span data-stu-id="98c13-135">share</span></span>         | <span data-ttu-id="98c13-136">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-136">[shareAction][]</span></span>   | <span data-ttu-id="98c13-137">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="98c13-137">An item was shared.</span></span>
| <span data-ttu-id="98c13-138">version</span><span class="sxs-lookup"><span data-stu-id="98c13-138">version</span></span>       | <span data-ttu-id="98c13-139">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="98c13-139">[versionAction][]</span></span> | <span data-ttu-id="98c13-140">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="98c13-140">An item was versioned.</span></span>

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a><span data-ttu-id="98c13-151">注解</span><span class="sxs-lookup"><span data-stu-id="98c13-151">Remarks</span></span>

<span data-ttu-id="98c13-152">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="98c13-152">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->
