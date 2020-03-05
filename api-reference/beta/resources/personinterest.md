---
title: personInterest 资源类型
description: personInterest 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1da3ad429011da62f49105c6f352c86ec0741cd4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521909"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="f545b-103">personInterest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f545b-103">personInterest resource type</span></span>

<span data-ttu-id="f545b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f545b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f545b-105">提供有关用户在各种服务中与其自身关联的兴趣的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f545b-105">Provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="f545b-106">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f545b-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f545b-107">方法</span><span class="sxs-lookup"><span data-stu-id="f545b-107">Methods</span></span>

| <span data-ttu-id="f545b-108">方法</span><span class="sxs-lookup"><span data-stu-id="f545b-108">Method</span></span>       | <span data-ttu-id="f545b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f545b-109">Return Type</span></span> | <span data-ttu-id="f545b-110">说明</span><span class="sxs-lookup"><span data-stu-id="f545b-110">Description</span></span> |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [<span data-ttu-id="f545b-111">获取 personInterest</span><span class="sxs-lookup"><span data-stu-id="f545b-111">Get personInterest</span></span>](../api/personinterest-get.md) | [<span data-ttu-id="f545b-112">personInterest</span><span class="sxs-lookup"><span data-stu-id="f545b-112">personInterest</span></span>](personinterest.md) | <span data-ttu-id="f545b-113">读取**personInterest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f545b-113">Read the properties and relationships of a **personInterest** object.</span></span> |
| [<span data-ttu-id="f545b-114">更新 personInterest</span><span class="sxs-lookup"><span data-stu-id="f545b-114">Update personInterest</span></span>](../api/personinterest-update.md)          | [<span data-ttu-id="f545b-115">personInterest</span><span class="sxs-lookup"><span data-stu-id="f545b-115">personInterest</span></span>](personinterest.md) | <span data-ttu-id="f545b-116">更新**personInterest**对象。</span><span class="sxs-lookup"><span data-stu-id="f545b-116">Update a **personInterest** object.</span></span>                               |
| [<span data-ttu-id="f545b-117">删除 personInterest</span><span class="sxs-lookup"><span data-stu-id="f545b-117">Delete personInterest</span></span>](../api/personinterest-delete.md)          | <span data-ttu-id="f545b-118">无</span><span class="sxs-lookup"><span data-stu-id="f545b-118">None</span></span>                                | <span data-ttu-id="f545b-119">删除**personInterest**对象。</span><span class="sxs-lookup"><span data-stu-id="f545b-119">Delete a **personInterest** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="f545b-120">属性</span><span class="sxs-lookup"><span data-stu-id="f545b-120">Properties</span></span>

| <span data-ttu-id="f545b-121">属性</span><span class="sxs-lookup"><span data-stu-id="f545b-121">Property</span></span>     | <span data-ttu-id="f545b-122">类型</span><span class="sxs-lookup"><span data-stu-id="f545b-122">Type</span></span>             | <span data-ttu-id="f545b-123">说明</span><span class="sxs-lookup"><span data-stu-id="f545b-123">Description</span></span>                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|<span data-ttu-id="f545b-124">categories</span><span class="sxs-lookup"><span data-stu-id="f545b-124">categories</span></span>    |<span data-ttu-id="f545b-125">String 集合</span><span class="sxs-lookup"><span data-stu-id="f545b-125">String collection</span></span> | <span data-ttu-id="f545b-126">包含用户与兴趣相关联的类别（例如，个人、recipies）。</span><span class="sxs-lookup"><span data-stu-id="f545b-126">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="f545b-127">说明</span><span class="sxs-lookup"><span data-stu-id="f545b-127">description</span></span>   |<span data-ttu-id="f545b-128">字符串</span><span class="sxs-lookup"><span data-stu-id="f545b-128">String</span></span>            | <span data-ttu-id="f545b-129">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="f545b-129">Contains a description of the interest.</span></span>                                              |
|<span data-ttu-id="f545b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="f545b-130">displayName</span></span>   |<span data-ttu-id="f545b-131">String</span><span class="sxs-lookup"><span data-stu-id="f545b-131">String</span></span>            | <span data-ttu-id="f545b-132">包含利息的友好名称。</span><span class="sxs-lookup"><span data-stu-id="f545b-132">Contains a friendly name for the interest.</span></span>                                           |
|<span data-ttu-id="f545b-133">webUrl</span><span class="sxs-lookup"><span data-stu-id="f545b-133">webUrl</span></span>        |<span data-ttu-id="f545b-134">String</span><span class="sxs-lookup"><span data-stu-id="f545b-134">String</span></span>            | <span data-ttu-id="f545b-135">包含指向有关该兴趣的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="f545b-135">Contains a link to a web page or resource about the interest.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="f545b-136">关系</span><span class="sxs-lookup"><span data-stu-id="f545b-136">Relationships</span></span>

<span data-ttu-id="f545b-137">无。</span><span class="sxs-lookup"><span data-stu-id="f545b-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f545b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f545b-138">JSON representation</span></span>

<span data-ttu-id="f545b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f545b-139">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personInterest",
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
  "description": "personInterest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
