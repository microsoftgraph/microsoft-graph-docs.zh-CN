---
title: conditionalAccessDeviceStates 资源类型
description: 表示策略作用域中的设备状态。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff61b1d9713a0da322d01e3c302ebefc98dbee46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507553"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="5187f-103">conditionalAccessDeviceStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="5187f-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="5187f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5187f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5187f-105">表示策略作用域中的设备状态。</span><span class="sxs-lookup"><span data-stu-id="5187f-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="5187f-106">属性</span><span class="sxs-lookup"><span data-stu-id="5187f-106">Properties</span></span>

| <span data-ttu-id="5187f-107">属性</span><span class="sxs-lookup"><span data-stu-id="5187f-107">Property</span></span>     | <span data-ttu-id="5187f-108">类型</span><span class="sxs-lookup"><span data-stu-id="5187f-108">Type</span></span>        | <span data-ttu-id="5187f-109">说明</span><span class="sxs-lookup"><span data-stu-id="5187f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5187f-110">includeStates</span><span class="sxs-lookup"><span data-stu-id="5187f-110">includeStates</span></span> | <span data-ttu-id="5187f-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="5187f-111">String collection</span></span> | <span data-ttu-id="5187f-112">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="5187f-112">States in the scope of the policy.</span></span> <span data-ttu-id="5187f-113">`All`是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="5187f-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="5187f-114">excludeStates</span><span class="sxs-lookup"><span data-stu-id="5187f-114">excludeStates</span></span> | <span data-ttu-id="5187f-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="5187f-115">String collection</span></span> | <span data-ttu-id="5187f-116">策略作用域中排除的状态。</span><span class="sxs-lookup"><span data-stu-id="5187f-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="5187f-117">可能的值`Compliant`： `DomainJoined`、。</span><span class="sxs-lookup"><span data-stu-id="5187f-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5187f-118">关系</span><span class="sxs-lookup"><span data-stu-id="5187f-118">Relationships</span></span>

<span data-ttu-id="5187f-119">无。</span><span class="sxs-lookup"><span data-stu-id="5187f-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5187f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5187f-120">JSON representation</span></span>

<span data-ttu-id="5187f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5187f-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeStates",
    "excludeStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDeviceStates",
  "baseType": null
}-->

```json
{
  "includeStates": [ "String" ],
  "excludeStates": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDeviceStates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->