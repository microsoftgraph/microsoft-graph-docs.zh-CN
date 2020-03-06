---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 17939db5752c114c5c9180d318725c2553b4f1d7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531666"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="9e641-105">目录资源类型（已删除的项目）</span><span class="sxs-lookup"><span data-stu-id="9e641-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="9e641-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e641-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e641-107">表示目录中已删除的项目。</span><span class="sxs-lookup"><span data-stu-id="9e641-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="9e641-108">删除某个项目后，它会被添加到已删除项目“容器”中。</span><span class="sxs-lookup"><span data-stu-id="9e641-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="9e641-109">已删除的项目将保留最多 30 天的还原时间。</span><span class="sxs-lookup"><span data-stu-id="9e641-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="9e641-110">30 天后，这些项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="9e641-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="9e641-111">目前，仅支持[应用程序](application.md)、[组](group.md)和[用户](user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="9e641-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="9e641-112">Methods</span><span class="sxs-lookup"><span data-stu-id="9e641-112">Methods</span></span>

| <span data-ttu-id="9e641-113">方法</span><span class="sxs-lookup"><span data-stu-id="9e641-113">Method</span></span>         | <span data-ttu-id="9e641-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e641-114">Return Type</span></span> | <span data-ttu-id="9e641-115">说明</span><span class="sxs-lookup"><span data-stu-id="9e641-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="9e641-116">Get deleted item</span><span class="sxs-lookup"><span data-stu-id="9e641-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="9e641-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9e641-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="9e641-118">获取已删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="9e641-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="9e641-119">Restore deleted item</span><span class="sxs-lookup"><span data-stu-id="9e641-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="9e641-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9e641-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9e641-121">还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="9e641-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="9e641-122">List deleted items</span><span class="sxs-lookup"><span data-stu-id="9e641-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="9e641-123">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e641-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9e641-124">获取最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="9e641-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="9e641-125">Permanently delete an item</span><span class="sxs-lookup"><span data-stu-id="9e641-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="9e641-126">无</span><span class="sxs-lookup"><span data-stu-id="9e641-126">None</span></span> | <span data-ttu-id="9e641-127">永久删除项目。</span><span class="sxs-lookup"><span data-stu-id="9e641-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="9e641-128">列出用户拥有的已删除项目</span><span class="sxs-lookup"><span data-stu-id="9e641-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="9e641-129">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="9e641-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="9e641-130">列出用户拥有的目录项。</span><span class="sxs-lookup"><span data-stu-id="9e641-130">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9e641-131">关系</span><span class="sxs-lookup"><span data-stu-id="9e641-131">Relationships</span></span>
| <span data-ttu-id="9e641-132">关系</span><span class="sxs-lookup"><span data-stu-id="9e641-132">Relationship</span></span> | <span data-ttu-id="9e641-133">类型</span><span class="sxs-lookup"><span data-stu-id="9e641-133">Type</span></span>   |<span data-ttu-id="9e641-134">说明</span><span class="sxs-lookup"><span data-stu-id="9e641-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e641-135">deletedItems</span><span class="sxs-lookup"><span data-stu-id="9e641-135">deletedItems</span></span>|<span data-ttu-id="9e641-136">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e641-136">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9e641-137">最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="9e641-137">Recently deleted items.</span></span> <span data-ttu-id="9e641-138">只读。</span><span class="sxs-lookup"><span data-stu-id="9e641-138">Read-only.</span></span> <span data-ttu-id="9e641-139">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e641-139">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e641-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e641-140">JSON representation</span></span>
<span data-ttu-id="9e641-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e641-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="9e641-142">示例</span><span class="sxs-lookup"><span data-stu-id="9e641-142">Example</span></span>

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
