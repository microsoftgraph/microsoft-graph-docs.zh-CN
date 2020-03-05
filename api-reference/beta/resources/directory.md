---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5aa90644a679c34eb7d2f9b53a5759b6b4293fed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507049"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="d1b9b-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="d1b9b-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="d1b9b-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d1b9b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1b9b-107">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="d1b9b-108">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="d1b9b-109">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="d1b9b-110">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="d1b9b-111">目前，仅支持[应用程序](application.md)、[组](group.md)和[用户](user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="d1b9b-112">方法</span><span class="sxs-lookup"><span data-stu-id="d1b9b-112">Methods</span></span>

| <span data-ttu-id="d1b9b-113">方法</span><span class="sxs-lookup"><span data-stu-id="d1b9b-113">Method</span></span>         | <span data-ttu-id="d1b9b-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1b9b-114">Return Type</span></span> | <span data-ttu-id="d1b9b-115">说明</span><span class="sxs-lookup"><span data-stu-id="d1b9b-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="d1b9b-116">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="d1b9b-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="d1b9b-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d1b9b-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="d1b9b-118">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="d1b9b-119">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="d1b9b-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="d1b9b-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="d1b9b-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="d1b9b-121">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="d1b9b-122">List deleted items</span><span class="sxs-lookup"><span data-stu-id="d1b9b-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="d1b9b-123">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1b9b-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d1b9b-124">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="d1b9b-125">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="d1b9b-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="d1b9b-126">无</span><span class="sxs-lookup"><span data-stu-id="d1b9b-126">None</span></span> | <span data-ttu-id="d1b9b-127">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="d1b9b-128">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="d1b9b-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="d1b9b-129">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1b9b-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="d1b9b-130">列出用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-130">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="d1b9b-131">列出 featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="d1b9b-131">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="d1b9b-132">[featureRolloutPolicy](featurerolloutpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="d1b9b-132">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="d1b9b-133">检索 featureRolloutPolicy 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-133">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="d1b9b-134">创建 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1b9b-134">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="d1b9b-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1b9b-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="d1b9b-136">创建新的 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-136">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="d1b9b-137">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1b9b-137">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="d1b9b-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1b9b-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="d1b9b-139">检索 featurerolloutpolicy 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-139">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="d1b9b-140">更新 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1b9b-140">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="d1b9b-141">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1b9b-141">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="d1b9b-142">更新 featurerolloutpolicy 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-142">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="d1b9b-143">删除 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="d1b9b-143">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="d1b9b-144">无</span><span class="sxs-lookup"><span data-stu-id="d1b9b-144">None</span></span> | <span data-ttu-id="d1b9b-145">删除 featureRolloutPolicy 对象。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-145">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d1b9b-146">属性</span><span class="sxs-lookup"><span data-stu-id="d1b9b-146">Properties</span></span>
| <span data-ttu-id="d1b9b-147">属性</span><span class="sxs-lookup"><span data-stu-id="d1b9b-147">Property</span></span>   | <span data-ttu-id="d1b9b-148">类型</span><span class="sxs-lookup"><span data-stu-id="d1b9b-148">Type</span></span> |<span data-ttu-id="d1b9b-149">说明</span><span class="sxs-lookup"><span data-stu-id="d1b9b-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1b9b-150">id</span><span class="sxs-lookup"><span data-stu-id="d1b9b-150">id</span></span>|<span data-ttu-id="d1b9b-151">String</span><span class="sxs-lookup"><span data-stu-id="d1b9b-151">String</span></span>| <span data-ttu-id="d1b9b-152">对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-152">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="d1b9b-153">键。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-153">Key.</span></span> <span data-ttu-id="d1b9b-154">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-154">Not nullable.</span></span> <span data-ttu-id="d1b9b-155">只读。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1b9b-156">关系</span><span class="sxs-lookup"><span data-stu-id="d1b9b-156">Relationships</span></span>
| <span data-ttu-id="d1b9b-157">关系</span><span class="sxs-lookup"><span data-stu-id="d1b9b-157">Relationship</span></span> | <span data-ttu-id="d1b9b-158">类型</span><span class="sxs-lookup"><span data-stu-id="d1b9b-158">Type</span></span>   |<span data-ttu-id="d1b9b-159">说明</span><span class="sxs-lookup"><span data-stu-id="d1b9b-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1b9b-160">DeletedItems</span><span class="sxs-lookup"><span data-stu-id="d1b9b-160">deleteditems</span></span>|<span data-ttu-id="d1b9b-161">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1b9b-161">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="d1b9b-162">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-162">Recently deleted items.</span></span> <span data-ttu-id="d1b9b-163">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-163">Read-only.</span></span> <span data-ttu-id="d1b9b-164">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-164">Nullable.</span></span>|
|<span data-ttu-id="d1b9b-165">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="d1b9b-165">featureRolloutPolicies</span></span>|<span data-ttu-id="d1b9b-166">[featureRolloutPolicy](featurerolloutpolicy.md)集合</span><span class="sxs-lookup"><span data-stu-id="d1b9b-166">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="d1b9b-167">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1b9b-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1b9b-168">JSON representation</span></span>
<span data-ttu-id="d1b9b-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1b9b-169">Here is a JSON representation of the resource.</span></span>

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
