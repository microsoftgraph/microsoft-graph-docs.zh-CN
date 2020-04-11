---
title: personWebsite 资源类型
description: personWebsite 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4e37e769832340676f0d206b6727a57ce9809361
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227687"
---
# <a name="personwebsite-resource-type"></a><span data-ttu-id="e9355-103">personWebsite 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9355-103">personWebsite resource type</span></span>

<span data-ttu-id="e9355-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9355-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9355-105">表示有关与各种服务中的用户相关联的网站的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e9355-105">Represents detailed information about websites associated with a user in various services.</span></span>

<span data-ttu-id="e9355-106">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e9355-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e9355-107">方法</span><span class="sxs-lookup"><span data-stu-id="e9355-107">Methods</span></span>

| <span data-ttu-id="e9355-108">方法</span><span class="sxs-lookup"><span data-stu-id="e9355-108">Method</span></span>                                                         | <span data-ttu-id="e9355-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e9355-109">Return Type</span></span>                       | <span data-ttu-id="e9355-110">说明</span><span class="sxs-lookup"><span data-stu-id="e9355-110">Description</span></span>                                                          |
|:---------------------------------------------------------------|:----------------------------------|:---------------------------------------------------------------------|
| [<span data-ttu-id="e9355-111">获取 personWebsite</span><span class="sxs-lookup"><span data-stu-id="e9355-111">Get personWebsite</span></span>](../api/personwebsite-get.md)               | [<span data-ttu-id="e9355-112">personWebsite</span><span class="sxs-lookup"><span data-stu-id="e9355-112">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="e9355-113">读取**personWebsite**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e9355-113">Read the properties and relationships of a **personWebsite** object.</span></span> |
| [<span data-ttu-id="e9355-114">更新 personWebsite</span><span class="sxs-lookup"><span data-stu-id="e9355-114">Update personWebsite</span></span>](../api/personwebsite-update.md)         | [<span data-ttu-id="e9355-115">personWebsite</span><span class="sxs-lookup"><span data-stu-id="e9355-115">personWebsite</span></span>](personwebsite.md) | <span data-ttu-id="e9355-116">更新**personWebsite**对象。</span><span class="sxs-lookup"><span data-stu-id="e9355-116">Update a **personWebsite** object.</span></span>                                   |
| [<span data-ttu-id="e9355-117">删除 personWebsite</span><span class="sxs-lookup"><span data-stu-id="e9355-117">Delete personWebsite</span></span>](../api/personwebsite-delete.md)         | <span data-ttu-id="e9355-118">无</span><span class="sxs-lookup"><span data-stu-id="e9355-118">None</span></span>                              | <span data-ttu-id="e9355-119">删除**personWebsite**对象。</span><span class="sxs-lookup"><span data-stu-id="e9355-119">Delete a **personWebsite** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="e9355-120">属性</span><span class="sxs-lookup"><span data-stu-id="e9355-120">Properties</span></span>

| <span data-ttu-id="e9355-121">属性</span><span class="sxs-lookup"><span data-stu-id="e9355-121">Property</span></span>     | <span data-ttu-id="e9355-122">类型</span><span class="sxs-lookup"><span data-stu-id="e9355-122">Type</span></span>              | <span data-ttu-id="e9355-123">说明</span><span class="sxs-lookup"><span data-stu-id="e9355-123">Description</span></span>                                                                                   |
|:-------------|:------------------|:----------------------------------------------------------------------------------------------|
|<span data-ttu-id="e9355-124">categories</span><span class="sxs-lookup"><span data-stu-id="e9355-124">categories</span></span>    |<span data-ttu-id="e9355-125">String 集合</span><span class="sxs-lookup"><span data-stu-id="e9355-125">String collection</span></span>  | <span data-ttu-id="e9355-126">包含用户与网站相关联的类别（例如，个人、食谱）。</span><span class="sxs-lookup"><span data-stu-id="e9355-126">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>  |
|<span data-ttu-id="e9355-127">说明</span><span class="sxs-lookup"><span data-stu-id="e9355-127">description</span></span>   |<span data-ttu-id="e9355-128">字符串</span><span class="sxs-lookup"><span data-stu-id="e9355-128">String</span></span>             | <span data-ttu-id="e9355-129">包含网站的说明。</span><span class="sxs-lookup"><span data-stu-id="e9355-129">Contains a description of the website.</span></span>                                                        |
|<span data-ttu-id="e9355-130">displayName</span><span class="sxs-lookup"><span data-stu-id="e9355-130">displayName</span></span>   |<span data-ttu-id="e9355-131">String</span><span class="sxs-lookup"><span data-stu-id="e9355-131">String</span></span>             | <span data-ttu-id="e9355-132">包含网站的友好名称。</span><span class="sxs-lookup"><span data-stu-id="e9355-132">Contains a friendly name for the website.</span></span>                                                     |
|<span data-ttu-id="e9355-133">WebUrl</span><span class="sxs-lookup"><span data-stu-id="e9355-133">webUrl</span></span>        |<span data-ttu-id="e9355-134">String</span><span class="sxs-lookup"><span data-stu-id="e9355-134">String</span></span>             | <span data-ttu-id="e9355-135">包含指向网站本身的链接。</span><span class="sxs-lookup"><span data-stu-id="e9355-135">Contains a link to the website itself.</span></span>                                                        |

## <a name="relationships"></a><span data-ttu-id="e9355-136">关系</span><span class="sxs-lookup"><span data-stu-id="e9355-136">Relationships</span></span>

<span data-ttu-id="e9355-137">无。</span><span class="sxs-lookup"><span data-stu-id="e9355-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9355-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9355-138">JSON representation</span></span>

<span data-ttu-id="e9355-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9355-139">The following is a JSON representation of the resource.</span></span>

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
