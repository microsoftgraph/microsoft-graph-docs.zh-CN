---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
ms.openlocfilehash: e83ace1a50998b6645e059fe0f63e3922497c1cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010687"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="50070-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="50070-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="50070-106">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="50070-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="50070-107">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="50070-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="50070-108">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="50070-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="50070-109">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="50070-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="50070-110">目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。</span><span class="sxs-lookup"><span data-stu-id="50070-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="50070-111">方法</span><span class="sxs-lookup"><span data-stu-id="50070-111">Methods</span></span>

| <span data-ttu-id="50070-112">方法</span><span class="sxs-lookup"><span data-stu-id="50070-112">Method</span></span>         | <span data-ttu-id="50070-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="50070-113">Return Type</span></span> | <span data-ttu-id="50070-114">说明</span><span class="sxs-lookup"><span data-stu-id="50070-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="50070-115">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="50070-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="50070-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="50070-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="50070-117">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="50070-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="50070-118">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="50070-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="50070-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="50070-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="50070-120">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="50070-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="50070-121">List deleted items</span><span class="sxs-lookup"><span data-stu-id="50070-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="50070-122">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50070-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="50070-123">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="50070-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="50070-124">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="50070-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="50070-125">无</span><span class="sxs-lookup"><span data-stu-id="50070-125">None</span></span> | <span data-ttu-id="50070-126">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="50070-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="50070-127">由用户拥有的删除列表项</span><span class="sxs-lookup"><span data-stu-id="50070-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="50070-128">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50070-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="50070-129">列出了由用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="50070-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="50070-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="50070-130">Relationships</span></span>
| <span data-ttu-id="50070-131">关系</span><span class="sxs-lookup"><span data-stu-id="50070-131">Relationship</span></span> | <span data-ttu-id="50070-132">类型</span><span class="sxs-lookup"><span data-stu-id="50070-132">Type</span></span>   |<span data-ttu-id="50070-133">说明</span><span class="sxs-lookup"><span data-stu-id="50070-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50070-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="50070-134">deletedItems</span></span>|<span data-ttu-id="50070-135">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50070-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="50070-136">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="50070-136">Recently deleted items.</span></span> <span data-ttu-id="50070-137">只读。</span><span class="sxs-lookup"><span data-stu-id="50070-137">Read-only.</span></span> <span data-ttu-id="50070-138">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="50070-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50070-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50070-139">JSON representation</span></span>
<span data-ttu-id="50070-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50070-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="50070-141">示例</span><span class="sxs-lookup"><span data-stu-id="50070-141">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
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