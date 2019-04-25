---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22c5b959f87b6178fa406bc4fd5d00ad52e5cf55
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535241"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="1eced-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="1eced-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eced-106">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="1eced-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="1eced-107">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="1eced-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="1eced-108">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="1eced-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="1eced-109">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="1eced-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="1eced-110">目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。</span><span class="sxs-lookup"><span data-stu-id="1eced-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1eced-111">方法</span><span class="sxs-lookup"><span data-stu-id="1eced-111">Methods</span></span>

| <span data-ttu-id="1eced-112">方法</span><span class="sxs-lookup"><span data-stu-id="1eced-112">Method</span></span>         | <span data-ttu-id="1eced-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="1eced-113">Return Type</span></span> | <span data-ttu-id="1eced-114">说明</span><span class="sxs-lookup"><span data-stu-id="1eced-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="1eced-115">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="1eced-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="1eced-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1eced-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="1eced-117">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="1eced-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="1eced-118">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="1eced-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="1eced-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1eced-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1eced-120">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="1eced-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="1eced-121">List deleted items</span><span class="sxs-lookup"><span data-stu-id="1eced-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="1eced-122">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="1eced-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1eced-123">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="1eced-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="1eced-124">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="1eced-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="1eced-125">无</span><span class="sxs-lookup"><span data-stu-id="1eced-125">None</span></span> | <span data-ttu-id="1eced-126">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="1eced-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="1eced-127">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="1eced-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="1eced-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="1eced-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="1eced-129">列出用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="1eced-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="1eced-130">属性</span><span class="sxs-lookup"><span data-stu-id="1eced-130">Properties</span></span>
| <span data-ttu-id="1eced-131">属性</span><span class="sxs-lookup"><span data-stu-id="1eced-131">Property</span></span>   | <span data-ttu-id="1eced-132">类型</span><span class="sxs-lookup"><span data-stu-id="1eced-132">Type</span></span> |<span data-ttu-id="1eced-133">说明</span><span class="sxs-lookup"><span data-stu-id="1eced-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1eced-134">id</span><span class="sxs-lookup"><span data-stu-id="1eced-134">id</span></span>|<span data-ttu-id="1eced-135">String</span><span class="sxs-lookup"><span data-stu-id="1eced-135">String</span></span>| <span data-ttu-id="1eced-136">对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="1eced-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="1eced-137">键。</span><span class="sxs-lookup"><span data-stu-id="1eced-137">Key.</span></span> <span data-ttu-id="1eced-138">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1eced-138">Not nullable.</span></span> <span data-ttu-id="1eced-139">只读。</span><span class="sxs-lookup"><span data-stu-id="1eced-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1eced-140">关系</span><span class="sxs-lookup"><span data-stu-id="1eced-140">Relationships</span></span>
| <span data-ttu-id="1eced-141">关系</span><span class="sxs-lookup"><span data-stu-id="1eced-141">Relationship</span></span> | <span data-ttu-id="1eced-142">类型</span><span class="sxs-lookup"><span data-stu-id="1eced-142">Type</span></span>   |<span data-ttu-id="1eced-143">说明</span><span class="sxs-lookup"><span data-stu-id="1eced-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1eced-144">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="1eced-144">deleteditems</span></span>|<span data-ttu-id="1eced-145">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1eced-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1eced-146">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="1eced-146">Recently deleted items.</span></span> <span data-ttu-id="1eced-147">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="1eced-147">Read-only.</span></span> <span data-ttu-id="1eced-148">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1eced-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1eced-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1eced-149">JSON representation</span></span>
<span data-ttu-id="1eced-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1eced-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
