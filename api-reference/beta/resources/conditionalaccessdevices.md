---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ada9dc6b9b9714941f4086d3ca49761fcbeb2ac
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805670"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="52e16-103">conditionalAccessDevices 资源类型</span><span class="sxs-lookup"><span data-stu-id="52e16-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="52e16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52e16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52e16-105">表示策略作用域中的设备。</span><span class="sxs-lookup"><span data-stu-id="52e16-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="52e16-106">属性</span><span class="sxs-lookup"><span data-stu-id="52e16-106">Properties</span></span>

| <span data-ttu-id="52e16-107">属性</span><span class="sxs-lookup"><span data-stu-id="52e16-107">Property</span></span>     | <span data-ttu-id="52e16-108">类型</span><span class="sxs-lookup"><span data-stu-id="52e16-108">Type</span></span>        | <span data-ttu-id="52e16-109">说明</span><span class="sxs-lookup"><span data-stu-id="52e16-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="52e16-110">includeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="52e16-110">includeDeviceStates</span></span> | <span data-ttu-id="52e16-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="52e16-111">String collection</span></span> | <span data-ttu-id="52e16-112">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="52e16-112">States in the scope of the policy.</span></span> <span data-ttu-id="52e16-113">`All`是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="52e16-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="52e16-114">excludeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="52e16-114">excludeDeviceStates</span></span> | <span data-ttu-id="52e16-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="52e16-115">String collection</span></span> | <span data-ttu-id="52e16-116">策略作用域中排除的状态。</span><span class="sxs-lookup"><span data-stu-id="52e16-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="52e16-117">可能的值`Compliant`： `DomainJoined`、。</span><span class="sxs-lookup"><span data-stu-id="52e16-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="52e16-118">关系</span><span class="sxs-lookup"><span data-stu-id="52e16-118">Relationships</span></span>

<span data-ttu-id="52e16-119">无。</span><span class="sxs-lookup"><span data-stu-id="52e16-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52e16-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52e16-120">JSON representation</span></span>

<span data-ttu-id="52e16-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52e16-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDeviceStates",
    "excludeDeviceStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDeviceStates": [ "String" ],
  "excludeDeviceStates": [ "String" ]
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
