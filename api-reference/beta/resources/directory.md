---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 531b688fe64f4cadb7a23cbc7db6cba313b86a0c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440474"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="651dd-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="651dd-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="651dd-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="651dd-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="651dd-107">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="651dd-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="651dd-108">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="651dd-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="651dd-109">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="651dd-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="651dd-110">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="651dd-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="651dd-111">目前，仅应用程序、组和用户资源支持已删除的项目[](application.md)功能。 [](group.md) [](user.md)</span><span class="sxs-lookup"><span data-stu-id="651dd-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="651dd-112">Methods</span><span class="sxs-lookup"><span data-stu-id="651dd-112">Methods</span></span>

| <span data-ttu-id="651dd-113">方法</span><span class="sxs-lookup"><span data-stu-id="651dd-113">Method</span></span>         | <span data-ttu-id="651dd-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="651dd-114">Return Type</span></span> | <span data-ttu-id="651dd-115">说明</span><span class="sxs-lookup"><span data-stu-id="651dd-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="651dd-116">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="651dd-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="651dd-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="651dd-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="651dd-118">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="651dd-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="651dd-119">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="651dd-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="651dd-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="651dd-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="651dd-121">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="651dd-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="651dd-122">List deleted items</span><span class="sxs-lookup"><span data-stu-id="651dd-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="651dd-123">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="651dd-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="651dd-124">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="651dd-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="651dd-125">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="651dd-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="651dd-126">无</span><span class="sxs-lookup"><span data-stu-id="651dd-126">None</span></span> | <span data-ttu-id="651dd-127">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="651dd-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="651dd-128">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="651dd-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="651dd-129">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="651dd-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="651dd-130">列出用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="651dd-130">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="651dd-131">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="651dd-131">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="651dd-132">[featureRolloutPolicy](featurerolloutpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="651dd-132">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="651dd-133">检索 featureRolloutPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="651dd-133">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="651dd-134">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="651dd-134">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="651dd-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="651dd-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="651dd-136">创建新的 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="651dd-136">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="651dd-137">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="651dd-137">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="651dd-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="651dd-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="651dd-139">检索 featurerolloutpolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="651dd-139">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="651dd-140">更新 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="651dd-140">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="651dd-141">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="651dd-141">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="651dd-142">更新 featurerolloutpolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="651dd-142">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="651dd-143">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="651dd-143">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="651dd-144">无</span><span class="sxs-lookup"><span data-stu-id="651dd-144">None</span></span> | <span data-ttu-id="651dd-145">删除 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="651dd-145">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="651dd-146">属性</span><span class="sxs-lookup"><span data-stu-id="651dd-146">Properties</span></span>
| <span data-ttu-id="651dd-147">属性</span><span class="sxs-lookup"><span data-stu-id="651dd-147">Property</span></span>   | <span data-ttu-id="651dd-148">类型</span><span class="sxs-lookup"><span data-stu-id="651dd-148">Type</span></span> |<span data-ttu-id="651dd-149">说明</span><span class="sxs-lookup"><span data-stu-id="651dd-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="651dd-150">id</span><span class="sxs-lookup"><span data-stu-id="651dd-150">id</span></span>|<span data-ttu-id="651dd-151">String</span><span class="sxs-lookup"><span data-stu-id="651dd-151">String</span></span>| <span data-ttu-id="651dd-152">对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="651dd-152">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="651dd-153">键。</span><span class="sxs-lookup"><span data-stu-id="651dd-153">Key.</span></span> <span data-ttu-id="651dd-154">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="651dd-154">Not nullable.</span></span> <span data-ttu-id="651dd-155">只读。</span><span class="sxs-lookup"><span data-stu-id="651dd-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="651dd-156">关系</span><span class="sxs-lookup"><span data-stu-id="651dd-156">Relationships</span></span>
| <span data-ttu-id="651dd-157">关系</span><span class="sxs-lookup"><span data-stu-id="651dd-157">Relationship</span></span> | <span data-ttu-id="651dd-158">类型</span><span class="sxs-lookup"><span data-stu-id="651dd-158">Type</span></span>   |<span data-ttu-id="651dd-159">说明</span><span class="sxs-lookup"><span data-stu-id="651dd-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="651dd-160">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="651dd-160">deleteditems</span></span>|<span data-ttu-id="651dd-161">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="651dd-161">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="651dd-162">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="651dd-162">Recently deleted items.</span></span> <span data-ttu-id="651dd-163">只读。</span><span class="sxs-lookup"><span data-stu-id="651dd-163">Read-only.</span></span> <span data-ttu-id="651dd-164">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="651dd-164">Nullable.</span></span>|
|<span data-ttu-id="651dd-165">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="651dd-165">featureRolloutPolicies</span></span>|<span data-ttu-id="651dd-166">[featureRolloutPolicy](featurerolloutpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="651dd-166">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="651dd-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="651dd-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="651dd-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="651dd-168">JSON representation</span></span>
<span data-ttu-id="651dd-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="651dd-169">Here is a JSON representation of the resource.</span></span>

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


