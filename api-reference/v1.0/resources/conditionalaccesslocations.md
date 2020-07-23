---
title: conditionalAccessLocations 资源类型
description: 表示策略作用域中包含和排除的位置。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5378764f36bf5fed858755a475fd85a400a2fed
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384469"
---
# <a name="conditionalaccesslocations-resource-type"></a><span data-ttu-id="e3f8f-103">conditionalAccessLocations 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3f8f-103">conditionalAccessLocations resource type</span></span>

<span data-ttu-id="e3f8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3f8f-105">表示策略作用域中包含和排除的位置。</span><span class="sxs-lookup"><span data-stu-id="e3f8f-105">Represents locations included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="e3f8f-106">属性</span><span class="sxs-lookup"><span data-stu-id="e3f8f-106">Properties</span></span>

| <span data-ttu-id="e3f8f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e3f8f-107">Property</span></span>     | <span data-ttu-id="e3f8f-108">类型</span><span class="sxs-lookup"><span data-stu-id="e3f8f-108">Type</span></span>        | <span data-ttu-id="e3f8f-109">说明</span><span class="sxs-lookup"><span data-stu-id="e3f8f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e3f8f-110">includeLocations</span><span class="sxs-lookup"><span data-stu-id="e3f8f-110">includeLocations</span></span> | <span data-ttu-id="e3f8f-111">String collection</span><span class="sxs-lookup"><span data-stu-id="e3f8f-111">String collection</span></span> | <span data-ttu-id="e3f8f-112">除非明确排除、或，否则策略范围中的位置 Id `All` `AllTrusted` 。</span><span class="sxs-lookup"><span data-stu-id="e3f8f-112">Location IDs in scope of policy unless explicitly excluded, `All`, or `AllTrusted`.</span></span> |
| <span data-ttu-id="e3f8f-113">excludeLocations</span><span class="sxs-lookup"><span data-stu-id="e3f8f-113">excludeLocations</span></span> | <span data-ttu-id="e3f8f-114">String collection</span><span class="sxs-lookup"><span data-stu-id="e3f8f-114">String collection</span></span> | <span data-ttu-id="e3f8f-115">从策略范围中排除的位置 Id。</span><span class="sxs-lookup"><span data-stu-id="e3f8f-115">Location IDs excluded from scope of policy.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3f8f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3f8f-116">JSON representation</span></span>

<span data-ttu-id="e3f8f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3f8f-117">The following is a JSON representation of the resource.</span></span>

## <a name="relationships"></a><span data-ttu-id="e3f8f-118">关系</span><span class="sxs-lookup"><span data-stu-id="e3f8f-118">Relationships</span></span>

<span data-ttu-id="e3f8f-119">无。</span><span class="sxs-lookup"><span data-stu-id="e3f8f-119">None.</span></span>

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
