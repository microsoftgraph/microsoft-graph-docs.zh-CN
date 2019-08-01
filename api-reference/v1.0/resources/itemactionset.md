---
author: daspek
ms.author: dspektor
title: ItemActionSet 资源类型
description: ItemActionSet 对象提供有关作为项目活动的一部分发生的操作的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a28a3380761e2d1914d7c088e5927fc5d3addd4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036720"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="3e0e7-103">itemActionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e0e7-103">itemActionSet resource type</span></span>

<span data-ttu-id="3e0e7-104">**ItemActionSet**资源提供有关对项目[活动][itemActivity]的操作的信息。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-104">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="3e0e7-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="3e0e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e0e7-106">Properties</span></span>

<span data-ttu-id="3e0e7-107">以下操作当前可用。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-107">The following actions are currently available.</span></span> <span data-ttu-id="3e0e7-108">由于将来可能会添加新操作, 因此请确保您的应用程序可以处理包含未知操作的**itemActionSet** 。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-108">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="3e0e7-109">属性名</span><span class="sxs-lookup"><span data-stu-id="3e0e7-109">Property name</span></span> | <span data-ttu-id="3e0e7-110">类型</span><span class="sxs-lookup"><span data-stu-id="3e0e7-110">Type</span></span>              | <span data-ttu-id="3e0e7-111">说明</span><span class="sxs-lookup"><span data-stu-id="3e0e7-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="3e0e7-112">comment</span><span class="sxs-lookup"><span data-stu-id="3e0e7-112">comment</span></span>       | <span data-ttu-id="3e0e7-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-113">[commentAction][]</span></span> | <span data-ttu-id="3e0e7-114">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-114">A comment was added to the item.</span></span>
| <span data-ttu-id="3e0e7-115">create</span><span class="sxs-lookup"><span data-stu-id="3e0e7-115">create</span></span>        | <span data-ttu-id="3e0e7-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-116">[createAction][]</span></span>  | <span data-ttu-id="3e0e7-117">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-117">An item was created.</span></span>
| <span data-ttu-id="3e0e7-118">delete</span><span class="sxs-lookup"><span data-stu-id="3e0e7-118">delete</span></span>        | <span data-ttu-id="3e0e7-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-119">[deleteAction][]</span></span>  | <span data-ttu-id="3e0e7-120">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-120">An item was deleted.</span></span>
| <span data-ttu-id="3e0e7-121">edit</span><span class="sxs-lookup"><span data-stu-id="3e0e7-121">edit</span></span>          | <span data-ttu-id="3e0e7-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-122">[editAction][]</span></span>    | <span data-ttu-id="3e0e7-123">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-123">An item was edited.</span></span>
| <span data-ttu-id="3e0e7-124">mention</span><span class="sxs-lookup"><span data-stu-id="3e0e7-124">mention</span></span>       | <span data-ttu-id="3e0e7-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-125">[mentionAction][]</span></span> | <span data-ttu-id="3e0e7-126">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="3e0e7-127">move</span><span class="sxs-lookup"><span data-stu-id="3e0e7-127">move</span></span>          | <span data-ttu-id="3e0e7-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-128">[moveAction][]</span></span>    | <span data-ttu-id="3e0e7-129">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-129">An item was moved.</span></span>
| <span data-ttu-id="3e0e7-130">rename</span><span class="sxs-lookup"><span data-stu-id="3e0e7-130">rename</span></span>        | <span data-ttu-id="3e0e7-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-131">[renameAction][]</span></span>  | <span data-ttu-id="3e0e7-132">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-132">An item was renamed.</span></span>
| <span data-ttu-id="3e0e7-133">restore</span><span class="sxs-lookup"><span data-stu-id="3e0e7-133">restore</span></span>       | <span data-ttu-id="3e0e7-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-134">[restoreAction][]</span></span> | <span data-ttu-id="3e0e7-135">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-135">An item was restored.</span></span>
| <span data-ttu-id="3e0e7-136">share</span><span class="sxs-lookup"><span data-stu-id="3e0e7-136">share</span></span>         | <span data-ttu-id="3e0e7-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-137">[shareAction][]</span></span>   | <span data-ttu-id="3e0e7-138">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-138">An item was shared.</span></span>
| <span data-ttu-id="3e0e7-139">version</span><span class="sxs-lookup"><span data-stu-id="3e0e7-139">version</span></span>       | <span data-ttu-id="3e0e7-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="3e0e7-140">[versionAction][]</span></span> | <span data-ttu-id="3e0e7-141">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="3e0e7-141">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="3e0e7-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e0e7-152">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
