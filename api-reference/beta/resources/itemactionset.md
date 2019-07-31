---
author: daspek
description: ItemActionSet 资源提供有关对项目执行 [活动] [itemActivity] 的操作的信息。
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8053942fe96011b018e46681d69d308f65aa5d5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967145"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="508b8-103">ItemActionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="508b8-103">ItemActionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="508b8-104">**ItemActionSet** 资源提供有关构成项目上某个[活动][itemActivity]的操作信息。</span><span class="sxs-lookup"><span data-stu-id="508b8-104">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="508b8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="508b8-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="508b8-106">属性</span><span class="sxs-lookup"><span data-stu-id="508b8-106">Properties</span></span>

<span data-ttu-id="508b8-107">以下是目前可用的操作。</span><span class="sxs-lookup"><span data-stu-id="508b8-107">Below are the actions that are available today.</span></span>
<span data-ttu-id="508b8-108">可能会在将来记录新操作，因此，请确保你的应用程序允许处理 **itemActionSet**，而无需执行任何应用程序理解的操作。</span><span class="sxs-lookup"><span data-stu-id="508b8-108">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="508b8-109">属性名</span><span class="sxs-lookup"><span data-stu-id="508b8-109">Property name</span></span> | <span data-ttu-id="508b8-110">类型</span><span class="sxs-lookup"><span data-stu-id="508b8-110">Type</span></span>              | <span data-ttu-id="508b8-111">说明</span><span class="sxs-lookup"><span data-stu-id="508b8-111">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="508b8-112">comment</span><span class="sxs-lookup"><span data-stu-id="508b8-112">comment</span></span>       | <span data-ttu-id="508b8-113">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-113">[commentAction][]</span></span> | <span data-ttu-id="508b8-114">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="508b8-114">A comment was added to the item.</span></span>
| <span data-ttu-id="508b8-115">create</span><span class="sxs-lookup"><span data-stu-id="508b8-115">create</span></span>        | <span data-ttu-id="508b8-116">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-116">[createAction][]</span></span>  | <span data-ttu-id="508b8-117">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="508b8-117">An item was created.</span></span>
| <span data-ttu-id="508b8-118">delete</span><span class="sxs-lookup"><span data-stu-id="508b8-118">delete</span></span>        | <span data-ttu-id="508b8-119">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-119">[deleteAction][]</span></span>  | <span data-ttu-id="508b8-120">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="508b8-120">An item was deleted.</span></span>
| <span data-ttu-id="508b8-121">edit</span><span class="sxs-lookup"><span data-stu-id="508b8-121">edit</span></span>          | <span data-ttu-id="508b8-122">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-122">[editAction][]</span></span>    | <span data-ttu-id="508b8-123">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="508b8-123">An item was edited.</span></span>
| <span data-ttu-id="508b8-124">mention</span><span class="sxs-lookup"><span data-stu-id="508b8-124">mention</span></span>       | <span data-ttu-id="508b8-125">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-125">[mentionAction][]</span></span> | <span data-ttu-id="508b8-126">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="508b8-126">A user was mentioned in the item.</span></span>
| <span data-ttu-id="508b8-127">move</span><span class="sxs-lookup"><span data-stu-id="508b8-127">move</span></span>          | <span data-ttu-id="508b8-128">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-128">[moveAction][]</span></span>    | <span data-ttu-id="508b8-129">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="508b8-129">An item was moved.</span></span>
| <span data-ttu-id="508b8-130">rename</span><span class="sxs-lookup"><span data-stu-id="508b8-130">rename</span></span>        | <span data-ttu-id="508b8-131">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-131">[renameAction][]</span></span>  | <span data-ttu-id="508b8-132">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="508b8-132">An item was renamed.</span></span>
| <span data-ttu-id="508b8-133">restore</span><span class="sxs-lookup"><span data-stu-id="508b8-133">restore</span></span>       | <span data-ttu-id="508b8-134">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-134">[restoreAction][]</span></span> | <span data-ttu-id="508b8-135">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="508b8-135">An item was restored.</span></span>
| <span data-ttu-id="508b8-136">share</span><span class="sxs-lookup"><span data-stu-id="508b8-136">share</span></span>         | <span data-ttu-id="508b8-137">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-137">[shareAction][]</span></span>   | <span data-ttu-id="508b8-138">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="508b8-138">An item was shared.</span></span>
| <span data-ttu-id="508b8-139">version</span><span class="sxs-lookup"><span data-stu-id="508b8-139">version</span></span>       | <span data-ttu-id="508b8-140">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="508b8-140">[versionAction][]</span></span> | <span data-ttu-id="508b8-141">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="508b8-141">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="508b8-152">注解</span><span class="sxs-lookup"><span data-stu-id="508b8-152">Remarks</span></span>

<span data-ttu-id="508b8-153">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="508b8-153">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
