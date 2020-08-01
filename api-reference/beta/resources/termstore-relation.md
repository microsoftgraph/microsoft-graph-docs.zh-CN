---
title: 关系资源类型
description: 表示术语库中术语之间的关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c4e12069ff50362a667a94aec28b715096616917
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539160"
---
# <a name="relation-resource-type"></a><span data-ttu-id="acf55-103">关系资源类型</span><span class="sxs-lookup"><span data-stu-id="acf55-103">relation resource type</span></span>

<span data-ttu-id="acf55-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="acf55-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acf55-105">表示术语[库]中[术语](../resources/termstore-term.md)之间的关系。</span><span class="sxs-lookup"><span data-stu-id="acf55-105">Represents the relationship between [terms](../resources/termstore-term.md) in a term [store].</span></span> <span data-ttu-id="acf55-106">目前支持两种类型的关系： pin 和重用。</span><span class="sxs-lookup"><span data-stu-id="acf55-106">Currently two types of relationships are supported: pin and reuse.</span></span> 

<span data-ttu-id="acf55-107">在 pin 关系中，术语可固定在不同术语集中的不同术语下。</span><span class="sxs-lookup"><span data-stu-id="acf55-107">In a pin relationship, a term can be pinned under a different term in a different term set.</span></span> <span data-ttu-id="acf55-108">在固定的关系中，只能在创建了术语的术语集中添加术语的新子项。</span><span class="sxs-lookup"><span data-stu-id="acf55-108">In a pinned relationship, new children to the term can only be added in the term set in which the term was created.</span></span> <span data-ttu-id="acf55-109">术语下的层次结构中的任何更改都将反映到固定术语的集中。</span><span class="sxs-lookup"><span data-stu-id="acf55-109">Any change in the hierarchy under the term is reflected across the sets in which the term was pinned.</span></span> 

<span data-ttu-id="acf55-110">重复使用关系类似于固定的关系，不同之处在于，可重复使用的术语的更改可从任何可重用术语的层次结构进行。</span><span class="sxs-lookup"><span data-stu-id="acf55-110">The reuse relationship is similar to the pinned relationship except that changes to the reused term can be made from any hierarchy in which the term is reused.</span></span> <span data-ttu-id="acf55-111">此外，对重复使用的术语的层次结构更改不会反映在重复使用该术语的其他术语集中。</span><span class="sxs-lookup"><span data-stu-id="acf55-111">Also, a change in hierarchy made to the reused term does not get reflected in the other term sets in which the term is reused.</span></span>

