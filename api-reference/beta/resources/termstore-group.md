---
author: mohitpcad
title: 组资源类型
doc_type: resourcePageType
description: 表示在术语库中使用的组。
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: 1249f94b96e0c6ff7251a2a97f4885a21258aaeb
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473463"
---
# <a name="group-resource-type"></a><span data-ttu-id="b970b-103">组资源类型</span><span class="sxs-lookup"><span data-stu-id="b970b-103">Group resource type</span></span>

<span data-ttu-id="b970b-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="b970b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="b970b-105">表示在术语库中使用的 [组](../resources/termstore-store.md)。</span><span class="sxs-lookup"><span data-stu-id="b970b-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="b970b-106">组是逻辑层次结构，其中包含其下的集合。</span><span class="sxs-lookup"><span data-stu-id="b970b-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="b970b-107">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="b970b-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="b970b-108">方法</span><span class="sxs-lookup"><span data-stu-id="b970b-108">Methods</span></span>

| <span data-ttu-id="b970b-109">方法</span><span class="sxs-lookup"><span data-stu-id="b970b-109">Method</span></span>                                                   | <span data-ttu-id="b970b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b970b-110">Return type</span></span>       |    <span data-ttu-id="b970b-111">说明</span><span class="sxs-lookup"><span data-stu-id="b970b-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="b970b-112">创建组</span><span class="sxs-lookup"><span data-stu-id="b970b-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="b970b-113">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="b970b-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="b970b-114">在术语库创建 [组]。</span><span class="sxs-lookup"><span data-stu-id="b970b-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="b970b-115">Get group</span><span class="sxs-lookup"><span data-stu-id="b970b-115">Get group</span></span>](../api/termstore-store-get-group.md)                           | <span data-ttu-id="b970b-116">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="b970b-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="b970b-117">检索术语库中的组 [数据]。</span><span class="sxs-lookup"><span data-stu-id="b970b-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="b970b-118">删除组</span><span class="sxs-lookup"><span data-stu-id="b970b-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="b970b-119">无</span><span class="sxs-lookup"><span data-stu-id="b970b-119">None</span></span> |  <span data-ttu-id="b970b-120">删除术语库中的 [组]。</span><span class="sxs-lookup"><span data-stu-id="b970b-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="b970b-121">属性</span><span class="sxs-lookup"><span data-stu-id="b970b-121">Properties</span></span>

| <span data-ttu-id="b970b-122">属性</span><span class="sxs-lookup"><span data-stu-id="b970b-122">Property</span></span>             | <span data-ttu-id="b970b-123">类型</span><span class="sxs-lookup"><span data-stu-id="b970b-123">Type</span></span>               | <span data-ttu-id="b970b-124">说明</span><span class="sxs-lookup"><span data-stu-id="b970b-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="b970b-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b970b-125">createdDateTime</span></span>      | <span data-ttu-id="b970b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b970b-126">DateTimeOffset</span></span>     | <span data-ttu-id="b970b-127">组创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b970b-127">Date and time of group creation.</span></span> <span data-ttu-id="b970b-128">只读。</span><span class="sxs-lookup"><span data-stu-id="b970b-128">Read-only.</span></span>
| <span data-ttu-id="b970b-129">说明</span><span class="sxs-lookup"><span data-stu-id="b970b-129">description</span></span>          | <span data-ttu-id="b970b-130">string</span><span class="sxs-lookup"><span data-stu-id="b970b-130">string</span></span>             | <span data-ttu-id="b970b-131">提供有关术语用法的详细信息的说明。</span><span class="sxs-lookup"><span data-stu-id="b970b-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="b970b-132">id</span><span class="sxs-lookup"><span data-stu-id="b970b-132">id</span></span>                   | <span data-ttu-id="b970b-133">string</span><span class="sxs-lookup"><span data-stu-id="b970b-133">string</span></span>             | <span data-ttu-id="b970b-134">组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b970b-134">Unique identifier of group.</span></span> <span data-ttu-id="b970b-135">只读。</span><span class="sxs-lookup"><span data-stu-id="b970b-135">Read-Only.</span></span>
| <span data-ttu-id="b970b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b970b-136">displayName</span></span>          | <span data-ttu-id="b970b-137">string</span><span class="sxs-lookup"><span data-stu-id="b970b-137">string</span></span>             | <span data-ttu-id="b970b-138">组的名称。</span><span class="sxs-lookup"><span data-stu-id="b970b-138">Name of group.</span></span>
| <span data-ttu-id="b970b-139">scope</span><span class="sxs-lookup"><span data-stu-id="b970b-139">scope</span></span>                | <span data-ttu-id="b970b-140">string</span><span class="sxs-lookup"><span data-stu-id="b970b-140">string</span></span>              | <span data-ttu-id="b970b-141">返回组的类型。</span><span class="sxs-lookup"><span data-stu-id="b970b-141">Returns type of group.</span></span> <span data-ttu-id="b970b-142">可能的值是"global"、"system"和"siteCollection"。</span><span class="sxs-lookup"><span data-stu-id="b970b-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>
| <span data-ttu-id="b970b-143">parentSiteId</span><span class="sxs-lookup"><span data-stu-id="b970b-143">parentSiteId</span></span>         | <span data-ttu-id="b970b-144">string</span><span class="sxs-lookup"><span data-stu-id="b970b-144">string</span></span>             | <span data-ttu-id="b970b-145">此组的父网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="b970b-145">Id of the parent site of this group.</span></span>

## <a name="relationships"></a><span data-ttu-id="b970b-146">关系</span><span class="sxs-lookup"><span data-stu-id="b970b-146">Relationships</span></span>
| <span data-ttu-id="b970b-147">关系</span><span class="sxs-lookup"><span data-stu-id="b970b-147">Relationship</span></span>       | <span data-ttu-id="b970b-148">类型</span><span class="sxs-lookup"><span data-stu-id="b970b-148">Type</span></span>                        | <span data-ttu-id="b970b-149">说明</span><span class="sxs-lookup"><span data-stu-id="b970b-149">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="b970b-150">sets</span><span class="sxs-lookup"><span data-stu-id="b970b-150">sets</span></span>           | <span data-ttu-id="b970b-151">[microsoft.graph.termStore.set][] 集合</span><span class="sxs-lookup"><span data-stu-id="b970b-151">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="b970b-152">术语库 中的组下的所有 [集]。</span><span class="sxs-lookup"><span data-stu-id="b970b-152">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="b970b-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b970b-153">JSON representation</span></span>

<span data-ttu-id="b970b-154">下面是组资源的 JSON **表示** 形式。</span><span class="sxs-lookup"><span data-stu-id="b970b-154">The following is a JSON representation of a **group** resource.</span></span>
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
  "displayName": "string",
  "parentSiteId" : "string"
}
```



[identitySet]: identitySet.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
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


