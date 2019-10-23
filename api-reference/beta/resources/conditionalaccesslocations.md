---
title: conditionalAccessLocations 资源类型
description: 表示策略作用域中包含和排除的位置。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6997664eb131664bcaaf571398ed393fb13c987c
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638566"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="c1eae-103">conditionalAccessLocations 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1eae-103">conditionalAccessLocations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1eae-104">表示策略作用域中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="c1eae-104">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="c1eae-105">属性</span><span class="sxs-lookup"><span data-stu-id="c1eae-105">Properties</span></span>

| <span data-ttu-id="c1eae-106">属性</span><span class="sxs-lookup"><span data-stu-id="c1eae-106">Property</span></span>     | <span data-ttu-id="c1eae-107">类型</span><span class="sxs-lookup"><span data-stu-id="c1eae-107">Type</span></span>        | <span data-ttu-id="c1eae-108">说明</span><span class="sxs-lookup"><span data-stu-id="c1eae-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c1eae-109">includeLocations</span><span class="sxs-lookup"><span data-stu-id="c1eae-109">includeLocations</span></span> | <span data-ttu-id="c1eae-110">String collection</span><span class="sxs-lookup"><span data-stu-id="c1eae-110">String collection</span></span> | <span data-ttu-id="c1eae-111">除非明确排除、 `All`或`AllTrusted`，否则策略范围中的位置 id。</span><span class="sxs-lookup"><span data-stu-id="c1eae-111">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="c1eae-112">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="c1eae-112">excludeLocations</span></span> | <span data-ttu-id="c1eae-113">String collection</span><span class="sxs-lookup"><span data-stu-id="c1eae-113">String collection</span></span> | <span data-ttu-id="c1eae-114">从策略范围中排除的位置 Id。</span><span class="sxs-lookup"><span data-stu-id="c1eae-114">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1eae-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1eae-115">JSON representation</span></span>

<span data-ttu-id="c1eae-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1eae-116">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="c1eae-117">关系</span><span class="sxs-lookup"><span data-stu-id="c1eae-117">Relationships</span></span>

<span data-ttu-id="c1eae-118">无。</span><span class="sxs-lookup"><span data-stu-id="c1eae-118">None.</span></span>

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