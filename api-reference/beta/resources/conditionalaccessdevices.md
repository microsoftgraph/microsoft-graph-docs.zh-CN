---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 94115e97c597bc34f03d843b8098f707ed39cd51
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761805"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="23101-103">conditionalAccessDevices 资源类型</span><span class="sxs-lookup"><span data-stu-id="23101-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="23101-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23101-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23101-105">表示策略作用域中的设备。</span><span class="sxs-lookup"><span data-stu-id="23101-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="23101-106">属性</span><span class="sxs-lookup"><span data-stu-id="23101-106">Properties</span></span>

| <span data-ttu-id="23101-107">属性</span><span class="sxs-lookup"><span data-stu-id="23101-107">Property</span></span>     | <span data-ttu-id="23101-108">类型</span><span class="sxs-lookup"><span data-stu-id="23101-108">Type</span></span>        | <span data-ttu-id="23101-109">说明</span><span class="sxs-lookup"><span data-stu-id="23101-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="23101-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="23101-110">includeDevices</span></span> | <span data-ttu-id="23101-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="23101-111">String collection</span></span> | <span data-ttu-id="23101-112">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="23101-112">States in the scope of the policy.</span></span> <span data-ttu-id="23101-113">`All` 是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="23101-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="23101-114">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="23101-114">excludeDevices</span></span> | <span data-ttu-id="23101-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="23101-115">String collection</span></span> | <span data-ttu-id="23101-116">策略作用域中排除的州。</span><span class="sxs-lookup"><span data-stu-id="23101-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="23101-117">可能的值 `Compliant` `DomainJoined` ：、。</span><span class="sxs-lookup"><span data-stu-id="23101-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |
| <span data-ttu-id="23101-118">includeDeviceStates (弃) </span><span class="sxs-lookup"><span data-stu-id="23101-118">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="23101-119">字符串集合</span><span class="sxs-lookup"><span data-stu-id="23101-119">String collection</span></span> | <span data-ttu-id="23101-120">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="23101-120">States in the scope of the policy.</span></span> <span data-ttu-id="23101-121">`All` 是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="23101-121">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="23101-122">excludeDeviceStates (弃) </span><span class="sxs-lookup"><span data-stu-id="23101-122">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="23101-123">字符串集合</span><span class="sxs-lookup"><span data-stu-id="23101-123">String collection</span></span> | <span data-ttu-id="23101-124">策略作用域中排除的州。</span><span class="sxs-lookup"><span data-stu-id="23101-124">States excluded from the scope of the policy.</span></span> <span data-ttu-id="23101-125">可能的值 `Compliant` `DomainJoined` ：、。</span><span class="sxs-lookup"><span data-stu-id="23101-125">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="23101-126">关系</span><span class="sxs-lookup"><span data-stu-id="23101-126">Relationships</span></span>

<span data-ttu-id="23101-127">无。</span><span class="sxs-lookup"><span data-stu-id="23101-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23101-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23101-128">JSON representation</span></span>

<span data-ttu-id="23101-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23101-129">The following is a JSON representation of the resource.</span></span>

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


