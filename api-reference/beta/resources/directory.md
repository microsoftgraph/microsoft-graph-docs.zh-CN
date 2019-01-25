---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22c5b959f87b6178fa406bc4fd5d00ad52e5cf55
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517482"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="13075-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="13075-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13075-106">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="13075-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="13075-107">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="13075-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="13075-108">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="13075-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="13075-109">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="13075-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="13075-110">目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。</span><span class="sxs-lookup"><span data-stu-id="13075-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="13075-111">方法</span><span class="sxs-lookup"><span data-stu-id="13075-111">Methods</span></span>

| <span data-ttu-id="13075-112">方法</span><span class="sxs-lookup"><span data-stu-id="13075-112">Method</span></span>         | <span data-ttu-id="13075-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="13075-113">Return Type</span></span> | <span data-ttu-id="13075-114">说明</span><span class="sxs-lookup"><span data-stu-id="13075-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="13075-115">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="13075-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="13075-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="13075-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="13075-117">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="13075-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="13075-118">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="13075-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="13075-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="13075-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="13075-120">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="13075-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="13075-121">List deleted items</span><span class="sxs-lookup"><span data-stu-id="13075-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="13075-122">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13075-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="13075-123">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="13075-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="13075-124">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="13075-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="13075-125">无</span><span class="sxs-lookup"><span data-stu-id="13075-125">None</span></span> | <span data-ttu-id="13075-126">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="13075-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="13075-127">由用户拥有的删除列表项</span><span class="sxs-lookup"><span data-stu-id="13075-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="13075-128">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13075-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="13075-129">列出了由用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="13075-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="13075-130">属性</span><span class="sxs-lookup"><span data-stu-id="13075-130">Properties</span></span>
| <span data-ttu-id="13075-131">属性</span><span class="sxs-lookup"><span data-stu-id="13075-131">Property</span></span>   | <span data-ttu-id="13075-132">类型</span><span class="sxs-lookup"><span data-stu-id="13075-132">Type</span></span> |<span data-ttu-id="13075-133">说明</span><span class="sxs-lookup"><span data-stu-id="13075-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13075-134">id</span><span class="sxs-lookup"><span data-stu-id="13075-134">id</span></span>|<span data-ttu-id="13075-135">String</span><span class="sxs-lookup"><span data-stu-id="13075-135">String</span></span>| <span data-ttu-id="13075-136">对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="13075-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="13075-137">键。</span><span class="sxs-lookup"><span data-stu-id="13075-137">Key.</span></span> <span data-ttu-id="13075-138">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="13075-138">Not nullable.</span></span> <span data-ttu-id="13075-139">只读。</span><span class="sxs-lookup"><span data-stu-id="13075-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13075-140">关系</span><span class="sxs-lookup"><span data-stu-id="13075-140">Relationships</span></span>
| <span data-ttu-id="13075-141">关系</span><span class="sxs-lookup"><span data-stu-id="13075-141">Relationship</span></span> | <span data-ttu-id="13075-142">类型</span><span class="sxs-lookup"><span data-stu-id="13075-142">Type</span></span>   |<span data-ttu-id="13075-143">说明</span><span class="sxs-lookup"><span data-stu-id="13075-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13075-144">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="13075-144">deleteditems</span></span>|<span data-ttu-id="13075-145">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13075-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="13075-146">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="13075-146">Recently deleted items.</span></span> <span data-ttu-id="13075-147">只读。</span><span class="sxs-lookup"><span data-stu-id="13075-147">Read-only.</span></span> <span data-ttu-id="13075-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="13075-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13075-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13075-149">JSON representation</span></span>
<span data-ttu-id="13075-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13075-150">Here is a JSON representation of the resource.</span></span>

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
