---
title: conditionalAccessLocations 资源类型
description: 表示策略作用域中包含和排除的位置。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a92d99d7a9e80084b8ec1ce385ce76d1f522b359
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916780"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="3a5c6-103">conditionalAccessLocations 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a5c6-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="3a5c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a5c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a5c6-105">表示策略作用域中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="3a5c6-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="3a5c6-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a5c6-106">Properties</span></span>

| <span data-ttu-id="3a5c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a5c6-107">Property</span></span>     | <span data-ttu-id="3a5c6-108">类型</span><span class="sxs-lookup"><span data-stu-id="3a5c6-108">Type</span></span>        | <span data-ttu-id="3a5c6-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a5c6-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3a5c6-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="3a5c6-110">includeLocations</span></span> | <span data-ttu-id="3a5c6-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="3a5c6-111">String collection</span></span> | <span data-ttu-id="3a5c6-112">除非明确排除、 `All`或`AllTrusted`，否则策略范围中的位置 id。</span><span class="sxs-lookup"><span data-stu-id="3a5c6-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="3a5c6-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="3a5c6-113">excludeLocations</span></span> | <span data-ttu-id="3a5c6-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="3a5c6-114">String collection</span></span> | <span data-ttu-id="3a5c6-115">从策略范围中排除的位置 Id。</span><span class="sxs-lookup"><span data-stu-id="3a5c6-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a5c6-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a5c6-116">JSON representation</span></span>

<span data-ttu-id="3a5c6-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a5c6-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="3a5c6-118">关系</span><span class="sxs-lookup"><span data-stu-id="3a5c6-118">Relationships</span></span>

<span data-ttu-id="3a5c6-119">无。</span><span class="sxs-lookup"><span data-stu-id="3a5c6-119">None.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeLocations",
    "excludeLocations"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessLocations",
  "baseType": null
}-->

```json
{
  "excludeLocations": ["String"],
  "includeLocations": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessLocations resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->