---
author: daspek
description: ItemActionSet 资源提供有关对项目执行 [活动] [itemActivity] 的操作的信息。
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b3b803b719ad14fabf19574a55360009c3dda14e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523133"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="cf98c-103">ItemActionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf98c-103">ItemActionSet resource type</span></span>

<span data-ttu-id="cf98c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cf98c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf98c-105">**ItemActionSet** 资源提供有关构成项目上某个[活动][itemActivity]的操作信息。</span><span class="sxs-lookup"><span data-stu-id="cf98c-105">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="cf98c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf98c-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cf98c-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf98c-107">Properties</span></span>

<span data-ttu-id="cf98c-108">以下是目前可用的操作。</span><span class="sxs-lookup"><span data-stu-id="cf98c-108">Below are the actions that are available today.</span></span>
<span data-ttu-id="cf98c-109">可能会在将来记录新操作，因此，请确保你的应用程序允许处理 **itemActionSet**，而无需执行任何应用程序理解的操作。</span><span class="sxs-lookup"><span data-stu-id="cf98c-109">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="cf98c-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="cf98c-110">Property name</span></span> | <span data-ttu-id="cf98c-111">类型</span><span class="sxs-lookup"><span data-stu-id="cf98c-111">Type</span></span>              | <span data-ttu-id="cf98c-112">说明</span><span class="sxs-lookup"><span data-stu-id="cf98c-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="cf98c-113">comment</span><span class="sxs-lookup"><span data-stu-id="cf98c-113">comment</span></span>       | <span data-ttu-id="cf98c-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-114">[commentAction][]</span></span> | <span data-ttu-id="cf98c-115">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="cf98c-115">A comment was added to the item.</span></span>
| <span data-ttu-id="cf98c-116">create</span><span class="sxs-lookup"><span data-stu-id="cf98c-116">create</span></span>        | <span data-ttu-id="cf98c-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-117">[createAction][]</span></span>  | <span data-ttu-id="cf98c-118">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="cf98c-118">An item was created.</span></span>
| <span data-ttu-id="cf98c-119">delete</span><span class="sxs-lookup"><span data-stu-id="cf98c-119">delete</span></span>        | <span data-ttu-id="cf98c-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-120">[deleteAction][]</span></span>  | <span data-ttu-id="cf98c-121">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="cf98c-121">An item was deleted.</span></span>
| <span data-ttu-id="cf98c-122">edit</span><span class="sxs-lookup"><span data-stu-id="cf98c-122">edit</span></span>          | <span data-ttu-id="cf98c-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-123">[editAction][]</span></span>    | <span data-ttu-id="cf98c-124">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="cf98c-124">An item was edited.</span></span>
| <span data-ttu-id="cf98c-125">mention</span><span class="sxs-lookup"><span data-stu-id="cf98c-125">mention</span></span>       | <span data-ttu-id="cf98c-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-126">[mentionAction][]</span></span> | <span data-ttu-id="cf98c-127">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="cf98c-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="cf98c-128">move</span><span class="sxs-lookup"><span data-stu-id="cf98c-128">move</span></span>          | <span data-ttu-id="cf98c-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-129">[moveAction][]</span></span>    | <span data-ttu-id="cf98c-130">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="cf98c-130">An item was moved.</span></span>
| <span data-ttu-id="cf98c-131">rename</span><span class="sxs-lookup"><span data-stu-id="cf98c-131">rename</span></span>        | <span data-ttu-id="cf98c-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-132">[renameAction][]</span></span>  | <span data-ttu-id="cf98c-133">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="cf98c-133">An item was renamed.</span></span>
| <span data-ttu-id="cf98c-134">restore</span><span class="sxs-lookup"><span data-stu-id="cf98c-134">restore</span></span>       | <span data-ttu-id="cf98c-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-135">[restoreAction][]</span></span> | <span data-ttu-id="cf98c-136">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="cf98c-136">An item was restored.</span></span>
| <span data-ttu-id="cf98c-137">share</span><span class="sxs-lookup"><span data-stu-id="cf98c-137">share</span></span>         | <span data-ttu-id="cf98c-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-138">[shareAction][]</span></span>   | <span data-ttu-id="cf98c-139">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="cf98c-139">An item was shared.</span></span>
| <span data-ttu-id="cf98c-140">version</span><span class="sxs-lookup"><span data-stu-id="cf98c-140">version</span></span>       | <span data-ttu-id="cf98c-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="cf98c-141">[versionAction][]</span></span> | <span data-ttu-id="cf98c-142">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="cf98c-142">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="cf98c-153">注解</span><span class="sxs-lookup"><span data-stu-id="cf98c-153">Remarks</span></span>

<span data-ttu-id="cf98c-154">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="cf98c-154">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
