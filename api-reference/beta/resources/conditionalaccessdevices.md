---
title: conditionalAccessDevices 资源类型
description: 表示策略作用域中的设备。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f0610fb376b265a261b8a88ab4181dd89bb9f6c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040069"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="1ee83-103">conditionalAccessDevices 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ee83-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="1ee83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ee83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ee83-105">表示策略作用域中的设备。</span><span class="sxs-lookup"><span data-stu-id="1ee83-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="1ee83-106">属性</span><span class="sxs-lookup"><span data-stu-id="1ee83-106">Properties</span></span>

| <span data-ttu-id="1ee83-107">属性</span><span class="sxs-lookup"><span data-stu-id="1ee83-107">Property</span></span>     | <span data-ttu-id="1ee83-108">类型</span><span class="sxs-lookup"><span data-stu-id="1ee83-108">Type</span></span>        | <span data-ttu-id="1ee83-109">说明</span><span class="sxs-lookup"><span data-stu-id="1ee83-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1ee83-110">includeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="1ee83-110">includeDeviceStates</span></span> | <span data-ttu-id="1ee83-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="1ee83-111">String collection</span></span> | <span data-ttu-id="1ee83-112">策略作用域中的状态。</span><span class="sxs-lookup"><span data-stu-id="1ee83-112">States in the scope of the policy.</span></span> <span data-ttu-id="1ee83-113">`All` 是唯一允许的值。</span><span class="sxs-lookup"><span data-stu-id="1ee83-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="1ee83-114">excludeDeviceStates</span><span class="sxs-lookup"><span data-stu-id="1ee83-114">excludeDeviceStates</span></span> | <span data-ttu-id="1ee83-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="1ee83-115">String collection</span></span> | <span data-ttu-id="1ee83-116">策略作用域中排除的状态。</span><span class="sxs-lookup"><span data-stu-id="1ee83-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="1ee83-117">可能的值： `Compliant` 、 `DomainJoined` 。</span><span class="sxs-lookup"><span data-stu-id="1ee83-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1ee83-118">关系</span><span class="sxs-lookup"><span data-stu-id="1ee83-118">Relationships</span></span>

<span data-ttu-id="1ee83-119">无。</span><span class="sxs-lookup"><span data-stu-id="1ee83-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ee83-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ee83-120">JSON representation</span></span>

<span data-ttu-id="1ee83-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ee83-121">The following is a JSON representation of the resource.</span></span>

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


