---
title: workPosition 资源类型
description: workPosition 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: d55a6d2572ec5ecbe190d8ab7dde3b2a7dd67f09
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228857"
---
# <a name="workposition-resource-type"></a><span data-ttu-id="52452-103">workPosition 资源类型</span><span class="sxs-lookup"><span data-stu-id="52452-103">workPosition resource type</span></span>

<span data-ttu-id="52452-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52452-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52452-105">表示有关与用户[配置文件](profile.md)相关联的工作职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="52452-105">Represents detailed information about work positions associated with a user's [profile](profile.md).</span></span>

<span data-ttu-id="52452-106">此资源类型继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="52452-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="52452-107">方法</span><span class="sxs-lookup"><span data-stu-id="52452-107">Methods</span></span>

| <span data-ttu-id="52452-108">方法</span><span class="sxs-lookup"><span data-stu-id="52452-108">Method</span></span>                                                      | <span data-ttu-id="52452-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="52452-109">Return Type</span></span>                     | <span data-ttu-id="52452-110">说明</span><span class="sxs-lookup"><span data-stu-id="52452-110">Description</span></span>                                                         |
|:------------------------------------------------------------|:--------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="52452-111">获取 workPosition</span><span class="sxs-lookup"><span data-stu-id="52452-111">Get workPosition</span></span>](../api/workposition-get.md)              | [<span data-ttu-id="52452-112">workPosition</span><span class="sxs-lookup"><span data-stu-id="52452-112">workPosition</span></span>](workposition.md) | <span data-ttu-id="52452-113">读取**workPosition**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="52452-113">Read the properties and relationships of a **workPosition** object.</span></span> |
| [<span data-ttu-id="52452-114">更新 workPosition</span><span class="sxs-lookup"><span data-stu-id="52452-114">Update workPosition</span></span>](../api/workposition-update.md)        | [<span data-ttu-id="52452-115">workPosition</span><span class="sxs-lookup"><span data-stu-id="52452-115">workPosition</span></span>](workposition.md) | <span data-ttu-id="52452-116">更新**workPosition**对象。</span><span class="sxs-lookup"><span data-stu-id="52452-116">Update a **workPosition** object.</span></span>                                   |
| [<span data-ttu-id="52452-117">删除 workPosition</span><span class="sxs-lookup"><span data-stu-id="52452-117">Delete workPosition</span></span>](../api/workposition-delete.md)        | <span data-ttu-id="52452-118">无</span><span class="sxs-lookup"><span data-stu-id="52452-118">None</span></span>                            | <span data-ttu-id="52452-119">删除**workPosition**对象。</span><span class="sxs-lookup"><span data-stu-id="52452-119">Delete a **workPosition** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="52452-120">属性</span><span class="sxs-lookup"><span data-stu-id="52452-120">Properties</span></span>

| <span data-ttu-id="52452-121">属性</span><span class="sxs-lookup"><span data-stu-id="52452-121">Property</span></span>             | <span data-ttu-id="52452-122">类型</span><span class="sxs-lookup"><span data-stu-id="52452-122">Type</span></span>                                | <span data-ttu-id="52452-123">说明</span><span class="sxs-lookup"><span data-stu-id="52452-123">Description</span></span>                                                                                                |
|:---------------------|:------------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="52452-124">categories</span><span class="sxs-lookup"><span data-stu-id="52452-124">categories</span></span>            | <span data-ttu-id="52452-125">String 集合</span><span class="sxs-lookup"><span data-stu-id="52452-125">String collection</span></span>                   | <span data-ttu-id="52452-126">包含用户与位置相关联的类别（例如，数字转换、人员）。</span><span class="sxs-lookup"><span data-stu-id="52452-126">Contains categories a user has associated with the position (for example, digital transformation, people).</span></span> |
|<span data-ttu-id="52452-127">介绍</span><span class="sxs-lookup"><span data-stu-id="52452-127">detail</span></span>                | [<span data-ttu-id="52452-128">positionDetail</span><span class="sxs-lookup"><span data-stu-id="52452-128">positionDetail</span></span>](positiondetail.md) | <span data-ttu-id="52452-129">包含有关用户的当前和前一个雇用职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="52452-129">Contains detail about the user's current and previous employment positions.</span></span>                                |

## <a name="relationships"></a><span data-ttu-id="52452-130">关系</span><span class="sxs-lookup"><span data-stu-id="52452-130">Relationships</span></span>

<span data-ttu-id="52452-131">无。</span><span class="sxs-lookup"><span data-stu-id="52452-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52452-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52452-132">JSON representation</span></span>

<span data-ttu-id="52452-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52452-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workPosition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
