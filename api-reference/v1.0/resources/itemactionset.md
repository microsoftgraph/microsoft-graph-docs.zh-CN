---
author: daspek
ms.author: dspektor
title: ItemActionSet 资源类型
description: ItemActionSet 对象提供有关作为项目活动的一部分发生的操作的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9563f138c5074e1317927e8e9636eeba42beed35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967448"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="b87a9-103">itemActionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="b87a9-103">itemActionSet resource type</span></span>

<span data-ttu-id="b87a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b87a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b87a9-105">**ItemActionSet**资源提供有关对项目[活动][itemActivity]的操作的信息。</span><span class="sxs-lookup"><span data-stu-id="b87a9-105">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="b87a9-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b87a9-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b87a9-107">属性</span><span class="sxs-lookup"><span data-stu-id="b87a9-107">Properties</span></span>

<span data-ttu-id="b87a9-108">以下操作当前可用。</span><span class="sxs-lookup"><span data-stu-id="b87a9-108">The following actions are currently available.</span></span> <span data-ttu-id="b87a9-109">由于将来可能会添加新操作，因此请确保您的应用程序可以处理包含未知操作的 **itemActionSet** 。</span><span class="sxs-lookup"><span data-stu-id="b87a9-109">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="b87a9-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="b87a9-110">Property name</span></span> | <span data-ttu-id="b87a9-111">类型</span><span class="sxs-lookup"><span data-stu-id="b87a9-111">Type</span></span>              | <span data-ttu-id="b87a9-112">说明</span><span class="sxs-lookup"><span data-stu-id="b87a9-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="b87a9-113">comment</span><span class="sxs-lookup"><span data-stu-id="b87a9-113">comment</span></span>       | <span data-ttu-id="b87a9-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-114">[commentAction][]</span></span> | <span data-ttu-id="b87a9-115">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="b87a9-115">A comment was added to the item.</span></span>
| <span data-ttu-id="b87a9-116">create</span><span class="sxs-lookup"><span data-stu-id="b87a9-116">create</span></span>        | <span data-ttu-id="b87a9-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-117">[createAction][]</span></span>  | <span data-ttu-id="b87a9-118">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="b87a9-118">An item was created.</span></span>
| <span data-ttu-id="b87a9-119">delete</span><span class="sxs-lookup"><span data-stu-id="b87a9-119">delete</span></span>        | <span data-ttu-id="b87a9-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-120">[deleteAction][]</span></span>  | <span data-ttu-id="b87a9-121">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="b87a9-121">An item was deleted.</span></span>
| <span data-ttu-id="b87a9-122">edit</span><span class="sxs-lookup"><span data-stu-id="b87a9-122">edit</span></span>          | <span data-ttu-id="b87a9-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-123">[editAction][]</span></span>    | <span data-ttu-id="b87a9-124">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="b87a9-124">An item was edited.</span></span>
| <span data-ttu-id="b87a9-125">mention</span><span class="sxs-lookup"><span data-stu-id="b87a9-125">mention</span></span>       | <span data-ttu-id="b87a9-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-126">[mentionAction][]</span></span> | <span data-ttu-id="b87a9-127">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="b87a9-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="b87a9-128">move</span><span class="sxs-lookup"><span data-stu-id="b87a9-128">move</span></span>          | <span data-ttu-id="b87a9-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-129">[moveAction][]</span></span>    | <span data-ttu-id="b87a9-130">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="b87a9-130">An item was moved.</span></span>
| <span data-ttu-id="b87a9-131">rename</span><span class="sxs-lookup"><span data-stu-id="b87a9-131">rename</span></span>        | <span data-ttu-id="b87a9-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-132">[renameAction][]</span></span>  | <span data-ttu-id="b87a9-133">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="b87a9-133">An item was renamed.</span></span>
| <span data-ttu-id="b87a9-134">restore</span><span class="sxs-lookup"><span data-stu-id="b87a9-134">restore</span></span>       | <span data-ttu-id="b87a9-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-135">[restoreAction][]</span></span> | <span data-ttu-id="b87a9-136">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="b87a9-136">An item was restored.</span></span>
| <span data-ttu-id="b87a9-137">share</span><span class="sxs-lookup"><span data-stu-id="b87a9-137">share</span></span>         | <span data-ttu-id="b87a9-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-138">[shareAction][]</span></span>   | <span data-ttu-id="b87a9-139">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="b87a9-139">An item was shared.</span></span>
| <span data-ttu-id="b87a9-140">version</span><span class="sxs-lookup"><span data-stu-id="b87a9-140">version</span></span>       | <span data-ttu-id="b87a9-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="b87a9-141">[versionAction][]</span></span> | <span data-ttu-id="b87a9-142">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="b87a9-142">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="b87a9-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b87a9-153">JSON representation</span></span>

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

