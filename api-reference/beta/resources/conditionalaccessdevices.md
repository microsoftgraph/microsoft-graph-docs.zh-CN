---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cbb542420228a4a383dea4e165323fbb6e8abb17
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082354"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="0a5bb-103">conditionalAccessDevices 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a5bb-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="0a5bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a5bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a5bb-105">表示策略作用域中的设备。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="0a5bb-106">属性</span><span class="sxs-lookup"><span data-stu-id="0a5bb-106">Properties</span></span>

| <span data-ttu-id="0a5bb-107">属性</span><span class="sxs-lookup"><span data-stu-id="0a5bb-107">Property</span></span>     | <span data-ttu-id="0a5bb-108">类型</span><span class="sxs-lookup"><span data-stu-id="0a5bb-108">Type</span></span>        | <span data-ttu-id="0a5bb-109">说明</span><span class="sxs-lookup"><span data-stu-id="0a5bb-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0a5bb-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="0a5bb-110">includeDevices</span></span> | <span data-ttu-id="0a5bb-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="0a5bb-111">String collection</span></span> | <span data-ttu-id="0a5bb-112">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-112">States in the scope of the policy.</span></span> <span data-ttu-id="0a5bb-113">`All` 是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-113">`All` is the only allowed value.</span></span> <span data-ttu-id="0a5bb-114">如果设置了 *deviceFIlter，则不能* 设置。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-114">Cannot be set if *deviceFIlter* is set.</span></span> |
| <span data-ttu-id="0a5bb-115">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="0a5bb-115">excludeDevices</span></span> | <span data-ttu-id="0a5bb-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="0a5bb-116">String collection</span></span> | <span data-ttu-id="0a5bb-117">策略作用域中排除的州。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-117">States excluded from the scope of the policy.</span></span> <span data-ttu-id="0a5bb-118">可能的值 `Compliant` `DomainJoined` ：、。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-118">Possible values: `Compliant`, `DomainJoined`.</span></span> <span data-ttu-id="0a5bb-119">如果设置了 **deviceFIlter，则不能** 设置。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-119">Cannot be set if **deviceFIlter** is set.</span></span> |
| <span data-ttu-id="0a5bb-120">deviceFilter</span><span class="sxs-lookup"><span data-stu-id="0a5bb-120">deviceFilter</span></span> | [<span data-ttu-id="0a5bb-121">conditionalAccessFilter</span><span class="sxs-lookup"><span data-stu-id="0a5bb-121">conditionalAccessFilter</span></span>](conditionalaccessfilter.md) | <span data-ttu-id="0a5bb-122">定义要包含/排除设备的动态设备语法规则的筛选器。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-122">Filter defining the dynamic-device-syntax rule to include/exclude devices.</span></span> <span data-ttu-id="0a5bb-123">筛选器可以使用设备属性 (例如扩展属性) /排除它们。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-123">A filter can use device properties (such as extension attributes) to include/exclude them.</span></span> <span data-ttu-id="0a5bb-124">如果设置了 **includeDevices** 或 **excludeDevices，则不能** 设置。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-124">Cannot be set if **includeDevices** or **excludeDevices** is set.</span></span> |
| <span data-ttu-id="0a5bb-125">includeDeviceStates (弃) </span><span class="sxs-lookup"><span data-stu-id="0a5bb-125">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="0a5bb-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="0a5bb-126">String collection</span></span> | <span data-ttu-id="0a5bb-127">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-127">States in the scope of the policy.</span></span> <span data-ttu-id="0a5bb-128">`All` 是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-128">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="0a5bb-129">excludeDeviceStates (弃) </span><span class="sxs-lookup"><span data-stu-id="0a5bb-129">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="0a5bb-130">String 集合</span><span class="sxs-lookup"><span data-stu-id="0a5bb-130">String collection</span></span> | <span data-ttu-id="0a5bb-131">策略作用域中排除的州。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-131">States excluded from the scope of the policy.</span></span> <span data-ttu-id="0a5bb-132">可能的值 `Compliant` `DomainJoined` ：、。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-132">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0a5bb-133">关系</span><span class="sxs-lookup"><span data-stu-id="0a5bb-133">Relationships</span></span>

<span data-ttu-id="0a5bb-134">无。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a5bb-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a5bb-135">JSON representation</span></span>

<span data-ttu-id="0a5bb-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a5bb-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices",
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ],
  "deviceFilter": {"@odata.type": "microsoft.graph.conditionalAccessFilter"}
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