<span data-ttu-id="acf55-112">继承自[entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="acf55-112">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="acf55-113">方法</span><span class="sxs-lookup"><span data-stu-id="acf55-113">Methods</span></span>
|<span data-ttu-id="acf55-114">方法</span><span class="sxs-lookup"><span data-stu-id="acf55-114">Method</span></span>|<span data-ttu-id="acf55-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="acf55-115">Return type</span></span>|<span data-ttu-id="acf55-116">说明</span><span class="sxs-lookup"><span data-stu-id="acf55-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="acf55-117">列表关系</span><span class="sxs-lookup"><span data-stu-id="acf55-117">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="acf55-118">[termstore](../resources/termstore-relation.md)集合的关系</span><span class="sxs-lookup"><span data-stu-id="acf55-118">[microsoft.graph.termstore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="acf55-119">检索**关系**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="acf55-119">Retrieve a list of **relation** objects.</span></span>|
|[<span data-ttu-id="acf55-120">创建关系</span><span class="sxs-lookup"><span data-stu-id="acf55-120">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="acf55-121">microsoft termstore</span><span class="sxs-lookup"><span data-stu-id="acf55-121">microsoft.graph.termstore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="acf55-122">创建新的**relation**对象。</span><span class="sxs-lookup"><span data-stu-id="acf55-122">Create a new **relation** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="acf55-123">属性</span><span class="sxs-lookup"><span data-stu-id="acf55-123">Properties</span></span>
|<span data-ttu-id="acf55-124">属性</span><span class="sxs-lookup"><span data-stu-id="acf55-124">Property</span></span>|<span data-ttu-id="acf55-125">类型</span><span class="sxs-lookup"><span data-stu-id="acf55-125">Type</span></span>|<span data-ttu-id="acf55-126">说明</span><span class="sxs-lookup"><span data-stu-id="acf55-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acf55-127">id</span><span class="sxs-lookup"><span data-stu-id="acf55-127">id</span></span>|<span data-ttu-id="acf55-128">String</span><span class="sxs-lookup"><span data-stu-id="acf55-128">String</span></span>|<span data-ttu-id="acf55-129">关系的 ID。</span><span class="sxs-lookup"><span data-stu-id="acf55-129">The ID of the relation.</span></span>|
|<span data-ttu-id="acf55-130">关系</span><span class="sxs-lookup"><span data-stu-id="acf55-130">relationship</span></span>|<span data-ttu-id="acf55-131">String</span><span class="sxs-lookup"><span data-stu-id="acf55-131">String</span></span>|<span data-ttu-id="acf55-132">关系的类型。</span><span class="sxs-lookup"><span data-stu-id="acf55-132">The type of relation.</span></span> <span data-ttu-id="acf55-133">可取值为：`pin`、`reuse`。</span><span class="sxs-lookup"><span data-stu-id="acf55-133">Possible values are: `pin`, `reuse`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acf55-134">关系</span><span class="sxs-lookup"><span data-stu-id="acf55-134">Relationships</span></span>
|<span data-ttu-id="acf55-135">关系</span><span class="sxs-lookup"><span data-stu-id="acf55-135">Relationship</span></span>|<span data-ttu-id="acf55-136">类型</span><span class="sxs-lookup"><span data-stu-id="acf55-136">Type</span></span>|<span data-ttu-id="acf55-137">说明</span><span class="sxs-lookup"><span data-stu-id="acf55-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acf55-138">fromTerm</span><span class="sxs-lookup"><span data-stu-id="acf55-138">fromTerm</span></span>|[<span data-ttu-id="acf55-139">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="acf55-139">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="acf55-140">关系的 from[术语]。</span><span class="sxs-lookup"><span data-stu-id="acf55-140">The from [term] of the relation.</span></span> <span data-ttu-id="acf55-141">定义关系的术语。</span><span class="sxs-lookup"><span data-stu-id="acf55-141">The term from which the relationship is defined.</span></span> <span data-ttu-id="acf55-142">空值指示关系是直接与[集]。</span><span class="sxs-lookup"><span data-stu-id="acf55-142">A null value would indicate the relation is directly with the [set].</span></span> |
|<span data-ttu-id="acf55-143">set</span><span class="sxs-lookup"><span data-stu-id="acf55-143">set</span></span>|[<span data-ttu-id="acf55-144">termStore 设置</span><span class="sxs-lookup"><span data-stu-id="acf55-144">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="acf55-145">与关系相关的[集合]。</span><span class="sxs-lookup"><span data-stu-id="acf55-145">The [set] in which the relation is relevant.</span></span>|
|<span data-ttu-id="acf55-146">toTerm</span><span class="sxs-lookup"><span data-stu-id="acf55-146">toTerm</span></span>|[<span data-ttu-id="acf55-147">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="acf55-147">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="acf55-148">关系的 to[术语]。</span><span class="sxs-lookup"><span data-stu-id="acf55-148">The to [term] of the relation.</span></span> <span data-ttu-id="acf55-149">为其定义接的术语。</span><span class="sxs-lookup"><span data-stu-id="acf55-149">The term to which the realtionship is defined.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acf55-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acf55-150">JSON representation</span></span>
<span data-ttu-id="acf55-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acf55-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.relation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "String (identifier)",
  "relationship": "String"
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.relations]: termstore-relation.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[术语]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation": "#"
  },
  "suppressions": []
}
-->
