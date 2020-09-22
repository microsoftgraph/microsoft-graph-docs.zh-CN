---
title: 术语资源类型
description: 定义术语库中的术语实体。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 831a873d245424bcb92c7281b1bbdc97b29223bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075558"
---
# <a name="term-resource-type"></a><span data-ttu-id="a7fec-103">术语资源类型</span><span class="sxs-lookup"><span data-stu-id="a7fec-103">term resource type</span></span>

<span data-ttu-id="a7fec-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="a7fec-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7fec-105">代表术语 [库]中使用的术语。</span><span class="sxs-lookup"><span data-stu-id="a7fec-105">Represents a term used in a term [store].</span></span> <span data-ttu-id="a7fec-106">术语可用于表示一个对象，该对象随后可用作标记 conent 的元数据。</span><span class="sxs-lookup"><span data-stu-id="a7fec-106">A term can be used to represent an object which can then be used as a metadata to tag conent.</span></span> <span data-ttu-id="a7fec-107">可以在 [集合]中以分层方式组织多个术语。</span><span class="sxs-lookup"><span data-stu-id="a7fec-107">Multiple terms can be organized in a hierarchical manner within a [set].</span></span>

<span data-ttu-id="a7fec-108">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="a7fec-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a7fec-109">方法</span><span class="sxs-lookup"><span data-stu-id="a7fec-109">Methods</span></span>
|<span data-ttu-id="a7fec-110">方法</span><span class="sxs-lookup"><span data-stu-id="a7fec-110">Method</span></span>|<span data-ttu-id="a7fec-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7fec-111">Return type</span></span>|<span data-ttu-id="a7fec-112">说明</span><span class="sxs-lookup"><span data-stu-id="a7fec-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7fec-113">列出子项</span><span class="sxs-lookup"><span data-stu-id="a7fec-113">List children</span></span>](../api/termstore-term-list-children.md)|<span data-ttu-id="a7fec-114">[Microsoft termStore](../resources/termstore-term.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7fec-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="a7fec-115">在术语 [库]中获取术语的第一级子级。</span><span class="sxs-lookup"><span data-stu-id="a7fec-115">Get the first level children of a term in a term [store].</span></span>|
|[<span data-ttu-id="a7fec-116">列表关系</span><span class="sxs-lookup"><span data-stu-id="a7fec-116">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="a7fec-117">[termStore](../resources/termstore-relation.md) 集合的关系</span><span class="sxs-lookup"><span data-stu-id="a7fec-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="a7fec-118">获取术语 [库]中术语的关系。</span><span class="sxs-lookup"><span data-stu-id="a7fec-118">Get the relations of a term in a term [store].</span></span>|
|[<span data-ttu-id="a7fec-119">创建关系</span><span class="sxs-lookup"><span data-stu-id="a7fec-119">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="a7fec-120">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="a7fec-120">microsoft.graph.termStore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="a7fec-121">为术语[库]中的术语或[集]创建新的关系。</span><span class="sxs-lookup"><span data-stu-id="a7fec-121">Create a new relation for a term or a [set] in a term [store].</span></span>|
|[<span data-ttu-id="a7fec-122">创建术语</span><span class="sxs-lookup"><span data-stu-id="a7fec-122">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="a7fec-123">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="a7fec-123">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="a7fec-124">在术语 [库]中创建新的术语对象。</span><span class="sxs-lookup"><span data-stu-id="a7fec-124">Create a new term object in a term [store].</span></span>|
|[<span data-ttu-id="a7fec-125">获取术语</span><span class="sxs-lookup"><span data-stu-id="a7fec-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="a7fec-126">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="a7fec-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="a7fec-127">读取术语  [库]中术语对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7fec-127">Read the properties and relationships of a term object in a term  [store].</span></span>|
|[<span data-ttu-id="a7fec-128">更新术语</span><span class="sxs-lookup"><span data-stu-id="a7fec-128">Update term</span></span>](../api/termstore-term-update.md)|[<span data-ttu-id="a7fec-129">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="a7fec-129">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="a7fec-130">更新术语 [库]中术语对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7fec-130">Update the properties of a term object in a term [store].</span></span>|
|[<span data-ttu-id="a7fec-131">删除术语</span><span class="sxs-lookup"><span data-stu-id="a7fec-131">Delete term</span></span>](../api/termstore-term-delete.md)|<span data-ttu-id="a7fec-132">无</span><span class="sxs-lookup"><span data-stu-id="a7fec-132">None</span></span>|<span data-ttu-id="a7fec-133">删除术语 [库]中的术语对象。</span><span class="sxs-lookup"><span data-stu-id="a7fec-133">Delete a term object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="a7fec-134">属性</span><span class="sxs-lookup"><span data-stu-id="a7fec-134">Properties</span></span>
|<span data-ttu-id="a7fec-135">属性</span><span class="sxs-lookup"><span data-stu-id="a7fec-135">Property</span></span>|<span data-ttu-id="a7fec-136">类型</span><span class="sxs-lookup"><span data-stu-id="a7fec-136">Type</span></span>|<span data-ttu-id="a7fec-137">说明</span><span class="sxs-lookup"><span data-stu-id="a7fec-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7fec-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7fec-138">createdDateTime</span></span>|<span data-ttu-id="a7fec-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7fec-139">DateTimeOffset</span></span>|<span data-ttu-id="a7fec-140">创建术语的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a7fec-140">Date and time of term creation.</span></span> <span data-ttu-id="a7fec-141">只读</span><span class="sxs-lookup"><span data-stu-id="a7fec-141">Read-only</span></span>|
|<span data-ttu-id="a7fec-142">说明</span><span class="sxs-lookup"><span data-stu-id="a7fec-142">descriptions</span></span>|<span data-ttu-id="a7fec-143">[termStore](../resources/termstore-localizeddescription.md) 集合的 localizedDescription</span><span class="sxs-lookup"><span data-stu-id="a7fec-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="a7fec-144">依赖于 languageTag 的术语的说明</span><span class="sxs-lookup"><span data-stu-id="a7fec-144">Description about term that is dependent on the languageTag</span></span>|
|<span data-ttu-id="a7fec-145">id</span><span class="sxs-lookup"><span data-stu-id="a7fec-145">id</span></span>|<span data-ttu-id="a7fec-146">String</span><span class="sxs-lookup"><span data-stu-id="a7fec-146">String</span></span>|<span data-ttu-id="a7fec-147">术语的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a7fec-147">Unique identifier of term.</span></span> <span data-ttu-id="a7fec-148">只读</span><span class="sxs-lookup"><span data-stu-id="a7fec-148">Read-Only</span></span>|
|<span data-ttu-id="a7fec-149">标题</span><span class="sxs-lookup"><span data-stu-id="a7fec-149">labels</span></span>|<span data-ttu-id="a7fec-150">[termStore](../resources/termstore-localizedlabel.md) 集合的 localizedLabel</span><span class="sxs-lookup"><span data-stu-id="a7fec-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>||<span data-ttu-id="a7fec-151">术语的标签元数据</span><span class="sxs-lookup"><span data-stu-id="a7fec-151">Label metadata for a term</span></span>|
|<span data-ttu-id="a7fec-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7fec-152">lastModifiedDateTime</span></span>|<span data-ttu-id="a7fec-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7fec-153">DateTimeOffset</span></span>|<span data-ttu-id="a7fec-154">上次修改术语的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a7fec-154">Last date and time of term modification.</span></span> <span data-ttu-id="a7fec-155">只读</span><span class="sxs-lookup"><span data-stu-id="a7fec-155">Read-only</span></span>|
|<span data-ttu-id="a7fec-156">properties</span><span class="sxs-lookup"><span data-stu-id="a7fec-156">properties</span></span>|<span data-ttu-id="a7fec-157">[键值](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7fec-157">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="a7fec-158">术语的属性集合</span><span class="sxs-lookup"><span data-stu-id="a7fec-158">Collection of properties on the term</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7fec-159">关系</span><span class="sxs-lookup"><span data-stu-id="a7fec-159">Relationships</span></span>
|<span data-ttu-id="a7fec-160">关系</span><span class="sxs-lookup"><span data-stu-id="a7fec-160">Relationship</span></span>|<span data-ttu-id="a7fec-161">类型</span><span class="sxs-lookup"><span data-stu-id="a7fec-161">Type</span></span>|<span data-ttu-id="a7fec-162">说明</span><span class="sxs-lookup"><span data-stu-id="a7fec-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7fec-163">children</span><span class="sxs-lookup"><span data-stu-id="a7fec-163">children</span></span>|<span data-ttu-id="a7fec-164">[Microsoft termStore](../resources/termstore-term.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7fec-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="a7fec-165">当前术语的子项</span><span class="sxs-lookup"><span data-stu-id="a7fec-165">Children of current term</span></span>|
|<span data-ttu-id="a7fec-166">公关</span><span class="sxs-lookup"><span data-stu-id="a7fec-166">relations</span></span>|<span data-ttu-id="a7fec-167">[termStore](../resources/termstore-relation.md) 集合的关系</span><span class="sxs-lookup"><span data-stu-id="a7fec-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="a7fec-168">指示与当前术语相关的术语，无论是固定的还是重用的</span><span class="sxs-lookup"><span data-stu-id="a7fec-168">To indicate which terms are related to the current term as either pinned or reused</span></span>|
|<span data-ttu-id="a7fec-169">set</span><span class="sxs-lookup"><span data-stu-id="a7fec-169">set</span></span>|[<span data-ttu-id="a7fec-170">termStore 设置</span><span class="sxs-lookup"><span data-stu-id="a7fec-170">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="a7fec-171">在其中创建术语的[集]</span><span class="sxs-lookup"><span data-stu-id="a7fec-171">The [set] in which the term is created</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a7fec-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7fec-172">JSON representation</span></span>
<span data-ttu-id="a7fec-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7fec-173">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.term",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.term",
  "id": "String (identifier)",
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```

[商店]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md
[group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Term is the entity used for tagging in termStore",
  "keywords": "term,facet,resource",
  "section": "documentation",
  "tocPath": "Terms",
  "tocBookmarks": {
    "Resources/termstore-term": "#"
  },
  "suppressions": []
}
-->


