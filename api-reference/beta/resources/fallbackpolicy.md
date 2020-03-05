---
title: fallbackPolicy 资源类型
description: '仅允许为 iOS 终结点指定回退策略，并且该策略旨在用于高优先级原始通知。 '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 822a5d24acbec878b864c70d357f76a1fa115e4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498572"
---
# <a name="fallbackpolicy-resource-type"></a><span data-ttu-id="36d9a-103">fallbackPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="36d9a-103">fallbackPolicy resource type</span></span>

<span data-ttu-id="36d9a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="36d9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36d9a-105">仅允许为 iOS 终结点指定回退策略，该策略旨在用于由于特定于平台的限制而无法发送到设备的高优先级原始通知（例如，节电模式）。</span><span class="sxs-lookup"><span data-stu-id="36d9a-105">Allows fallback policy to be specified for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span>

## <a name="properties"></a><span data-ttu-id="36d9a-106">属性</span><span class="sxs-lookup"><span data-stu-id="36d9a-106">Properties</span></span>

| <span data-ttu-id="36d9a-107">属性</span><span class="sxs-lookup"><span data-stu-id="36d9a-107">Property</span></span>     | <span data-ttu-id="36d9a-108">类型</span><span class="sxs-lookup"><span data-stu-id="36d9a-108">Type</span></span>        | <span data-ttu-id="36d9a-109">说明</span><span class="sxs-lookup"><span data-stu-id="36d9a-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="36d9a-110">endpointFallback</span><span class="sxs-lookup"><span data-stu-id="36d9a-110">endpointFallback</span></span> | [<span data-ttu-id="36d9a-111">fallbackPolicyProperties</span><span class="sxs-lookup"><span data-stu-id="36d9a-111">fallbackPolicyProperties</span></span>](fallbackpolicyproperties.md) | <span data-ttu-id="36d9a-112">EndpointFallback 策略对象在终结点级别处理通知回退策略，目前限制为 iOS。</span><span class="sxs-lookup"><span data-stu-id="36d9a-112">EndpointFallback policy object handles notification fallback policy at an end point level and is currently limited to iOS.</span></span> |   


## <a name="json-representation"></a><span data-ttu-id="36d9a-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36d9a-113">JSON representation</span></span>

<span data-ttu-id="36d9a-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36d9a-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicy",
  "baseType": null
}-->

```json
{
  "endpointFallback": {"@odata.type": "microsoft.graph.fallbackpolicyProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
