---
title: 术语资源类型
description: 定义术语存储中的术语实体。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5645b85a5d017fd05010e04e118853a904a78b6c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516176"
---
# <a name="term-resource-type"></a><span data-ttu-id="66f6f-103">术语资源类型</span><span class="sxs-lookup"><span data-stu-id="66f6f-103">term resource type</span></span>

<span data-ttu-id="66f6f-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="66f6f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66f6f-105">表示术语库中使用的 [术语]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-105">Represents a term used in a term [store].</span></span> <span data-ttu-id="66f6f-106">术语可用于表示一个对象，然后该对象可用作标记内容的元数据。</span><span class="sxs-lookup"><span data-stu-id="66f6f-106">A term can be used to represent an object which can then be used as a metadata to tag content.</span></span> <span data-ttu-id="66f6f-107">多个术语可以在一组内以分层方式 [组织]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-107">Multiple terms can be organized in a hierarchical manner within a [set].</span></span>

<span data-ttu-id="66f6f-108">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="66f6f-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="66f6f-109">方法</span><span class="sxs-lookup"><span data-stu-id="66f6f-109">Methods</span></span>
|<span data-ttu-id="66f6f-110">方法</span><span class="sxs-lookup"><span data-stu-id="66f6f-110">Method</span></span>|<span data-ttu-id="66f6f-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="66f6f-111">Return type</span></span>|<span data-ttu-id="66f6f-112">说明</span><span class="sxs-lookup"><span data-stu-id="66f6f-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66f6f-113">列出子项</span><span class="sxs-lookup"><span data-stu-id="66f6f-113">List children</span></span>](../api/termstore-term-list-children.md)|<span data-ttu-id="66f6f-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="66f6f-115">获取术语存储中术语的第一级 [子级]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-115">Get the first level children of a term in a term [store].</span></span>|
|[<span data-ttu-id="66f6f-116">列出关系</span><span class="sxs-lookup"><span data-stu-id="66f6f-116">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="66f6f-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="66f6f-118">获取术语存储中术语 [的关系]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-118">Get the relations of a term in a term [store].</span></span>|
|[<span data-ttu-id="66f6f-119">创建关系</span><span class="sxs-lookup"><span data-stu-id="66f6f-119">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="66f6f-120">microsoft.graph.termStore.relation</span><span class="sxs-lookup"><span data-stu-id="66f6f-120">microsoft.graph.termStore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="66f6f-121">在术语存储中为 [术语或集] 创建新 [关系]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-121">Create a new relation for a term or a [set] in a term [store].</span></span>|
|[<span data-ttu-id="66f6f-122">创建术语</span><span class="sxs-lookup"><span data-stu-id="66f6f-122">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="66f6f-123">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="66f6f-123">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="66f6f-124">在术语存储中创建新的术语 [对象]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-124">Create a new term object in a term [store].</span></span>|
|[<span data-ttu-id="66f6f-125">获取术语</span><span class="sxs-lookup"><span data-stu-id="66f6f-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="66f6f-126">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="66f6f-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="66f6f-127">读取术语存储中术语对象  [的属性和关系]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-127">Read the properties and relationships of a term object in a term  [store].</span></span>|
|[<span data-ttu-id="66f6f-128">更新术语</span><span class="sxs-lookup"><span data-stu-id="66f6f-128">Update term</span></span>](../api/termstore-term-update.md)|[<span data-ttu-id="66f6f-129">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="66f6f-129">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="66f6f-130">更新术语存储中术语对象 [的属性]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-130">Update the properties of a term object in a term [store].</span></span>|
|[<span data-ttu-id="66f6f-131">删除术语</span><span class="sxs-lookup"><span data-stu-id="66f6f-131">Delete term</span></span>](../api/termstore-term-delete.md)|<span data-ttu-id="66f6f-132">无</span><span class="sxs-lookup"><span data-stu-id="66f6f-132">None</span></span>|<span data-ttu-id="66f6f-133">删除术语存储中的术语 [对象]。</span><span class="sxs-lookup"><span data-stu-id="66f6f-133">Delete a term object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="66f6f-134">属性</span><span class="sxs-lookup"><span data-stu-id="66f6f-134">Properties</span></span>
|<span data-ttu-id="66f6f-135">属性</span><span class="sxs-lookup"><span data-stu-id="66f6f-135">Property</span></span>|<span data-ttu-id="66f6f-136">类型</span><span class="sxs-lookup"><span data-stu-id="66f6f-136">Type</span></span>|<span data-ttu-id="66f6f-137">说明</span><span class="sxs-lookup"><span data-stu-id="66f6f-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66f6f-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66f6f-138">createdDateTime</span></span>|<span data-ttu-id="66f6f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66f6f-139">DateTimeOffset</span></span>|<span data-ttu-id="66f6f-140">术语创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66f6f-140">Date and time of term creation.</span></span> <span data-ttu-id="66f6f-141">只读</span><span class="sxs-lookup"><span data-stu-id="66f6f-141">Read-only</span></span>|
|<span data-ttu-id="66f6f-142">说明</span><span class="sxs-lookup"><span data-stu-id="66f6f-142">descriptions</span></span>|<span data-ttu-id="66f6f-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="66f6f-144">有关依赖于 languageTag 的术语的说明</span><span class="sxs-lookup"><span data-stu-id="66f6f-144">Description about term that is dependent on the languageTag</span></span>|
|<span data-ttu-id="66f6f-145">id</span><span class="sxs-lookup"><span data-stu-id="66f6f-145">id</span></span>|<span data-ttu-id="66f6f-146">String</span><span class="sxs-lookup"><span data-stu-id="66f6f-146">String</span></span>|<span data-ttu-id="66f6f-147">术语的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="66f6f-147">Unique identifier of term.</span></span> <span data-ttu-id="66f6f-148">只读</span><span class="sxs-lookup"><span data-stu-id="66f6f-148">Read-Only</span></span>|
|<span data-ttu-id="66f6f-149">labels</span><span class="sxs-lookup"><span data-stu-id="66f6f-149">labels</span></span>|<span data-ttu-id="66f6f-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="66f6f-151">术语的标签元数据</span><span class="sxs-lookup"><span data-stu-id="66f6f-151">Label metadata for a term</span></span>|
|<span data-ttu-id="66f6f-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66f6f-152">lastModifiedDateTime</span></span>|<span data-ttu-id="66f6f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66f6f-153">DateTimeOffset</span></span>|<span data-ttu-id="66f6f-154">上次修改术语的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66f6f-154">Last date and time of term modification.</span></span> <span data-ttu-id="66f6f-155">只读</span><span class="sxs-lookup"><span data-stu-id="66f6f-155">Read-only</span></span>|
|<span data-ttu-id="66f6f-156">properties</span><span class="sxs-lookup"><span data-stu-id="66f6f-156">properties</span></span>|<span data-ttu-id="66f6f-157">[microsoft.graph.keyValue](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-157">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="66f6f-158">术语的属性集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-158">Collection of properties on the term</span></span>|

## <a name="relationships"></a><span data-ttu-id="66f6f-159">关系</span><span class="sxs-lookup"><span data-stu-id="66f6f-159">Relationships</span></span>
|<span data-ttu-id="66f6f-160">关系</span><span class="sxs-lookup"><span data-stu-id="66f6f-160">Relationship</span></span>|<span data-ttu-id="66f6f-161">类型</span><span class="sxs-lookup"><span data-stu-id="66f6f-161">Type</span></span>|<span data-ttu-id="66f6f-162">说明</span><span class="sxs-lookup"><span data-stu-id="66f6f-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66f6f-163">children</span><span class="sxs-lookup"><span data-stu-id="66f6f-163">children</span></span>|<span data-ttu-id="66f6f-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="66f6f-165">当前术语的子项</span><span class="sxs-lookup"><span data-stu-id="66f6f-165">Children of current term</span></span>|
|<span data-ttu-id="66f6f-166">relations</span><span class="sxs-lookup"><span data-stu-id="66f6f-166">relations</span></span>|<span data-ttu-id="66f6f-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66f6f-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="66f6f-168">指示与当前术语相关的术语（固定或重复使用）</span><span class="sxs-lookup"><span data-stu-id="66f6f-168">To indicate which terms are related to the current term as either pinned or reused</span></span>|
|<span data-ttu-id="66f6f-169">set</span><span class="sxs-lookup"><span data-stu-id="66f6f-169">set</span></span>|[<span data-ttu-id="66f6f-170">microsoft.graph.termStore.set</span><span class="sxs-lookup"><span data-stu-id="66f6f-170">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="66f6f-171">[创建]术语的集</span><span class="sxs-lookup"><span data-stu-id="66f6f-171">The [set] in which the term is created</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66f6f-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66f6f-172">JSON representation</span></span>
<span data-ttu-id="66f6f-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66f6f-173">The following is a JSON representation of the resource.</span></span>
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


