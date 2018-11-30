---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
ms.openlocfilehash: 3b2f77ea21f2352b0a8fa647af84d9b0af08a2ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041788"
---
# <a name="itemactionset-resource-type"></a><span data-ttu-id="3db1a-102">ItemActionSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="3db1a-102">ItemActionSet resource type</span></span>

> <span data-ttu-id="3db1a-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3db1a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3db1a-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3db1a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3db1a-105">**ItemActionSet** 资源提供有关构成项目上某个[活动][itemActivity]的操作信息。</span><span class="sxs-lookup"><span data-stu-id="3db1a-105">The **ItemActionSet** resource provides information about the actions that made up an [activity][itemActivity] on an item.</span></span>

[itemActivity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="3db1a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3db1a-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3db1a-107">属性</span><span class="sxs-lookup"><span data-stu-id="3db1a-107">Properties</span></span>

<span data-ttu-id="3db1a-108">以下是目前可用的操作。</span><span class="sxs-lookup"><span data-stu-id="3db1a-108">Below are the actions that are available today.</span></span>
<span data-ttu-id="3db1a-109">可能会在将来记录新操作，因此，请确保你的应用程序允许处理 **itemActionSet**，而无需执行任何应用程序理解的操作。</span><span class="sxs-lookup"><span data-stu-id="3db1a-109">New actions may get logged in the future, so make sure your app is tolerant of handling an **itemActionSet** without any actions that your app understands.</span></span>

| <span data-ttu-id="3db1a-110">属性名称</span><span class="sxs-lookup"><span data-stu-id="3db1a-110">Property name</span></span> | <span data-ttu-id="3db1a-111">类型</span><span class="sxs-lookup"><span data-stu-id="3db1a-111">Type</span></span>              | <span data-ttu-id="3db1a-112">说明</span><span class="sxs-lookup"><span data-stu-id="3db1a-112">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="3db1a-113">comment</span><span class="sxs-lookup"><span data-stu-id="3db1a-113">comment</span></span>       | <span data-ttu-id="3db1a-114">[commentAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-114">[commentAction][]</span></span> | <span data-ttu-id="3db1a-115">向项目添加了注释。</span><span class="sxs-lookup"><span data-stu-id="3db1a-115">A comment was added to the item.</span></span>
| <span data-ttu-id="3db1a-116">create</span><span class="sxs-lookup"><span data-stu-id="3db1a-116">create</span></span>        | <span data-ttu-id="3db1a-117">[createAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-117">[createAction][]</span></span>  | <span data-ttu-id="3db1a-118">创建了项目。</span><span class="sxs-lookup"><span data-stu-id="3db1a-118">An item was created.</span></span>
| <span data-ttu-id="3db1a-119">delete</span><span class="sxs-lookup"><span data-stu-id="3db1a-119">delete</span></span>        | <span data-ttu-id="3db1a-120">[deleteAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-120">[deleteAction][]</span></span>  | <span data-ttu-id="3db1a-121">删除了项目。</span><span class="sxs-lookup"><span data-stu-id="3db1a-121">An item was deleted.</span></span>
| <span data-ttu-id="3db1a-122">edit</span><span class="sxs-lookup"><span data-stu-id="3db1a-122">edit</span></span>          | <span data-ttu-id="3db1a-123">[editAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-123">[editAction][]</span></span>    | <span data-ttu-id="3db1a-124">编辑了项目。</span><span class="sxs-lookup"><span data-stu-id="3db1a-124">An item was edited.</span></span>
| <span data-ttu-id="3db1a-125">mention</span><span class="sxs-lookup"><span data-stu-id="3db1a-125">mention</span></span>       | <span data-ttu-id="3db1a-126">[mentionAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-126">[mentionAction][]</span></span> | <span data-ttu-id="3db1a-127">项目中提及用户。</span><span class="sxs-lookup"><span data-stu-id="3db1a-127">A user was mentioned in the item.</span></span>
| <span data-ttu-id="3db1a-128">move</span><span class="sxs-lookup"><span data-stu-id="3db1a-128">move</span></span>          | <span data-ttu-id="3db1a-129">[moveAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-129">[moveAction][]</span></span>    | <span data-ttu-id="3db1a-130">移动了项目。</span><span class="sxs-lookup"><span data-stu-id="3db1a-130">An item was moved.</span></span>
| <span data-ttu-id="3db1a-131">rename</span><span class="sxs-lookup"><span data-stu-id="3db1a-131">rename</span></span>        | <span data-ttu-id="3db1a-132">[renameAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-132">[renameAction][]</span></span>  | <span data-ttu-id="3db1a-133">重命名了项目。</span><span class="sxs-lookup"><span data-stu-id="3db1a-133">An item was renamed.</span></span>
| <span data-ttu-id="3db1a-134">restore</span><span class="sxs-lookup"><span data-stu-id="3db1a-134">restore</span></span>       | <span data-ttu-id="3db1a-135">[restoreAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-135">[restoreAction][]</span></span> | <span data-ttu-id="3db1a-136">恢复了项目。</span><span class="sxs-lookup"><span data-stu-id="3db1a-136">An item was restored.</span></span>
| <span data-ttu-id="3db1a-137">share</span><span class="sxs-lookup"><span data-stu-id="3db1a-137">share</span></span>         | <span data-ttu-id="3db1a-138">[shareAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-138">[shareAction][]</span></span>   | <span data-ttu-id="3db1a-139">共享了项目。</span><span class="sxs-lookup"><span data-stu-id="3db1a-139">An item was shared.</span></span>
| <span data-ttu-id="3db1a-140">version</span><span class="sxs-lookup"><span data-stu-id="3db1a-140">version</span></span>       | <span data-ttu-id="3db1a-141">[versionAction][]</span><span class="sxs-lookup"><span data-stu-id="3db1a-141">[versionAction][]</span></span> | <span data-ttu-id="3db1a-142">确定了项目的版本。</span><span class="sxs-lookup"><span data-stu-id="3db1a-142">An item was versioned.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="3db1a-153">注解</span><span class="sxs-lookup"><span data-stu-id="3db1a-153">Remarks</span></span>

<span data-ttu-id="3db1a-154">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="3db1a-154">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
