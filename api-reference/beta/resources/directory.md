---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b35c2c56c7033cd668b311c17169f5c719e5948
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062080"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="e9a83-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="e9a83-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9a83-106">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="e9a83-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="e9a83-107">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="e9a83-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="e9a83-108">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="e9a83-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="e9a83-109">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="e9a83-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="e9a83-110">目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。</span><span class="sxs-lookup"><span data-stu-id="e9a83-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e9a83-111">方法</span><span class="sxs-lookup"><span data-stu-id="e9a83-111">Methods</span></span>

| <span data-ttu-id="e9a83-112">方法</span><span class="sxs-lookup"><span data-stu-id="e9a83-112">Method</span></span>         | <span data-ttu-id="e9a83-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e9a83-113">Return Type</span></span> | <span data-ttu-id="e9a83-114">说明</span><span class="sxs-lookup"><span data-stu-id="e9a83-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="e9a83-115">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="e9a83-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="e9a83-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9a83-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="e9a83-117">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="e9a83-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="e9a83-118">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="e9a83-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="e9a83-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e9a83-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="e9a83-120">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="e9a83-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="e9a83-121">List deleted items</span><span class="sxs-lookup"><span data-stu-id="e9a83-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="e9a83-122">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="e9a83-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e9a83-123">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="e9a83-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="e9a83-124">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="e9a83-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="e9a83-125">无</span><span class="sxs-lookup"><span data-stu-id="e9a83-125">None</span></span> | <span data-ttu-id="e9a83-126">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="e9a83-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="e9a83-127">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="e9a83-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="e9a83-128">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="e9a83-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e9a83-129">列出用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="e9a83-129">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="e9a83-130">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="e9a83-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="e9a83-131">[featureRolloutPolicy](featurerolloutpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="e9a83-131">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="e9a83-132">检索 featureRolloutPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e9a83-132">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="e9a83-133">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e9a83-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="e9a83-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e9a83-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="e9a83-135">创建新的 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e9a83-135">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="e9a83-136">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e9a83-136">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="e9a83-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e9a83-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="e9a83-138">检索 featurerolloutpolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e9a83-138">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="e9a83-139">更新 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e9a83-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="e9a83-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e9a83-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="e9a83-141">更新 featurerolloutpolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e9a83-141">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="e9a83-142">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="e9a83-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="e9a83-143">无</span><span class="sxs-lookup"><span data-stu-id="e9a83-143">None</span></span> | <span data-ttu-id="e9a83-144">删除 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="e9a83-144">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e9a83-145">属性</span><span class="sxs-lookup"><span data-stu-id="e9a83-145">Properties</span></span>
| <span data-ttu-id="e9a83-146">属性</span><span class="sxs-lookup"><span data-stu-id="e9a83-146">Property</span></span>   | <span data-ttu-id="e9a83-147">类型</span><span class="sxs-lookup"><span data-stu-id="e9a83-147">Type</span></span> |<span data-ttu-id="e9a83-148">说明</span><span class="sxs-lookup"><span data-stu-id="e9a83-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9a83-149">id</span><span class="sxs-lookup"><span data-stu-id="e9a83-149">id</span></span>|<span data-ttu-id="e9a83-150">String</span><span class="sxs-lookup"><span data-stu-id="e9a83-150">String</span></span>| <span data-ttu-id="e9a83-151">对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="e9a83-151">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="e9a83-152">键。</span><span class="sxs-lookup"><span data-stu-id="e9a83-152">Key.</span></span> <span data-ttu-id="e9a83-153">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e9a83-153">Not nullable.</span></span> <span data-ttu-id="e9a83-154">只读。</span><span class="sxs-lookup"><span data-stu-id="e9a83-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9a83-155">关系</span><span class="sxs-lookup"><span data-stu-id="e9a83-155">Relationships</span></span>
| <span data-ttu-id="e9a83-156">关系</span><span class="sxs-lookup"><span data-stu-id="e9a83-156">Relationship</span></span> | <span data-ttu-id="e9a83-157">类型</span><span class="sxs-lookup"><span data-stu-id="e9a83-157">Type</span></span>   |<span data-ttu-id="e9a83-158">说明</span><span class="sxs-lookup"><span data-stu-id="e9a83-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9a83-159">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="e9a83-159">deleteditems</span></span>|<span data-ttu-id="e9a83-160">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e9a83-160">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e9a83-161">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="e9a83-161">Recently deleted items.</span></span> <span data-ttu-id="e9a83-162">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="e9a83-162">Read-only.</span></span> <span data-ttu-id="e9a83-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e9a83-163">Nullable.</span></span>|
|<span data-ttu-id="e9a83-164">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="e9a83-164">featureRolloutPolicies</span></span>|<span data-ttu-id="e9a83-165">[featureRolloutPolicy](featurerolloutpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="e9a83-165">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="e9a83-166">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e9a83-166">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9a83-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9a83-167">JSON representation</span></span>
<span data-ttu-id="e9a83-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9a83-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "suppressions": []
}
-->
