---
title: conditionalAccessLocations 资源类型
description: 表示策略作用域中包含和排除的位置。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b4cdf4fbd1b81d4a4376983a424c2579376a76d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018898"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="f6b34-103">conditionalAccessLocations 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6b34-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="f6b34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6b34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6b34-105">表示策略作用域中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="f6b34-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="f6b34-106">属性</span><span class="sxs-lookup"><span data-stu-id="f6b34-106">Properties</span></span>

| <span data-ttu-id="f6b34-107">属性</span><span class="sxs-lookup"><span data-stu-id="f6b34-107">Property</span></span>     | <span data-ttu-id="f6b34-108">类型</span><span class="sxs-lookup"><span data-stu-id="f6b34-108">Type</span></span>        | <span data-ttu-id="f6b34-109">说明</span><span class="sxs-lookup"><span data-stu-id="f6b34-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f6b34-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="f6b34-110">includeLocations</span></span> | <span data-ttu-id="f6b34-111">String collection</span><span class="sxs-lookup"><span data-stu-id="f6b34-111">String collection</span></span> | <span data-ttu-id="f6b34-112">除非明确排除、或，否则策略范围中的位置 Id `All` `AllTrusted` 。</span><span class="sxs-lookup"><span data-stu-id="f6b34-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="f6b34-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="f6b34-113">excludeLocations</span></span> | <span data-ttu-id="f6b34-114">String collection</span><span class="sxs-lookup"><span data-stu-id="f6b34-114">String collection</span></span> | <span data-ttu-id="f6b34-115">从策略范围中排除的位置 Id。</span><span class="sxs-lookup"><span data-stu-id="f6b34-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f6b34-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6b34-116">JSON representation</span></span>

<span data-ttu-id="f6b34-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6b34-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="f6b34-118">关系</span><span class="sxs-lookup"><span data-stu-id="f6b34-118">Relationships</span></span>

<span data-ttu-id="f6b34-119">无。</span><span class="sxs-lookup"><span data-stu-id="f6b34-119">None.</span></span>

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

