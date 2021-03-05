---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9c46e671f707a8e31c172e4a078647cd7d103d48
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472732"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="dfd35-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="dfd35-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="dfd35-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfd35-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfd35-107">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="dfd35-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="dfd35-108">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="dfd35-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="dfd35-109">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="dfd35-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="dfd35-110">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="dfd35-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="dfd35-111">目前，仅应用程序、组和用户资源支持已删除的项目[](application.md)功能。 [](group.md) [](user.md)</span><span class="sxs-lookup"><span data-stu-id="dfd35-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="dfd35-112">Methods</span><span class="sxs-lookup"><span data-stu-id="dfd35-112">Methods</span></span>

| <span data-ttu-id="dfd35-113">方法</span><span class="sxs-lookup"><span data-stu-id="dfd35-113">Method</span></span>         | <span data-ttu-id="dfd35-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfd35-114">Return Type</span></span> | <span data-ttu-id="dfd35-115">说明</span><span class="sxs-lookup"><span data-stu-id="dfd35-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="dfd35-116">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="dfd35-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="dfd35-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="dfd35-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="dfd35-118">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="dfd35-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="dfd35-119">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="dfd35-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="dfd35-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="dfd35-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="dfd35-121">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="dfd35-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="dfd35-122">List deleted items</span><span class="sxs-lookup"><span data-stu-id="dfd35-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="dfd35-123">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfd35-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dfd35-124">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="dfd35-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="dfd35-125">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="dfd35-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="dfd35-126">无</span><span class="sxs-lookup"><span data-stu-id="dfd35-126">None</span></span> | <span data-ttu-id="dfd35-127">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="dfd35-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="dfd35-128">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="dfd35-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="dfd35-129">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="dfd35-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="dfd35-130">列出用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="dfd35-130">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dfd35-131">关系</span><span class="sxs-lookup"><span data-stu-id="dfd35-131">Relationships</span></span>
| <span data-ttu-id="dfd35-132">关系</span><span class="sxs-lookup"><span data-stu-id="dfd35-132">Relationship</span></span> | <span data-ttu-id="dfd35-133">类型</span><span class="sxs-lookup"><span data-stu-id="dfd35-133">Type</span></span>   |<span data-ttu-id="dfd35-134">说明</span><span class="sxs-lookup"><span data-stu-id="dfd35-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfd35-135">deletedItems</span><span class="sxs-lookup"><span data-stu-id="dfd35-135">deletedItems</span></span>|<span data-ttu-id="dfd35-136">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfd35-136">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="dfd35-137">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="dfd35-137">Recently deleted items.</span></span> <span data-ttu-id="dfd35-138">只读。</span><span class="sxs-lookup"><span data-stu-id="dfd35-138">Read-only.</span></span> <span data-ttu-id="dfd35-139">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dfd35-139">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfd35-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfd35-140">JSON representation</span></span>
<span data-ttu-id="dfd35-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfd35-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="dfd35-142">示例</span><span class="sxs-lookup"><span data-stu-id="dfd35-142">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```http
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

