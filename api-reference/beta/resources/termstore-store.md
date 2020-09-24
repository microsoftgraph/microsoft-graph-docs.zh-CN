---
title: 存储资源类型
description: 表示分类术语库。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de8b0c004da804a4d9a617eec20de22c51e98108
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258424"
---
# <a name="store-resource-type"></a><span data-ttu-id="f1d27-103">存储资源类型</span><span class="sxs-lookup"><span data-stu-id="f1d27-103">store resource type</span></span>

<span data-ttu-id="f1d27-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="f1d27-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1d27-105">表示分类术语库。</span><span class="sxs-lookup"><span data-stu-id="f1d27-105">Represents a taxonomy term store.</span></span>

<span data-ttu-id="f1d27-106">继承自 [entity](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="f1d27-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f1d27-107">方法</span><span class="sxs-lookup"><span data-stu-id="f1d27-107">Methods</span></span>
|<span data-ttu-id="f1d27-108">方法</span><span class="sxs-lookup"><span data-stu-id="f1d27-108">Method</span></span>|<span data-ttu-id="f1d27-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1d27-109">Return type</span></span>|<span data-ttu-id="f1d27-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1d27-110">Description</span></span>
|:---|:---|:---
|[<span data-ttu-id="f1d27-111">List groups</span><span class="sxs-lookup"><span data-stu-id="f1d27-111">List groups</span></span>](../api/termstore-list-groups.md)|<span data-ttu-id="f1d27-112">[Microsoft termStore](../resources/termstore-group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1d27-112">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span>| <span data-ttu-id="f1d27-113">将组从术语库对象中的提供中获取。</span><span class="sxs-lookup"><span data-stu-id="f1d27-113">Get the groups from available in the term store object.</span></span>|
|[<span data-ttu-id="f1d27-114">获取存储区</span><span class="sxs-lookup"><span data-stu-id="f1d27-114">Get store</span></span>](../api/termstore-store-get.md) | [<span data-ttu-id="f1d27-115">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="f1d27-115">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="f1d27-116">读取术语库对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1d27-116">Read the properties and relationships of a term store object.</span></span>
|[<span data-ttu-id="f1d27-117">更新存储</span><span class="sxs-lookup"><span data-stu-id="f1d27-117">Update store</span></span>](../api/termstore-store-update.md) | [<span data-ttu-id="f1d27-118">microsoft termStore</span><span class="sxs-lookup"><span data-stu-id="f1d27-118">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="f1d27-119">更新术语库对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f1d27-119">Update the properties of a term store object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1d27-120">属性</span><span class="sxs-lookup"><span data-stu-id="f1d27-120">Properties</span></span>
|<span data-ttu-id="f1d27-121">属性</span><span class="sxs-lookup"><span data-stu-id="f1d27-121">Property</span></span>|<span data-ttu-id="f1d27-122">类型</span><span class="sxs-lookup"><span data-stu-id="f1d27-122">Type</span></span>|<span data-ttu-id="f1d27-123">说明</span><span class="sxs-lookup"><span data-stu-id="f1d27-123">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="f1d27-124">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="f1d27-124">defaultLanguageTag</span></span> | <span data-ttu-id="f1d27-125">字符串</span><span class="sxs-lookup"><span data-stu-id="f1d27-125">String</span></span> | <span data-ttu-id="f1d27-126">术语库的默认语言。</span><span class="sxs-lookup"><span data-stu-id="f1d27-126">Default language of the term store.</span></span>
|<span data-ttu-id="f1d27-127">id</span><span class="sxs-lookup"><span data-stu-id="f1d27-127">id</span></span>|<span data-ttu-id="f1d27-128">字符串</span><span class="sxs-lookup"><span data-stu-id="f1d27-128">String</span></span> | <span data-ttu-id="f1d27-129">术语库的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f1d27-129">Unique identifier of the term store.</span></span> <span data-ttu-id="f1d27-130">只读。</span><span class="sxs-lookup"><span data-stu-id="f1d27-130">Read-only.</span></span>
|<span data-ttu-id="f1d27-131">languageTags</span><span class="sxs-lookup"><span data-stu-id="f1d27-131">languageTags</span></span> | <span data-ttu-id="f1d27-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="f1d27-132">String collection</span></span> | <span data-ttu-id="f1d27-133">术语库的语言列表。</span><span class="sxs-lookup"><span data-stu-id="f1d27-133">List of languages for the term store.</span></span>

## <a name="relationships"></a><span data-ttu-id="f1d27-134">关系</span><span class="sxs-lookup"><span data-stu-id="f1d27-134">Relationships</span></span>
|<span data-ttu-id="f1d27-135">关系</span><span class="sxs-lookup"><span data-stu-id="f1d27-135">Relationship</span></span>|<span data-ttu-id="f1d27-136">类型</span><span class="sxs-lookup"><span data-stu-id="f1d27-136">Type</span></span>|<span data-ttu-id="f1d27-137">说明</span><span class="sxs-lookup"><span data-stu-id="f1d27-137">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="f1d27-138">groups</span><span class="sxs-lookup"><span data-stu-id="f1d27-138">groups</span></span> |<span data-ttu-id="f1d27-139">[Microsoft termStore](../resources/termstore-group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1d27-139">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span> | <span data-ttu-id="f1d27-140">术语库中可用的所有组的集合。</span><span class="sxs-lookup"><span data-stu-id="f1d27-140">Collection of all groups available in the term store.</span></span>
|<span data-ttu-id="f1d27-141">下例</span><span class="sxs-lookup"><span data-stu-id="f1d27-141">sets</span></span> | <span data-ttu-id="f1d27-142">[Microsoft termStore](../resources/termstore-set.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1d27-142">[microsoft.graph.termStore.set](../resources/termstore-set.md) collection</span></span> | <span data-ttu-id="f1d27-143">术语库中可用的所有集的集合。</span><span class="sxs-lookup"><span data-stu-id="f1d27-143">Collection of all sets available in the term store.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f1d27-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1d27-144">JSON representation</span></span>
<span data-ttu-id="f1d27-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1d27-145">The following is a JSON representation of the resource.</span></span>
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



