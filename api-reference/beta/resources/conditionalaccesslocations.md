---
title: conditionalAccessLocations 资源类型
description: 表示包含在策略作用域中和从策略范围中排除的位置。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 153d64d32015fcd6119a4d880bbc786905c39b9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132385"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="b437e-103">conditionalAccessLocations 资源类型</span><span class="sxs-lookup"><span data-stu-id="b437e-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="b437e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b437e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b437e-105">表示包含在策略作用域中和从策略范围中排除的位置。</span><span class="sxs-lookup"><span data-stu-id="b437e-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="b437e-106">属性</span><span class="sxs-lookup"><span data-stu-id="b437e-106">Properties</span></span>

| <span data-ttu-id="b437e-107">属性</span><span class="sxs-lookup"><span data-stu-id="b437e-107">Property</span></span>     | <span data-ttu-id="b437e-108">类型</span><span class="sxs-lookup"><span data-stu-id="b437e-108">Type</span></span>        | <span data-ttu-id="b437e-109">说明</span><span class="sxs-lookup"><span data-stu-id="b437e-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b437e-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="b437e-110">includeLocations</span></span> | <span data-ttu-id="b437e-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b437e-111">String collection</span></span> | <span data-ttu-id="b437e-112">除非明确排除，否则策略范围内的位置 `All` ID 或 `AllTrusted` 。</span><span class="sxs-lookup"><span data-stu-id="b437e-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="b437e-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="b437e-113">excludeLocations</span></span> | <span data-ttu-id="b437e-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b437e-114">String collection</span></span> | <span data-ttu-id="b437e-115">从策略作用域中排除的位置 ID。</span><span class="sxs-lookup"><span data-stu-id="b437e-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b437e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b437e-116">JSON representation</span></span>

<span data-ttu-id="b437e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b437e-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="b437e-118">关系</span><span class="sxs-lookup"><span data-stu-id="b437e-118">Relationships</span></span>

<span data-ttu-id="b437e-119">无。</span><span class="sxs-lookup"><span data-stu-id="b437e-119">None.</span></span>

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

