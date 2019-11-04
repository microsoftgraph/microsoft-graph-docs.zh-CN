---
title: personInterest 资源类型
description: personInterest 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ef2675b8c604115fc5e04a7747dc4c110d567604
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939023"
---
# <a name="personinterest-resource-type"></a><span data-ttu-id="ee4f3-103">personInterest 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee4f3-103">personInterest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee4f3-104">[PersonInterest](personinterest.md)资源类型提供有关用户在各种服务中与其自身关联的兴趣的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-104">The [personInterest](personinterest.md) resource type provides detailed information about interests the user has associated with themselves in various services.</span></span>

<span data-ttu-id="ee4f3-105">继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ee4f3-106">方法</span><span class="sxs-lookup"><span data-stu-id="ee4f3-106">Methods</span></span>

| <span data-ttu-id="ee4f3-107">方法</span><span class="sxs-lookup"><span data-stu-id="ee4f3-107">Method</span></span>       | <span data-ttu-id="ee4f3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ee4f3-108">Return Type</span></span> | <span data-ttu-id="ee4f3-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee4f3-109">Description</span></span> |
|:---------------------------------------------------|:------------------------------------|:------------------------------------------------------------|
| [<span data-ttu-id="ee4f3-110">获取 personInterest</span><span class="sxs-lookup"><span data-stu-id="ee4f3-110">Get personInterest</span></span>](../api/personinterest-get.md) | [<span data-ttu-id="ee4f3-111">personInterest</span><span class="sxs-lookup"><span data-stu-id="ee4f3-111">personInterest</span></span>](personinterest.md) | <span data-ttu-id="ee4f3-112">读取 personInterest 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-112">Read properties and relationships of personInterest object.</span></span> |
| [<span data-ttu-id="ee4f3-113">Update</span><span class="sxs-lookup"><span data-stu-id="ee4f3-113">Update</span></span>](../api/personinterest-update.md)          | [<span data-ttu-id="ee4f3-114">personInterest</span><span class="sxs-lookup"><span data-stu-id="ee4f3-114">personInterest</span></span>](personinterest.md) | <span data-ttu-id="ee4f3-115">更新 personInterest 对象。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-115">Update personInterest object.</span></span>                               |
| [<span data-ttu-id="ee4f3-116">删除</span><span class="sxs-lookup"><span data-stu-id="ee4f3-116">Delete</span></span>](../api/personinterest-delete.md)          | <span data-ttu-id="ee4f3-117">无</span><span class="sxs-lookup"><span data-stu-id="ee4f3-117">None</span></span>                                | <span data-ttu-id="ee4f3-118">删除 personInterest 对象。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-118">Delete personInterest object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="ee4f3-119">属性</span><span class="sxs-lookup"><span data-stu-id="ee4f3-119">Properties</span></span>

| <span data-ttu-id="ee4f3-120">属性</span><span class="sxs-lookup"><span data-stu-id="ee4f3-120">Property</span></span>     | <span data-ttu-id="ee4f3-121">类型</span><span class="sxs-lookup"><span data-stu-id="ee4f3-121">Type</span></span>             | <span data-ttu-id="ee4f3-122">描述</span><span class="sxs-lookup"><span data-stu-id="ee4f3-122">Description</span></span>                                                                          |
|:-------------|:-----------------|:-------------------------------------------------------------------------------------|
|<span data-ttu-id="ee4f3-123">类别</span><span class="sxs-lookup"><span data-stu-id="ee4f3-123">categories</span></span>    |<span data-ttu-id="ee4f3-124">String collection</span><span class="sxs-lookup"><span data-stu-id="ee4f3-124">String collection</span></span> | <span data-ttu-id="ee4f3-125">包含用户与兴趣相关联的类别（例如： personal、recipies）</span><span class="sxs-lookup"><span data-stu-id="ee4f3-125">Contains categories a user has associated with the interest (eg: personal, recipies)</span></span> |
|<span data-ttu-id="ee4f3-126">description</span><span class="sxs-lookup"><span data-stu-id="ee4f3-126">description</span></span>   |<span data-ttu-id="ee4f3-127">字符串</span><span class="sxs-lookup"><span data-stu-id="ee4f3-127">String</span></span>            | <span data-ttu-id="ee4f3-128">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-128">Contains a description of the interest.</span></span>                                              |
|<span data-ttu-id="ee4f3-129">displayName</span><span class="sxs-lookup"><span data-stu-id="ee4f3-129">displayName</span></span>   |<span data-ttu-id="ee4f3-130">String</span><span class="sxs-lookup"><span data-stu-id="ee4f3-130">String</span></span>            | <span data-ttu-id="ee4f3-131">包含利息的友好名称。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-131">Contains a friendly name for the interest.</span></span>                                           |
|<span data-ttu-id="ee4f3-132">webUrl</span><span class="sxs-lookup"><span data-stu-id="ee4f3-132">webUrl</span></span>        |<span data-ttu-id="ee4f3-133">String</span><span class="sxs-lookup"><span data-stu-id="ee4f3-133">String</span></span>            | <span data-ttu-id="ee4f3-134">包含有关感兴趣的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-134">Contains a link to a webpage or resource about the interest.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="ee4f3-135">关系</span><span class="sxs-lookup"><span data-stu-id="ee4f3-135">Relationships</span></span>

<span data-ttu-id="ee4f3-136">无</span><span class="sxs-lookup"><span data-stu-id="ee4f3-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee4f3-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee4f3-137">JSON representation</span></span>

<span data-ttu-id="ee4f3-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee4f3-138">The following is a JSON representation of the resource.</span></span> 

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