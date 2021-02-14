---
author: daspek
title: ItemActionSet 资源类型
description: itemActionSet 对象提供有关作为项目活动一部分进行的操作的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 6dcc630b76adcbec3c719a43280e4b28d1d933e5
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239252"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="13f2c-103">itemActionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="13f2c-103">itemActionSet resource type</span></span>

<span data-ttu-id="13f2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13f2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13f2c-105">**itemActionSet** 资源提供有关在项目上 [创建活动的操作][itemActivity]的信息。</span><span class="sxs-lookup"><span data-stu-id="13f2c-105">The **itemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

><span data-ttu-id="13f2c-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="13f2c-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[itemActivity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="13f2c-107">属性</span><span class="sxs-lookup"><span data-stu-id="13f2c-107">Properties</span></span>

<span data-ttu-id="13f2c-108">当前提供以下操作。</span><span class="sxs-lookup"><span data-stu-id="13f2c-108">The following actions are currently available.</span></span> <span data-ttu-id="13f2c-109">由于将来可能会添加新操作，因此请确保你的应用可以处理包含 **未知操作的项目** 操作集。</span><span class="sxs-lookup"><span data-stu-id="13f2c-109">Because new actions might be added in the future, make sure that your app can handle an **itemActionSet** that includes unknown actions.</span></span>

| <span data-ttu-id="13f2c-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="13f2c-110">Property name</span></span> | <span data-ttu-id="13f2c-111">类型</span><span class="sxs-lookup"><span data-stu-id="13f2c-111">Type</span></span>              | <span data-ttu-id="13f2c-112">说明</span><span class="sxs-lookup"><span data-stu-id="13f2c-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="13f2c-113">comment</span><span class="sxs-lookup"><span data-stu-id="13f2c-113">comment</span></span>       | <span data-ttu-id="13f2c-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-114">[commentAction][]</span></span> | <span data-ttu-id="13f2c-115">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="13f2c-115">A comment was added to the item.</span></span>
| <span data-ttu-id="13f2c-116">create</span><span class="sxs-lookup"><span data-stu-id="13f2c-116">create</span></span>        | <span data-ttu-id="13f2c-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-117">[createAction][]</span></span>  | <span data-ttu-id="13f2c-118">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="13f2c-118">An item was created.</span></span>
| <span data-ttu-id="13f2c-119">delete</span><span class="sxs-lookup"><span data-stu-id="13f2c-119">delete</span></span>        | <span data-ttu-id="13f2c-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-120">[deleteAction][]</span></span>  | <span data-ttu-id="13f2c-121">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="13f2c-121">An item was deleted.</span></span>
| <span data-ttu-id="13f2c-122">edit</span><span class="sxs-lookup"><span data-stu-id="13f2c-122">edit</span></span>          | <span data-ttu-id="13f2c-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-123">[editAction][]</span></span>    | <span data-ttu-id="13f2c-124">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="13f2c-124">An item was edited.</span></span>
| <span data-ttu-id="13f2c-125">mention</span><span class="sxs-lookup"><span data-stu-id="13f2c-125">mention</span></span>       | <span data-ttu-id="13f2c-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-126">[mentionAction][]</span></span> | <span data-ttu-id="13f2c-127">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="13f2c-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="13f2c-128">move</span><span class="sxs-lookup"><span data-stu-id="13f2c-128">move</span></span>          | <span data-ttu-id="13f2c-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-129">[moveAction][]</span></span>    | <span data-ttu-id="13f2c-130">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="13f2c-130">An item was moved.</span></span>
| <span data-ttu-id="13f2c-131">rename</span><span class="sxs-lookup"><span data-stu-id="13f2c-131">rename</span></span>        | <span data-ttu-id="13f2c-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-132">[renameAction][]</span></span>  | <span data-ttu-id="13f2c-133">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="13f2c-133">An item was renamed.</span></span>
| <span data-ttu-id="13f2c-134">restore</span><span class="sxs-lookup"><span data-stu-id="13f2c-134">restore</span></span>       | <span data-ttu-id="13f2c-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-135">[restoreAction][]</span></span> | <span data-ttu-id="13f2c-136">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="13f2c-136">An item was restored.</span></span>
| <span data-ttu-id="13f2c-137">share</span><span class="sxs-lookup"><span data-stu-id="13f2c-137">share</span></span>         | <span data-ttu-id="13f2c-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-138">[shareAction][]</span></span>   | <span data-ttu-id="13f2c-139">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="13f2c-139">An item was shared.</span></span>
| <span data-ttu-id="13f2c-140">version</span><span class="sxs-lookup"><span data-stu-id="13f2c-140">version</span></span>       | <span data-ttu-id="13f2c-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="13f2c-141">[versionAction][]</span></span> | <span data-ttu-id="13f2c-142">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="13f2c-142">An item was versioned.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="13f2c-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13f2c-153">JSON representation</span></span>

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

