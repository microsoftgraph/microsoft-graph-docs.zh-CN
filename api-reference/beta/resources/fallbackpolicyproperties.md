---
title: fallbackPolicyProperties 资源类型
description: '允许在 iOS 终结点上为高优先级原始通知指定回退策略，使用其他属性指定回退等待时间 (延迟) 和相应的视觉通知内容。 '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: ee32b40f71c2540bb06b8b4478d0f896aac40b85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071206"
---
# <a name="fallbackpolicyproperties-resource-type"></a><span data-ttu-id="18a6f-103">fallbackPolicyProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="18a6f-103">fallbackPolicyProperties resource type</span></span>

<span data-ttu-id="18a6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18a6f-105">允许在 iOS 终结点上为高优先级原始通知指定回退策略，使用其他属性指定回退等待时间 (延迟) 和相应的视觉通知内容。</span><span class="sxs-lookup"><span data-stu-id="18a6f-105">Allows fallback policy to be specified for high-priority raw notifications on iOS endpoints only, with additional properties for specifying fallback wait time (delay) and corresponding visual notification content.</span></span> 

## <a name="properties"></a><span data-ttu-id="18a6f-106">属性</span><span class="sxs-lookup"><span data-stu-id="18a6f-106">Properties</span></span>

| <span data-ttu-id="18a6f-107">属性</span><span class="sxs-lookup"><span data-stu-id="18a6f-107">Property</span></span>     | <span data-ttu-id="18a6f-108">类型</span><span class="sxs-lookup"><span data-stu-id="18a6f-108">Type</span></span>        | <span data-ttu-id="18a6f-109">说明</span><span class="sxs-lookup"><span data-stu-id="18a6f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="18a6f-110">platformTypes</span><span class="sxs-lookup"><span data-stu-id="18a6f-110">platformTypes</span></span> | <span data-ttu-id="18a6f-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="18a6f-111">String collection</span></span> | <span data-ttu-id="18a6f-112">指定开发人员想要对其启用原始 toast 通知回退的平台。</span><span class="sxs-lookup"><span data-stu-id="18a6f-112">Specifies the platforms that a developer wants to enable raw-to-visual toast notification fallback on.</span></span> <span data-ttu-id="18a6f-113">目前，如果指定了 **fallbackPolicy** ，则 **targetPolicy** 必须包含 `iOS` 和可选的其他平台。</span><span class="sxs-lookup"><span data-stu-id="18a6f-113">Currently, if **fallbackPolicy** is specified, **targetPolicy.platformTypes** must include `iOS` and optionally other platforms.</span></span> <span data-ttu-id="18a6f-114">此外，FallbackPolicy 是必需的，并且当前仅支持 **platformTypes** 平台 `iOS` 。</span><span class="sxs-lookup"><span data-stu-id="18a6f-114">In addition, **fallbackPolicy.endpointFallback.platformTypes** is required and the only supported platform is currently `iOS`.</span></span> |
| <span data-ttu-id="18a6f-115">fallbackDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="18a6f-115">fallbackDelayInSeconds</span></span> | <span data-ttu-id="18a6f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="18a6f-116">Int32</span></span> | <span data-ttu-id="18a6f-117">此延迟表示在将直接 toast 通知发送到不提取原始通知的每个用户 iOS 设备订阅之前，将 (以秒为单位的时间) 的时间量。</span><span class="sxs-lookup"><span data-stu-id="18a6f-117">This delay represents the amount of time that will pass (in seconds) before a direct toast notification will be sent as a fallback to each users� iOS device subscription that does not fetch the raw notification.</span></span> <span data-ttu-id="18a6f-118">该值必须介于60和600之间。</span><span class="sxs-lookup"><span data-stu-id="18a6f-118">The value must be between 60 and 600.</span></span> |
| <span data-ttu-id="18a6f-119">visualContent</span><span class="sxs-lookup"><span data-stu-id="18a6f-119">visualContent</span></span> | [<span data-ttu-id="18a6f-120">visualProperties</span><span class="sxs-lookup"><span data-stu-id="18a6f-120">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="18a6f-121">在 iOS 上回退启动的原始到可视用户通知的可视内容。</span><span class="sxs-lookup"><span data-stu-id="18a6f-121">The visual content of a fallback initiated, raw-to-visual user notification on iOS.</span></span> |
 


## <a name="json-representation"></a><span data-ttu-id="18a6f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18a6f-122">JSON representation</span></span>

<span data-ttu-id="18a6f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18a6f-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicyProperties",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"],
  "fallbackDelayInSeconds": 60,
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicyProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

