---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
ms.openlocfilehash: 74b4d1ff94b567557fd90701b1c4bae479a8317e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048671"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="dd507-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="dd507-105">directory resource type (deleted items)</span></span>

> <span data-ttu-id="dd507-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dd507-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd507-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dd507-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd507-108">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="dd507-108">Represents a deleted item in the directory.</span></span> <span data-ttu-id="dd507-109">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="dd507-109">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="dd507-110">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="dd507-110">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="dd507-111">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="dd507-111">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="dd507-112">目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。</span><span class="sxs-lookup"><span data-stu-id="dd507-112">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dd507-113">方法</span><span class="sxs-lookup"><span data-stu-id="dd507-113">Methods</span></span>

| <span data-ttu-id="dd507-114">方法</span><span class="sxs-lookup"><span data-stu-id="dd507-114">Method</span></span>         | <span data-ttu-id="dd507-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd507-115">Return Type</span></span> | <span data-ttu-id="dd507-116">说明</span><span class="sxs-lookup"><span data-stu-id="dd507-116">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="dd507-117">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="dd507-117">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="dd507-118">directoryObject</span><span class="sxs-lookup"><span data-stu-id="dd507-118">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="dd507-119">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="dd507-119">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="dd507-120">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="dd507-120">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="dd507-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="dd507-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="dd507-122">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="dd507-122">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="dd507-123">List deleted items</span><span class="sxs-lookup"><span data-stu-id="dd507-123">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="dd507-124">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd507-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dd507-125">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="dd507-125">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="dd507-126">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="dd507-126">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="dd507-127">无</span><span class="sxs-lookup"><span data-stu-id="dd507-127">None</span></span> | <span data-ttu-id="dd507-128">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="dd507-128">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="dd507-129">由用户拥有的删除列表项</span><span class="sxs-lookup"><span data-stu-id="dd507-129">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="dd507-130">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd507-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="dd507-131">列出了由用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="dd507-131">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd507-132">属性</span><span class="sxs-lookup"><span data-stu-id="dd507-132">Properties</span></span>
| <span data-ttu-id="dd507-133">属性</span><span class="sxs-lookup"><span data-stu-id="dd507-133">Property</span></span>   | <span data-ttu-id="dd507-134">类型</span><span class="sxs-lookup"><span data-stu-id="dd507-134">Type</span></span> |<span data-ttu-id="dd507-135">说明</span><span class="sxs-lookup"><span data-stu-id="dd507-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd507-136">id</span><span class="sxs-lookup"><span data-stu-id="dd507-136">id</span></span>|<span data-ttu-id="dd507-137">String</span><span class="sxs-lookup"><span data-stu-id="dd507-137">String</span></span>| <span data-ttu-id="dd507-138">对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="dd507-138">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="dd507-139">键。</span><span class="sxs-lookup"><span data-stu-id="dd507-139">Key.</span></span> <span data-ttu-id="dd507-140">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="dd507-140">Not nullable.</span></span> <span data-ttu-id="dd507-141">只读。</span><span class="sxs-lookup"><span data-stu-id="dd507-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd507-142">Relationships</span><span class="sxs-lookup"><span data-stu-id="dd507-142">Relationships</span></span>
| <span data-ttu-id="dd507-143">关系</span><span class="sxs-lookup"><span data-stu-id="dd507-143">Relationship</span></span> | <span data-ttu-id="dd507-144">类型</span><span class="sxs-lookup"><span data-stu-id="dd507-144">Type</span></span>   |<span data-ttu-id="dd507-145">说明</span><span class="sxs-lookup"><span data-stu-id="dd507-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd507-146">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="dd507-146">deleteditems</span></span>|<span data-ttu-id="dd507-147">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd507-147">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dd507-148">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="dd507-148">Recently deleted items.</span></span> <span data-ttu-id="dd507-149">只读。</span><span class="sxs-lookup"><span data-stu-id="dd507-149">Read-only.</span></span> <span data-ttu-id="dd507-150">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dd507-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd507-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd507-151">JSON representation</span></span>
<span data-ttu-id="dd507-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd507-152">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->