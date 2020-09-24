---
author: mohitpcad
title: 组资源类型
doc_type: resourcePageType
description: 代表术语库中使用的组。
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: aa86722dfd0a761525a8ec4d142ed27dc93be6c2
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258423"
---
# <a name="group-resource-type"></a><span data-ttu-id="d2156-103">组资源类型</span><span class="sxs-lookup"><span data-stu-id="d2156-103">Group resource type</span></span>

<span data-ttu-id="d2156-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="d2156-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="d2156-105">代表术语 [库](../resources/termstore-store.md)中使用的组。</span><span class="sxs-lookup"><span data-stu-id="d2156-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="d2156-106">组是一个逻辑层次结构，其中包含在其下设置的集合。</span><span class="sxs-lookup"><span data-stu-id="d2156-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="d2156-107">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="d2156-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d2156-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2156-108">Methods</span></span>

| <span data-ttu-id="d2156-109">方法</span><span class="sxs-lookup"><span data-stu-id="d2156-109">Method</span></span>                                                   | <span data-ttu-id="d2156-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2156-110">Return type</span></span>       |    <span data-ttu-id="d2156-111">说明</span><span class="sxs-lookup"><span data-stu-id="d2156-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="d2156-112">创建组</span><span class="sxs-lookup"><span data-stu-id="d2156-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="d2156-113">[termStore 的组]</span><span class="sxs-lookup"><span data-stu-id="d2156-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="d2156-114">在术语 [库]中创建一个组。</span><span class="sxs-lookup"><span data-stu-id="d2156-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="d2156-115">Get group</span><span class="sxs-lookup"><span data-stu-id="d2156-115">Get group</span></span>](../api/termstore-store-get-group.md)                           | <span data-ttu-id="d2156-116">[termStore 的组]</span><span class="sxs-lookup"><span data-stu-id="d2156-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="d2156-117">在术语 [库]中检索组的数据。</span><span class="sxs-lookup"><span data-stu-id="d2156-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="d2156-118">删除组</span><span class="sxs-lookup"><span data-stu-id="d2156-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="d2156-119">无</span><span class="sxs-lookup"><span data-stu-id="d2156-119">None</span></span> |  <span data-ttu-id="d2156-120">删除术语 [库]中的组。</span><span class="sxs-lookup"><span data-stu-id="d2156-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="d2156-121">属性</span><span class="sxs-lookup"><span data-stu-id="d2156-121">Properties</span></span>

| <span data-ttu-id="d2156-122">属性</span><span class="sxs-lookup"><span data-stu-id="d2156-122">Property</span></span>             | <span data-ttu-id="d2156-123">类型</span><span class="sxs-lookup"><span data-stu-id="d2156-123">Type</span></span>               | <span data-ttu-id="d2156-124">说明</span><span class="sxs-lookup"><span data-stu-id="d2156-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="d2156-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2156-125">createdDateTime</span></span>      | <span data-ttu-id="d2156-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2156-126">DateTimeOffset</span></span>     | <span data-ttu-id="d2156-127">创建组的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d2156-127">Date and time of group creation.</span></span> <span data-ttu-id="d2156-128">只读。</span><span class="sxs-lookup"><span data-stu-id="d2156-128">Read-only.</span></span>
| <span data-ttu-id="d2156-129">说明</span><span class="sxs-lookup"><span data-stu-id="d2156-129">description</span></span>          | <span data-ttu-id="d2156-130">string</span><span class="sxs-lookup"><span data-stu-id="d2156-130">string</span></span>             | <span data-ttu-id="d2156-131">说明：提供有关术语用法的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2156-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="d2156-132">id</span><span class="sxs-lookup"><span data-stu-id="d2156-132">id</span></span>                   | <span data-ttu-id="d2156-133">string</span><span class="sxs-lookup"><span data-stu-id="d2156-133">string</span></span>             | <span data-ttu-id="d2156-134">组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d2156-134">Unique identifier of group.</span></span> <span data-ttu-id="d2156-135">只读。</span><span class="sxs-lookup"><span data-stu-id="d2156-135">Read-Only.</span></span>
| <span data-ttu-id="d2156-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d2156-136">displayName</span></span>          | <span data-ttu-id="d2156-137">string</span><span class="sxs-lookup"><span data-stu-id="d2156-137">string</span></span>             | <span data-ttu-id="d2156-138">组的名称。</span><span class="sxs-lookup"><span data-stu-id="d2156-138">Name of group.</span></span>
| <span data-ttu-id="d2156-139">scope</span><span class="sxs-lookup"><span data-stu-id="d2156-139">scope</span></span>                | <span data-ttu-id="d2156-140">string</span><span class="sxs-lookup"><span data-stu-id="d2156-140">string</span></span>              | <span data-ttu-id="d2156-141">返回组的类型。</span><span class="sxs-lookup"><span data-stu-id="d2156-141">Returns type of group.</span></span> <span data-ttu-id="d2156-142">可能的值为 "global"、"system" 和 "siteCollection"。</span><span class="sxs-lookup"><span data-stu-id="d2156-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>

## <a name="relationships"></a><span data-ttu-id="d2156-143">关系</span><span class="sxs-lookup"><span data-stu-id="d2156-143">Relationships</span></span>
| <span data-ttu-id="d2156-144">关系</span><span class="sxs-lookup"><span data-stu-id="d2156-144">Relationship</span></span>       | <span data-ttu-id="d2156-145">类型</span><span class="sxs-lookup"><span data-stu-id="d2156-145">Type</span></span>                        | <span data-ttu-id="d2156-146">说明</span><span class="sxs-lookup"><span data-stu-id="d2156-146">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="d2156-147">下例</span><span class="sxs-lookup"><span data-stu-id="d2156-147">sets</span></span>           | <span data-ttu-id="d2156-148">[Microsoft termStore][] 集合</span><span class="sxs-lookup"><span data-stu-id="d2156-148">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="d2156-149">术语 [库]中的组下的所有集。</span><span class="sxs-lookup"><span data-stu-id="d2156-149">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2156-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2156-150">JSON representation</span></span>

<span data-ttu-id="d2156-151">以下是 **组** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2156-151">The following is a JSON representation of a **group** resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "string",
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "scope" : "microsoft.graph.termStore.groupScope",
  "displayName": "string" 
}
```



[identitySet]: identitySet.md
[termStore 设置]: termstore-set.md
[microsoft.graph.termStore.set]: termstore-set.md
[termStore 的组]: termstore-group.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
<!--
{
  "type": "#page.annotation",
  "description": "TermGroup is the entity used for managing permissions for the termSets in termStore",
  "keywords": "termGroup,facet,resource",
  "section": "documentation",
  "tocPath": "TermGroup",
  "tocBookmarks": {
    "Resources/termStore.group": "#"
  },
  "suppressions": []
}
-->


