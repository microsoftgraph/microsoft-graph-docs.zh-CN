---
title: 术语资源类型
description: 定义术语库中的术语实体。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71c22c86d2ebbb02587a20355adb1d461479297d
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273571"
---
# <a name="term-resource-type"></a><span data-ttu-id="e2dc8-103">术语资源类型</span><span class="sxs-lookup"><span data-stu-id="e2dc8-103">term resource type</span></span>

<span data-ttu-id="e2dc8-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="e2dc8-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2dc8-105">代表术语 [库]中使用的术语。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-105">Represents a term used in a term [store].</span></span> <span data-ttu-id="e2dc8-106">术语可用于表示可用作标记内容的元数据的对象。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-106">A term can be used to represent an object which can then be used as a metadata to tag content.</span></span> <span data-ttu-id="e2dc8-107">可以在 [集合]中以分层方式组织多个术语。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-107">Multiple terms can be organized in a hierarchical manner within a [set].</span></span>

<span data-ttu-id="e2dc8-108">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e2dc8-109">Methods</span><span class="sxs-lookup"><span data-stu-id="e2dc8-109">Methods</span></span>
|<span data-ttu-id="e2dc8-110">方法</span><span class="sxs-lookup"><span data-stu-id="e2dc8-110">Method</span></span>|<span data-ttu-id="e2dc8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2dc8-111">Return type</span></span>|<span data-ttu-id="e2dc8-112">说明</span><span class="sxs-lookup"><span data-stu-id="e2dc8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2dc8-113">列出子项</span><span class="sxs-lookup"><span data-stu-id="e2dc8-113">List children</span></span>](../api/termstore-term-list-children.md)|<span data-ttu-id="e2dc8-114">[Microsoft termStore](../resources/termstore-term.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2dc8-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="e2dc8-115">在术语 [库]中获取术语的第一级子级。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-115">Get the first level children of a term in a term [store].</span></span>|
|[<span data-ttu-id="e2dc8-116">列表关系</span><span class="sxs-lookup"><span data-stu-id="e2dc8-116">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="e2dc8-117">[termStore](../resources/termstore-relation.md) 集合的关系</span><span class="sxs-lookup"><span data-stu-id="e2dc8-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="e2dc8-118">获取术语 [库]中术语的关系。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-118">Get the relations of a term in a term [store].</span></span>|
|[<span data-ttu-id="e2dc8-119">创建关系</span><span class="sxs-lookup"><span data-stu-id="e2dc8-119">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="e2dc8-120">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="e2dc8-120">microsoft.graph.termStore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="e2dc8-121">为术语[库]中的术语或[集]创建新的关系。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-121">Create a new relation for a term or a [set] in a term [store].</span></span>|
|[<span data-ttu-id="e2dc8-122">创建术语</span><span class="sxs-lookup"><span data-stu-id="e2dc8-122">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="e2dc8-123">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="e2dc8-123">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="e2dc8-124">在术语 [库]中创建新的术语对象。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-124">Create a new term object in a term [store].</span></span>|
|[<span data-ttu-id="e2dc8-125">获取术语</span><span class="sxs-lookup"><span data-stu-id="e2dc8-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="e2dc8-126">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="e2dc8-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="e2dc8-127">读取术语  [库]中术语对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-127">Read the properties and relationships of a term object in a term  [store].</span></span>|
|[<span data-ttu-id="e2dc8-128">更新术语</span><span class="sxs-lookup"><span data-stu-id="e2dc8-128">Update term</span></span>](../api/termstore-term-update.md)|[<span data-ttu-id="e2dc8-129">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="e2dc8-129">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="e2dc8-130">更新术语 [库]中术语对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-130">Update the properties of a term object in a term [store].</span></span>|
|[<span data-ttu-id="e2dc8-131">删除术语</span><span class="sxs-lookup"><span data-stu-id="e2dc8-131">Delete term</span></span>](../api/termstore-term-delete.md)|<span data-ttu-id="e2dc8-132">无</span><span class="sxs-lookup"><span data-stu-id="e2dc8-132">None</span></span>|<span data-ttu-id="e2dc8-133">删除术语 [库]中的术语对象。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-133">Delete a term object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="e2dc8-134">属性</span><span class="sxs-lookup"><span data-stu-id="e2dc8-134">Properties</span></span>
|<span data-ttu-id="e2dc8-135">属性</span><span class="sxs-lookup"><span data-stu-id="e2dc8-135">Property</span></span>|<span data-ttu-id="e2dc8-136">类型</span><span class="sxs-lookup"><span data-stu-id="e2dc8-136">Type</span></span>|<span data-ttu-id="e2dc8-137">说明</span><span class="sxs-lookup"><span data-stu-id="e2dc8-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2dc8-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2dc8-138">createdDateTime</span></span>|<span data-ttu-id="e2dc8-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2dc8-139">DateTimeOffset</span></span>|<span data-ttu-id="e2dc8-140">创建术语的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-140">Date and time of term creation.</span></span> <span data-ttu-id="e2dc8-141">只读</span><span class="sxs-lookup"><span data-stu-id="e2dc8-141">Read-only</span></span>|
|<span data-ttu-id="e2dc8-142">说明</span><span class="sxs-lookup"><span data-stu-id="e2dc8-142">descriptions</span></span>|<span data-ttu-id="e2dc8-143">[termStore](../resources/termstore-localizeddescription.md) 集合的 localizedDescription</span><span class="sxs-lookup"><span data-stu-id="e2dc8-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="e2dc8-144">依赖于 languageTag 的术语的说明</span><span class="sxs-lookup"><span data-stu-id="e2dc8-144">Description about term that is dependent on the languageTag</span></span>|
|<span data-ttu-id="e2dc8-145">id</span><span class="sxs-lookup"><span data-stu-id="e2dc8-145">id</span></span>|<span data-ttu-id="e2dc8-146">字符串</span><span class="sxs-lookup"><span data-stu-id="e2dc8-146">String</span></span>|<span data-ttu-id="e2dc8-147">术语的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-147">Unique identifier of term.</span></span> <span data-ttu-id="e2dc8-148">只读</span><span class="sxs-lookup"><span data-stu-id="e2dc8-148">Read-Only</span></span>|
|<span data-ttu-id="e2dc8-149">标题</span><span class="sxs-lookup"><span data-stu-id="e2dc8-149">labels</span></span>|<span data-ttu-id="e2dc8-150">[termStore](../resources/termstore-localizedlabel.md) 集合的 localizedLabel</span><span class="sxs-lookup"><span data-stu-id="e2dc8-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>||<span data-ttu-id="e2dc8-151">术语的标签元数据</span><span class="sxs-lookup"><span data-stu-id="e2dc8-151">Label metadata for a term</span></span>|
|<span data-ttu-id="e2dc8-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2dc8-152">lastModifiedDateTime</span></span>|<span data-ttu-id="e2dc8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2dc8-153">DateTimeOffset</span></span>|<span data-ttu-id="e2dc8-154">上次修改术语的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-154">Last date and time of term modification.</span></span> <span data-ttu-id="e2dc8-155">只读</span><span class="sxs-lookup"><span data-stu-id="e2dc8-155">Read-only</span></span>|
|<span data-ttu-id="e2dc8-156">properties</span><span class="sxs-lookup"><span data-stu-id="e2dc8-156">properties</span></span>|<span data-ttu-id="e2dc8-157">[键值](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2dc8-157">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="e2dc8-158">术语的属性集合</span><span class="sxs-lookup"><span data-stu-id="e2dc8-158">Collection of properties on the term</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2dc8-159">关系</span><span class="sxs-lookup"><span data-stu-id="e2dc8-159">Relationships</span></span>
|<span data-ttu-id="e2dc8-160">关系</span><span class="sxs-lookup"><span data-stu-id="e2dc8-160">Relationship</span></span>|<span data-ttu-id="e2dc8-161">类型</span><span class="sxs-lookup"><span data-stu-id="e2dc8-161">Type</span></span>|<span data-ttu-id="e2dc8-162">说明</span><span class="sxs-lookup"><span data-stu-id="e2dc8-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2dc8-163">children</span><span class="sxs-lookup"><span data-stu-id="e2dc8-163">children</span></span>|<span data-ttu-id="e2dc8-164">[Microsoft termStore](../resources/termstore-term.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2dc8-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="e2dc8-165">当前术语的子项</span><span class="sxs-lookup"><span data-stu-id="e2dc8-165">Children of current term</span></span>|
|<span data-ttu-id="e2dc8-166">公关</span><span class="sxs-lookup"><span data-stu-id="e2dc8-166">relations</span></span>|<span data-ttu-id="e2dc8-167">[termStore](../resources/termstore-relation.md) 集合的关系</span><span class="sxs-lookup"><span data-stu-id="e2dc8-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="e2dc8-168">指示与当前术语相关的术语，无论是固定的还是重用的</span><span class="sxs-lookup"><span data-stu-id="e2dc8-168">To indicate which terms are related to the current term as either pinned or reused</span></span>|
|<span data-ttu-id="e2dc8-169">set</span><span class="sxs-lookup"><span data-stu-id="e2dc8-169">set</span></span>|[<span data-ttu-id="e2dc8-170">termStore 设置</span><span class="sxs-lookup"><span data-stu-id="e2dc8-170">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="e2dc8-171">在其中创建术语的[集]</span><span class="sxs-lookup"><span data-stu-id="e2dc8-171">The [set] in which the term is created</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2dc8-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2dc8-172">JSON representation</span></span>
<span data-ttu-id="e2dc8-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2dc8-173">The following is a JSON representation of the resource.</span></span>
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

[microsoft]: ../resources/termstore-store.md
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


