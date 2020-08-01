---
title: 设置资源类型
description: 代表术语库中的集合。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5e74e0a603d088c7964b13fad51018171642c6ec
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539159"
---
# <a name="set-resource-type"></a><span data-ttu-id="1c23a-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="1c23a-103">set resource type</span></span>

<span data-ttu-id="1c23a-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="1c23a-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c23a-105">代表术语[库]中使用的集合。</span><span class="sxs-lookup"><span data-stu-id="1c23a-105">Represents the set used in a term [store].</span></span> <span data-ttu-id="1c23a-106">该集合表示包含分层术语集合的单位。</span><span class="sxs-lookup"><span data-stu-id="1c23a-106">The set represents a unit which contains a collection of hierarchical terms.</span></span> <span data-ttu-id="1c23a-107">一个[组]可以包含多个集。</span><span class="sxs-lookup"><span data-stu-id="1c23a-107">A [group] can contain multiple sets.</span></span>

<span data-ttu-id="1c23a-108">继承自[entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="1c23a-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1c23a-109">方法</span><span class="sxs-lookup"><span data-stu-id="1c23a-109">Methods</span></span>
|<span data-ttu-id="1c23a-110">方法</span><span class="sxs-lookup"><span data-stu-id="1c23a-110">Method</span></span>|<span data-ttu-id="1c23a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c23a-111">Return type</span></span>|<span data-ttu-id="1c23a-112">说明</span><span class="sxs-lookup"><span data-stu-id="1c23a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1c23a-113">列表集</span><span class="sxs-lookup"><span data-stu-id="1c23a-113">List sets</span></span>](../api/termstore-group-list-sets.md)|<span data-ttu-id="1c23a-114">[termStore 的]集合</span><span class="sxs-lookup"><span data-stu-id="1c23a-114">collection [microsoft.graph.termStore.set]</span></span> | <span data-ttu-id="1c23a-115">返回术语[存储][组]中包含的集的列表</span><span class="sxs-lookup"><span data-stu-id="1c23a-115">Returns list of sets contained within a [group] of a term [store]</span></span> |
|[<span data-ttu-id="1c23a-116">创建集</span><span class="sxs-lookup"><span data-stu-id="1c23a-116">Create set</span></span>](../api/termstore-set-post.md)|[<span data-ttu-id="1c23a-117">termStore 设置</span><span class="sxs-lookup"><span data-stu-id="1c23a-117">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="1c23a-118">在术语[库]中创建新的 set 对象。</span><span class="sxs-lookup"><span data-stu-id="1c23a-118">Create a new set object in a term [store].</span></span>|
|[<span data-ttu-id="1c23a-119">创建术语</span><span class="sxs-lookup"><span data-stu-id="1c23a-119">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="1c23a-120">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="1c23a-120">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="1c23a-121">在术语[库]中创建新的[术语]对象。</span><span class="sxs-lookup"><span data-stu-id="1c23a-121">Create a new [term] object in a term [store].</span></span>|
|[<span data-ttu-id="1c23a-122">Get set</span><span class="sxs-lookup"><span data-stu-id="1c23a-122">Get set</span></span>](../api/termstore-set-get.md)|[<span data-ttu-id="1c23a-123">termStore 设置</span><span class="sxs-lookup"><span data-stu-id="1c23a-123">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)| <span data-ttu-id="1c23a-124">在术语[库]中获取一个 set 对象。</span><span class="sxs-lookup"><span data-stu-id="1c23a-124">Get a set object in a term [store].</span></span>|
|[<span data-ttu-id="1c23a-125">获取术语</span><span class="sxs-lookup"><span data-stu-id="1c23a-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="1c23a-126">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="1c23a-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)| <span data-ttu-id="1c23a-127">在术语[库]中获取[术语]对象。</span><span class="sxs-lookup"><span data-stu-id="1c23a-127">Get a [term] object in a term [store].</span></span>|
|[<span data-ttu-id="1c23a-128">更新集</span><span class="sxs-lookup"><span data-stu-id="1c23a-128">Update set</span></span>](../api/termstore-set-update.md)|[<span data-ttu-id="1c23a-129">termStore 设置</span><span class="sxs-lookup"><span data-stu-id="1c23a-129">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="1c23a-130">更新术语[库]中的 set 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1c23a-130">Update the properties of a set object in a term [store].</span></span>|
|[<span data-ttu-id="1c23a-131">删除集</span><span class="sxs-lookup"><span data-stu-id="1c23a-131">Delete set</span></span>](../api/termstore-set-delete.md)|<span data-ttu-id="1c23a-132">无</span><span class="sxs-lookup"><span data-stu-id="1c23a-132">None</span></span>|<span data-ttu-id="1c23a-133">删除术语[库]中的 set 对象。</span><span class="sxs-lookup"><span data-stu-id="1c23a-133">Deletes a set object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="1c23a-134">属性</span><span class="sxs-lookup"><span data-stu-id="1c23a-134">Properties</span></span>
|<span data-ttu-id="1c23a-135">属性</span><span class="sxs-lookup"><span data-stu-id="1c23a-135">Property</span></span>|<span data-ttu-id="1c23a-136">类型</span><span class="sxs-lookup"><span data-stu-id="1c23a-136">Type</span></span>|<span data-ttu-id="1c23a-137">说明</span><span class="sxs-lookup"><span data-stu-id="1c23a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c23a-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c23a-138">createdDateTime</span></span>|<span data-ttu-id="1c23a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c23a-139">DateTimeOffset</span></span>|<span data-ttu-id="1c23a-140">创建集的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1c23a-140">Date and time of set creation.</span></span> <span data-ttu-id="1c23a-141">只读。</span><span class="sxs-lookup"><span data-stu-id="1c23a-141">Read-only.</span></span>|
|<span data-ttu-id="1c23a-142">说明</span><span class="sxs-lookup"><span data-stu-id="1c23a-142">description</span></span>|<span data-ttu-id="1c23a-143">String</span><span class="sxs-lookup"><span data-stu-id="1c23a-143">String</span></span>|<span data-ttu-id="1c23a-144">说明：提供有关术语用法的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1c23a-144">Description giving details on the term usage.</span></span>|
|<span data-ttu-id="1c23a-145">id</span><span class="sxs-lookup"><span data-stu-id="1c23a-145">id</span></span>|<span data-ttu-id="1c23a-146">字符串</span><span class="sxs-lookup"><span data-stu-id="1c23a-146">String</span></span>|<span data-ttu-id="1c23a-147">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1c23a-147">Unique identifier.</span></span> <span data-ttu-id="1c23a-148">只读。</span><span class="sxs-lookup"><span data-stu-id="1c23a-148">Read-only.</span></span>|
|<span data-ttu-id="1c23a-149">localizedNames</span><span class="sxs-lookup"><span data-stu-id="1c23a-149">localizedNames</span></span>|<span data-ttu-id="1c23a-150">[termStore](../resources/termstore-localizedname.md)集合的 localizedName</span><span class="sxs-lookup"><span data-stu-id="1c23a-150">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="1c23a-151">每个 languageTag 的集的名称。</span><span class="sxs-lookup"><span data-stu-id="1c23a-151">Name of the set for each languageTag.</span></span>|
|<span data-ttu-id="1c23a-152">properties</span><span class="sxs-lookup"><span data-stu-id="1c23a-152">properties</span></span>|<span data-ttu-id="1c23a-153">[键值](../resources/keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c23a-153">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="1c23a-154">集的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="1c23a-154">Custom properties for the set.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c23a-155">关系</span><span class="sxs-lookup"><span data-stu-id="1c23a-155">Relationships</span></span>
|<span data-ttu-id="1c23a-156">关系</span><span class="sxs-lookup"><span data-stu-id="1c23a-156">Relationship</span></span>|<span data-ttu-id="1c23a-157">类型</span><span class="sxs-lookup"><span data-stu-id="1c23a-157">Type</span></span>|<span data-ttu-id="1c23a-158">说明</span><span class="sxs-lookup"><span data-stu-id="1c23a-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c23a-159">children</span><span class="sxs-lookup"><span data-stu-id="1c23a-159">children</span></span>|<span data-ttu-id="1c23a-160">[Microsoft termStore](../resources/termstore-term.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c23a-160">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="1c23a-161">术语[库]中设置的子术语。</span><span class="sxs-lookup"><span data-stu-id="1c23a-161">Children terms of set in term [store].</span></span>|
|<span data-ttu-id="1c23a-162">parentGroup</span><span class="sxs-lookup"><span data-stu-id="1c23a-162">parentGroup</span></span>|[<span data-ttu-id="1c23a-163">termStore 的组</span><span class="sxs-lookup"><span data-stu-id="1c23a-163">microsoft.graph.termStore.group</span></span>](../resources/termstore-group.md)|<span data-ttu-id="1c23a-164">包含集的父[组]。</span><span class="sxs-lookup"><span data-stu-id="1c23a-164">The parent [group] that contains the set.</span></span>|
|<span data-ttu-id="1c23a-165">公关</span><span class="sxs-lookup"><span data-stu-id="1c23a-165">relations</span></span>|<span data-ttu-id="1c23a-166">[termStore](../resources/termstore-relation.md)集合的关系</span><span class="sxs-lookup"><span data-stu-id="1c23a-166">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="1c23a-167">指示已固定或直接在集合下重复使用的术语。</span><span class="sxs-lookup"><span data-stu-id="1c23a-167">Indicates which terms have been pinned or reused directly under the set.</span></span>|
|<span data-ttu-id="1c23a-168">而言</span><span class="sxs-lookup"><span data-stu-id="1c23a-168">terms</span></span>|<span data-ttu-id="1c23a-169">[Microsoft termStore](../resources/termstore-term.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c23a-169">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="1c23a-170">该集下的所有条件。</span><span class="sxs-lookup"><span data-stu-id="1c23a-170">All the terms under the set.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c23a-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c23a-171">JSON representation</span></span>
<span data-ttu-id="1c23a-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c23a-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[termStore 设置]: termstore-set.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[microsoft]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[组]: ../resources/termstore-group.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[术语]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set": "#"
  },
  "suppressions": []
}
-->
