---
title: workPosition 资源类型
description: workPosition 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2a0d742d289cefac825155a2e8917365c0bb97af
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950463"
---
# <a name="workposition-resource-type"></a><span data-ttu-id="fc6ca-103">workPosition 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc6ca-103">workPosition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc6ca-104">表示有关与用户[配置文件](profile.md)相关联的工作职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-104">Represents detailed information about work positions associated with a user's [profile](profile.md).</span></span>

<span data-ttu-id="fc6ca-105">此资源类型继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-105">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fc6ca-106">方法</span><span class="sxs-lookup"><span data-stu-id="fc6ca-106">Methods</span></span>

| <span data-ttu-id="fc6ca-107">方法</span><span class="sxs-lookup"><span data-stu-id="fc6ca-107">Method</span></span>                                         | <span data-ttu-id="fc6ca-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="fc6ca-108">Return Type</span></span>                     | <span data-ttu-id="fc6ca-109">说明</span><span class="sxs-lookup"><span data-stu-id="fc6ca-109">Description</span></span>                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [<span data-ttu-id="fc6ca-110">获取 workPosition</span><span class="sxs-lookup"><span data-stu-id="fc6ca-110">Get workPosition</span></span>](../api/workposition-get.md) | [<span data-ttu-id="fc6ca-111">workPosition</span><span class="sxs-lookup"><span data-stu-id="fc6ca-111">workPosition</span></span>](workposition.md) | <span data-ttu-id="fc6ca-112">读取**workPosition**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-112">Read the properties and relationships of a **workPosition** object.</span></span> |
| [<span data-ttu-id="fc6ca-113">更新 workPosition</span><span class="sxs-lookup"><span data-stu-id="fc6ca-113">Update workPosition</span></span>](../api/workposition-update.md)        | [<span data-ttu-id="fc6ca-114">workPosition</span><span class="sxs-lookup"><span data-stu-id="fc6ca-114">workPosition</span></span>](workposition.md) | <span data-ttu-id="fc6ca-115">更新**workPosition**对象。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-115">Update a **workPosition** object.</span></span>                               |
| [<span data-ttu-id="fc6ca-116">删除 workPosition</span><span class="sxs-lookup"><span data-stu-id="fc6ca-116">Delete workPosition</span></span>](../api/workposition-delete.md)        | <span data-ttu-id="fc6ca-117">无</span><span class="sxs-lookup"><span data-stu-id="fc6ca-117">None</span></span>                            | <span data-ttu-id="fc6ca-118">删除**workPosition**对象。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-118">Delete a **workPosition** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="fc6ca-119">属性</span><span class="sxs-lookup"><span data-stu-id="fc6ca-119">Properties</span></span>

| <span data-ttu-id="fc6ca-120">属性</span><span class="sxs-lookup"><span data-stu-id="fc6ca-120">Property</span></span>             | <span data-ttu-id="fc6ca-121">类型</span><span class="sxs-lookup"><span data-stu-id="fc6ca-121">Type</span></span>                               | <span data-ttu-id="fc6ca-122">描述</span><span class="sxs-lookup"><span data-stu-id="fc6ca-122">Description</span></span>                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="fc6ca-123">类别</span><span class="sxs-lookup"><span data-stu-id="fc6ca-123">categories</span></span>            |<span data-ttu-id="fc6ca-124">String collection</span><span class="sxs-lookup"><span data-stu-id="fc6ca-124">String collection</span></span>                   | <span data-ttu-id="fc6ca-125">包含用户与位置相关联的类别（例如，数字转换、人员）。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-125">Contains categories a user has associated with the position (for example, digital transformation, people).</span></span> |
|<span data-ttu-id="fc6ca-126">介绍</span><span class="sxs-lookup"><span data-stu-id="fc6ca-126">detail</span></span>                |[<span data-ttu-id="fc6ca-127">positionDetail</span><span class="sxs-lookup"><span data-stu-id="fc6ca-127">positionDetail</span></span>](positiondetail.md) | <span data-ttu-id="fc6ca-128">包含有关用户的当前和前一个雇用职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-128">Contains detail about the user's current and previous employment positions.</span></span>                                 |

## <a name="relationships"></a><span data-ttu-id="fc6ca-129">关系</span><span class="sxs-lookup"><span data-stu-id="fc6ca-129">Relationships</span></span>

<span data-ttu-id="fc6ca-130">无。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc6ca-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc6ca-131">JSON representation</span></span>

<span data-ttu-id="fc6ca-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc6ca-132">The following is a JSON representation of the resource.</span></span>

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
