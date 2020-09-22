---
title: 存储资源类型
description: 表示分类术语库。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9a315cd9187528b07932710171376b7efcda7af9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988791"
---
# <a name="store-resource-type"></a><span data-ttu-id="e1d02-103">存储资源类型</span><span class="sxs-lookup"><span data-stu-id="e1d02-103">store resource type</span></span>

<span data-ttu-id="e1d02-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="e1d02-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d02-105">表示分类术语库。</span><span class="sxs-lookup"><span data-stu-id="e1d02-105">Represents a taxonomy term store.</span></span>

<span data-ttu-id="e1d02-106">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="e1d02-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e1d02-107">方法</span><span class="sxs-lookup"><span data-stu-id="e1d02-107">Methods</span></span>
|<span data-ttu-id="e1d02-108">方法</span><span class="sxs-lookup"><span data-stu-id="e1d02-108">Method</span></span>|<span data-ttu-id="e1d02-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e1d02-109">Return type</span></span>|<span data-ttu-id="e1d02-110">说明</span><span class="sxs-lookup"><span data-stu-id="e1d02-110">Description</span></span>
|:---|:---|:---
|[<span data-ttu-id="e1d02-111">List groups</span><span class="sxs-lookup"><span data-stu-id="e1d02-111">List groups</span></span>](../api/termstore-list-groups.md)|<span data-ttu-id="e1d02-112">[Microsoft termStore](../resources/termstore-group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1d02-112">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span>| <span data-ttu-id="e1d02-113">将组从术语库对象中的提供中获取。</span><span class="sxs-lookup"><span data-stu-id="e1d02-113">Get the groups from available in the term store object.</span></span>|
|[<span data-ttu-id="e1d02-114">获取存储区</span><span class="sxs-lookup"><span data-stu-id="e1d02-114">Get store</span></span>](../api/termstore-store-get.md) | [<span data-ttu-id="e1d02-115">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="e1d02-115">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="e1d02-116">读取术语库对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e1d02-116">Read the properties and relationships of a term store object.</span></span>
|[<span data-ttu-id="e1d02-117">更新存储</span><span class="sxs-lookup"><span data-stu-id="e1d02-117">Update store</span></span>](../api/termstore-store-update.md) | [<span data-ttu-id="e1d02-118">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="e1d02-118">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="e1d02-119">更新术语库对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e1d02-119">Update the properties of a term store object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1d02-120">属性</span><span class="sxs-lookup"><span data-stu-id="e1d02-120">Properties</span></span>
|<span data-ttu-id="e1d02-121">属性</span><span class="sxs-lookup"><span data-stu-id="e1d02-121">Property</span></span>|<span data-ttu-id="e1d02-122">类型</span><span class="sxs-lookup"><span data-stu-id="e1d02-122">Type</span></span>|<span data-ttu-id="e1d02-123">说明</span><span class="sxs-lookup"><span data-stu-id="e1d02-123">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="e1d02-124">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="e1d02-124">defaultLanguageTag</span></span> | <span data-ttu-id="e1d02-125">String</span><span class="sxs-lookup"><span data-stu-id="e1d02-125">String</span></span> | <span data-ttu-id="e1d02-126">Termstore 的默认语言。</span><span class="sxs-lookup"><span data-stu-id="e1d02-126">Default language of the termstore.</span></span>
|<span data-ttu-id="e1d02-127">id</span><span class="sxs-lookup"><span data-stu-id="e1d02-127">id</span></span>|<span data-ttu-id="e1d02-128">String</span><span class="sxs-lookup"><span data-stu-id="e1d02-128">String</span></span> | <span data-ttu-id="e1d02-129">术语库的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e1d02-129">Unique identifier of the term store.</span></span> <span data-ttu-id="e1d02-130">只读。</span><span class="sxs-lookup"><span data-stu-id="e1d02-130">Read-only.</span></span>
|<span data-ttu-id="e1d02-131">languageTags</span><span class="sxs-lookup"><span data-stu-id="e1d02-131">languageTags</span></span> | <span data-ttu-id="e1d02-132">String collection</span><span class="sxs-lookup"><span data-stu-id="e1d02-132">String collection</span></span> | <span data-ttu-id="e1d02-133">术语库的语言列表。</span><span class="sxs-lookup"><span data-stu-id="e1d02-133">List of languages for the term store.</span></span>

## <a name="relationships"></a><span data-ttu-id="e1d02-134">关系</span><span class="sxs-lookup"><span data-stu-id="e1d02-134">Relationships</span></span>
|<span data-ttu-id="e1d02-135">关系</span><span class="sxs-lookup"><span data-stu-id="e1d02-135">Relationship</span></span>|<span data-ttu-id="e1d02-136">类型</span><span class="sxs-lookup"><span data-stu-id="e1d02-136">Type</span></span>|<span data-ttu-id="e1d02-137">说明</span><span class="sxs-lookup"><span data-stu-id="e1d02-137">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="e1d02-138">groups</span><span class="sxs-lookup"><span data-stu-id="e1d02-138">groups</span></span> |<span data-ttu-id="e1d02-139">[Microsoft termStore](../resources/termstore-group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1d02-139">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span> | <span data-ttu-id="e1d02-140">术语库中可用的所有组的集合。</span><span class="sxs-lookup"><span data-stu-id="e1d02-140">Collection of all groups available in the term store.</span></span>
|<span data-ttu-id="e1d02-141">下例</span><span class="sxs-lookup"><span data-stu-id="e1d02-141">sets</span></span> | <span data-ttu-id="e1d02-142">[Microsoft termStore](../resources/termstore-set.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1d02-142">[microsoft.graph.termStore.set](../resources/termstore-set.md) collection</span></span> | <span data-ttu-id="e1d02-143">术语库中可用的所有集的集合。</span><span class="sxs-lookup"><span data-stu-id="e1d02-143">Collection of all sets available in the term store.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1d02-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1d02-144">JSON representation</span></span>
<span data-ttu-id="e1d02-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1d02-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "TermStore is the top-level entity used for managing taxonomy for a client",
  "keywords": "termStore,facet,resource",
  "section": "documentation",
  "tocPath": "TermStore",
  "tocBookmarks": {
    "Resources/termStore.store": "#"
  },
  "suppressions": []
}
-->



