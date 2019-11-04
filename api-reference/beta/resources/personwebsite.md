---
title: personWebsite 资源类型
description: personWebsite 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: b5e6b8c3013c647087ab3d8db28b0196d0c79036
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949494"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="5d754-103">personWebsite 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d754-103">personWebsite resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d754-104">表示有关与各种服务中的用户相关联的网站的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5d754-104">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="5d754-105">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="5d754-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5d754-106">方法</span><span class="sxs-lookup"><span data-stu-id="5d754-106">Methods</span></span>

| <span data-ttu-id="5d754-107">方法</span><span class="sxs-lookup"><span data-stu-id="5d754-107">Method</span></span>                                           | <span data-ttu-id="5d754-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5d754-108">Return Type</span></span>                       | <span data-ttu-id="5d754-109">说明</span><span class="sxs-lookup"><span data-stu-id="5d754-109">Description</span></span>                                                |
|:-------------------------------------------------|:----------------------------------|:-----------------------------------------------------------|
| [<span data-ttu-id="5d754-110">获取 personWebsite</span><span class="sxs-lookup"><span data-stu-id="5d754-110">Get personWebsite</span></span>](../api/personwebsite-get.md) | [<span data-ttu-id="5d754-111">personWebsite</span><span class="sxs-lookup"><span data-stu-id="5d754-111">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="5d754-112">读取**personWebsite**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5d754-112">Read the properties and relationships of a **personWebsite** object.</span></span> |
| [<span data-ttu-id="5d754-113">更新 personWebsite</span><span class="sxs-lookup"><span data-stu-id="5d754-113">Update personWebsite</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="5d754-114">personWebsite</span><span class="sxs-lookup"><span data-stu-id="5d754-114">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="5d754-115">更新**personWebsite**对象。</span><span class="sxs-lookup"><span data-stu-id="5d754-115">Update a **personWebsite** object.</span></span>                               |
| [<span data-ttu-id="5d754-116">删除 personWebsite</span><span class="sxs-lookup"><span data-stu-id="5d754-116">Delete personWebsite</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="5d754-117">无</span><span class="sxs-lookup"><span data-stu-id="5d754-117">None</span></span>                              | <span data-ttu-id="5d754-118">删除**personWebsite**对象。</span><span class="sxs-lookup"><span data-stu-id="5d754-118">Delete a **personWebsite** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="5d754-119">属性</span><span class="sxs-lookup"><span data-stu-id="5d754-119">Properties</span></span>

| <span data-ttu-id="5d754-120">属性</span><span class="sxs-lookup"><span data-stu-id="5d754-120">Property</span></span>     | <span data-ttu-id="5d754-121">类型</span><span class="sxs-lookup"><span data-stu-id="5d754-121">Type</span></span>              | <span data-ttu-id="5d754-122">描述</span><span class="sxs-lookup"><span data-stu-id="5d754-122">Description</span></span>                                                                         |
|:-------------|:------------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="5d754-123">类别</span><span class="sxs-lookup"><span data-stu-id="5d754-123">categories</span></span>    |<span data-ttu-id="5d754-124">String collection</span><span class="sxs-lookup"><span data-stu-id="5d754-124">String collection</span></span>  | <span data-ttu-id="5d754-125">包含用户与网站相关联的类别（例如，个人、食谱）。</span><span class="sxs-lookup"><span data-stu-id="5d754-125">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="5d754-126">description</span><span class="sxs-lookup"><span data-stu-id="5d754-126">description</span></span>   |<span data-ttu-id="5d754-127">字符串</span><span class="sxs-lookup"><span data-stu-id="5d754-127">String</span></span>             | <span data-ttu-id="5d754-128">包含网站的说明。</span><span class="sxs-lookup"><span data-stu-id="5d754-128">Contains a description of the website.</span></span>                                              |
|<span data-ttu-id="5d754-129">displayName</span><span class="sxs-lookup"><span data-stu-id="5d754-129">displayName</span></span>   |<span data-ttu-id="5d754-130">String</span><span class="sxs-lookup"><span data-stu-id="5d754-130">String</span></span>             | <span data-ttu-id="5d754-131">包含网站的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5d754-131">Contains a friendly name for the website.</span></span>                                           |
|<span data-ttu-id="5d754-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="5d754-132">webUrl</span></span>        |<span data-ttu-id="5d754-133">String</span><span class="sxs-lookup"><span data-stu-id="5d754-133">String</span></span>             | <span data-ttu-id="5d754-134">包含指向网站本身的链接。</span><span class="sxs-lookup"><span data-stu-id="5d754-134">Contains a link to the website itself.</span></span>                                              |

## <a name="relationships"></a><span data-ttu-id="5d754-135">关系</span><span class="sxs-lookup"><span data-stu-id="5d754-135">Relationships</span></span>

<span data-ttu-id="5d754-136">无。</span><span class="sxs-lookup"><span data-stu-id="5d754-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d754-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d754-137">JSON representation</span></span>

<span data-ttu-id="5d754-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d754-138">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personWebsite",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "description": "String",
  "displayName": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personWebsite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
