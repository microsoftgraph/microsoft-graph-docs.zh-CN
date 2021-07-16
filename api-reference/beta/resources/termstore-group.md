---
author: mohitpcad
title: 组资源类型
doc_type: resourcePageType
description: 表示在术语库中使用的组。
localization_priority: Normal
ms.prod: taxonomy
ms.openlocfilehash: ec2e9609b2de278d2596d42b18cae2fe450efd86
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456357"
---
# <a name="group-resource-type"></a><span data-ttu-id="a6a96-103">组资源类型</span><span class="sxs-lookup"><span data-stu-id="a6a96-103">Group resource type</span></span>

<span data-ttu-id="a6a96-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="a6a96-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="a6a96-105">表示在术语库中使用的 [组](../resources/termstore-store.md)。</span><span class="sxs-lookup"><span data-stu-id="a6a96-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="a6a96-106">组是逻辑层次结构，其中包含其下的集合。</span><span class="sxs-lookup"><span data-stu-id="a6a96-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="a6a96-107">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="a6a96-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="a6a96-108">方法</span><span class="sxs-lookup"><span data-stu-id="a6a96-108">Methods</span></span>

| <span data-ttu-id="a6a96-109">方法</span><span class="sxs-lookup"><span data-stu-id="a6a96-109">Method</span></span>                                                   | <span data-ttu-id="a6a96-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6a96-110">Return type</span></span>       |    <span data-ttu-id="a6a96-111">说明</span><span class="sxs-lookup"><span data-stu-id="a6a96-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="a6a96-112">创建组</span><span class="sxs-lookup"><span data-stu-id="a6a96-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="a6a96-113">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="a6a96-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="a6a96-114">在术语库创建 [组]。</span><span class="sxs-lookup"><span data-stu-id="a6a96-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="a6a96-115">Get group</span><span class="sxs-lookup"><span data-stu-id="a6a96-115">Get group</span></span>](../api/termstore-group-get.md)                           | <span data-ttu-id="a6a96-116">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="a6a96-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="a6a96-117">检索术语库中的组 [数据]。</span><span class="sxs-lookup"><span data-stu-id="a6a96-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="a6a96-118">删除组</span><span class="sxs-lookup"><span data-stu-id="a6a96-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="a6a96-119">无</span><span class="sxs-lookup"><span data-stu-id="a6a96-119">None</span></span> |  <span data-ttu-id="a6a96-120">删除术语库中的 [组]。</span><span class="sxs-lookup"><span data-stu-id="a6a96-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="a6a96-121">属性</span><span class="sxs-lookup"><span data-stu-id="a6a96-121">Properties</span></span>

| <span data-ttu-id="a6a96-122">属性</span><span class="sxs-lookup"><span data-stu-id="a6a96-122">Property</span></span>             | <span data-ttu-id="a6a96-123">类型</span><span class="sxs-lookup"><span data-stu-id="a6a96-123">Type</span></span>               | <span data-ttu-id="a6a96-124">说明</span><span class="sxs-lookup"><span data-stu-id="a6a96-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="a6a96-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a96-125">createdDateTime</span></span>      | <span data-ttu-id="a6a96-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a96-126">DateTimeOffset</span></span>     | <span data-ttu-id="a6a96-127">组创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a6a96-127">Date and time of group creation.</span></span> <span data-ttu-id="a6a96-128">只读。</span><span class="sxs-lookup"><span data-stu-id="a6a96-128">Read-only.</span></span>
| <span data-ttu-id="a6a96-129">说明</span><span class="sxs-lookup"><span data-stu-id="a6a96-129">description</span></span>          | <span data-ttu-id="a6a96-130">string</span><span class="sxs-lookup"><span data-stu-id="a6a96-130">string</span></span>             | <span data-ttu-id="a6a96-131">提供有关术语用法的详细信息的说明。</span><span class="sxs-lookup"><span data-stu-id="a6a96-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="a6a96-132">id</span><span class="sxs-lookup"><span data-stu-id="a6a96-132">id</span></span>                   | <span data-ttu-id="a6a96-133">string</span><span class="sxs-lookup"><span data-stu-id="a6a96-133">string</span></span>             | <span data-ttu-id="a6a96-134">组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a6a96-134">Unique identifier of group.</span></span> <span data-ttu-id="a6a96-135">只读。</span><span class="sxs-lookup"><span data-stu-id="a6a96-135">Read-Only.</span></span>
| <span data-ttu-id="a6a96-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a6a96-136">displayName</span></span>          | <span data-ttu-id="a6a96-137">string</span><span class="sxs-lookup"><span data-stu-id="a6a96-137">string</span></span>             | <span data-ttu-id="a6a96-138">组的名称。</span><span class="sxs-lookup"><span data-stu-id="a6a96-138">Name of group.</span></span>
| <span data-ttu-id="a6a96-139">scope</span><span class="sxs-lookup"><span data-stu-id="a6a96-139">scope</span></span>                | <span data-ttu-id="a6a96-140">string</span><span class="sxs-lookup"><span data-stu-id="a6a96-140">string</span></span>              | <span data-ttu-id="a6a96-141">返回组的类型。</span><span class="sxs-lookup"><span data-stu-id="a6a96-141">Returns type of group.</span></span> <span data-ttu-id="a6a96-142">可能的值是"global"、"system"和"siteCollection"。</span><span class="sxs-lookup"><span data-stu-id="a6a96-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>
| <span data-ttu-id="a6a96-143">parentSiteId</span><span class="sxs-lookup"><span data-stu-id="a6a96-143">parentSiteId</span></span>         | <span data-ttu-id="a6a96-144">string</span><span class="sxs-lookup"><span data-stu-id="a6a96-144">string</span></span>             | <span data-ttu-id="a6a96-145">此组的父网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="a6a96-145">Id of the parent site of this group.</span></span>

## <a name="relationships"></a><span data-ttu-id="a6a96-146">关系</span><span class="sxs-lookup"><span data-stu-id="a6a96-146">Relationships</span></span>
| <span data-ttu-id="a6a96-147">关系</span><span class="sxs-lookup"><span data-stu-id="a6a96-147">Relationship</span></span>       | <span data-ttu-id="a6a96-148">类型</span><span class="sxs-lookup"><span data-stu-id="a6a96-148">Type</span></span>                        | <span data-ttu-id="a6a96-149">说明</span><span class="sxs-lookup"><span data-stu-id="a6a96-149">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="a6a96-150">sets</span><span class="sxs-lookup"><span data-stu-id="a6a96-150">sets</span></span>           | <span data-ttu-id="a6a96-151">[microsoft.graph.termStore.set][] 集合</span><span class="sxs-lookup"><span data-stu-id="a6a96-151">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="a6a96-152">术语库 中的组下的所有 [集]。</span><span class="sxs-lookup"><span data-stu-id="a6a96-152">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6a96-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6a96-153">JSON representation</span></span>

<span data-ttu-id="a6a96-154">下面是组资源的 JSON **表示** 形式。</span><span class="sxs-lookup"><span data-stu-id="a6a96-154">The following is a JSON representation of a **group** resource.</span></span>
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
    "Resources/termStore.group&quot;: &quot;#"
  },
  "suppressions": []
}
-->


