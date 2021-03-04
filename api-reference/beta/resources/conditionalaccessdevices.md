---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a42e6023ace493c5efb230ffd53eb9c4caee7d16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440526"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="b782b-103">conditionalAccessDevices 资源类型</span><span class="sxs-lookup"><span data-stu-id="b782b-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="b782b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b782b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b782b-105">表示策略作用域中的设备。</span><span class="sxs-lookup"><span data-stu-id="b782b-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="b782b-106">属性</span><span class="sxs-lookup"><span data-stu-id="b782b-106">Properties</span></span>

| <span data-ttu-id="b782b-107">属性</span><span class="sxs-lookup"><span data-stu-id="b782b-107">Property</span></span>     | <span data-ttu-id="b782b-108">类型</span><span class="sxs-lookup"><span data-stu-id="b782b-108">Type</span></span>        | <span data-ttu-id="b782b-109">说明</span><span class="sxs-lookup"><span data-stu-id="b782b-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b782b-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="b782b-110">includeDevices</span></span> | <span data-ttu-id="b782b-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b782b-111">String collection</span></span> | <span data-ttu-id="b782b-112">策略范围内状态。</span><span class="sxs-lookup"><span data-stu-id="b782b-112">States in the scope of the policy.</span></span> <span data-ttu-id="b782b-113">`All` 是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="b782b-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="b782b-114">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="b782b-114">excludeDevices</span></span> | <span data-ttu-id="b782b-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b782b-115">String collection</span></span> | <span data-ttu-id="b782b-116">策略作用域中排除的国家/省/市/</span><span class="sxs-lookup"><span data-stu-id="b782b-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="b782b-117">可能的值： `Compliant` `DomainJoined` ， 。</span><span class="sxs-lookup"><span data-stu-id="b782b-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |
| <span data-ttu-id="b782b-118">includeDeviceStates (弃) </span><span class="sxs-lookup"><span data-stu-id="b782b-118">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="b782b-119">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b782b-119">String collection</span></span> | <span data-ttu-id="b782b-120">策略范围内状态。</span><span class="sxs-lookup"><span data-stu-id="b782b-120">States in the scope of the policy.</span></span> <span data-ttu-id="b782b-121">`All` 是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="b782b-121">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="b782b-122">excludeDeviceStates (已弃) </span><span class="sxs-lookup"><span data-stu-id="b782b-122">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="b782b-123">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b782b-123">String collection</span></span> | <span data-ttu-id="b782b-124">策略作用域中排除的国家/省/市/</span><span class="sxs-lookup"><span data-stu-id="b782b-124">States excluded from the scope of the policy.</span></span> <span data-ttu-id="b782b-125">可能的值： `Compliant` `DomainJoined` ， 。</span><span class="sxs-lookup"><span data-stu-id="b782b-125">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b782b-126">关系</span><span class="sxs-lookup"><span data-stu-id="b782b-126">Relationships</span></span>

<span data-ttu-id="b782b-127">无。</span><span class="sxs-lookup"><span data-stu-id="b782b-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b782b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b782b-128">JSON representation</span></span>

<span data-ttu-id="b782b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b782b-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDevices resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


