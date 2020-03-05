---
title: fallbackPolicyProperties 资源类型
description: '允许在 iOS 终结点上为高优先级原始通知指定回退策略，其中包含用于指定回退等待时间（延迟）和相应的视觉通知内容的附加属性。 '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 3922fc08bf30dde7daa7e01d1f810cb3e45d5d81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498537"
---
# <a name="fallbackpolicyproperties-resource-type"></a><span data-ttu-id="ba3e3-103">fallbackPolicyProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba3e3-103">fallbackPolicyProperties resource type</span></span>

<span data-ttu-id="ba3e3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ba3e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba3e3-105">允许在 iOS 终结点上为高优先级原始通知指定回退策略，其中包含用于指定回退等待时间（延迟）和相应的视觉通知内容的附加属性。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-105">Allows fallback policy to be specified for high-priority raw notifications on iOS endpoints only, with additional properties for specifying fallback wait time (delay) and corresponding visual notification content.</span></span> 

## <a name="properties"></a><span data-ttu-id="ba3e3-106">属性</span><span class="sxs-lookup"><span data-stu-id="ba3e3-106">Properties</span></span>

| <span data-ttu-id="ba3e3-107">属性</span><span class="sxs-lookup"><span data-stu-id="ba3e3-107">Property</span></span>     | <span data-ttu-id="ba3e3-108">类型</span><span class="sxs-lookup"><span data-stu-id="ba3e3-108">Type</span></span>        | <span data-ttu-id="ba3e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="ba3e3-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ba3e3-110">platformTypes</span><span class="sxs-lookup"><span data-stu-id="ba3e3-110">platformTypes</span></span> | <span data-ttu-id="ba3e3-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="ba3e3-111">String collection</span></span> | <span data-ttu-id="ba3e3-112">指定开发人员想要对其启用原始 toast 通知回退的平台。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-112">Specifies the platforms that a developer wants to enable raw-to-visual toast notification fallback on.</span></span> <span data-ttu-id="ba3e3-113">目前，如果指定了**fallbackPolicy** ，则**targetPolicy**必须包含`iOS`和可选的其他平台。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-113">Currently, if **fallbackPolicy** is specified, **targetPolicy.platformTypes** must include `iOS` and optionally other platforms.</span></span> <span data-ttu-id="ba3e3-114">此外， **fallbackPolicy**是必需的，并且当前`iOS`仅支持 platformTypes 平台。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-114">In addition, **fallbackPolicy.endpointFallback.platformTypes** is required and the only supported platform is currently `iOS`.</span></span> |
| <span data-ttu-id="ba3e3-115">fallbackDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="ba3e3-115">fallbackDelayInSeconds</span></span> | <span data-ttu-id="ba3e3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ba3e3-116">Int32</span></span> | <span data-ttu-id="ba3e3-117">此延迟表示将直接 toast 通知发送到不提取原始通知的每个用户 iOS 设备订阅之前传递的时间量（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-117">This delay represents the amount of time that will pass (in seconds) before a direct toast notification will be sent as a fallback to each users� iOS device subscription that does not fetch the raw notification.</span></span> <span data-ttu-id="ba3e3-118">该值必须介于60和600之间。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-118">The value must be between 60 and 600.</span></span> |
| <span data-ttu-id="ba3e3-119">visualContent</span><span class="sxs-lookup"><span data-stu-id="ba3e3-119">visualContent</span></span> | [<span data-ttu-id="ba3e3-120">visualProperties</span><span class="sxs-lookup"><span data-stu-id="ba3e3-120">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="ba3e3-121">在 iOS 上回退启动的原始到可视用户通知的可视内容。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-121">The visual content of a fallback initiated, raw-to-visual user notification on iOS.</span></span> |
 


## <a name="json-representation"></a><span data-ttu-id="ba3e3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba3e3-122">JSON representation</span></span>

<span data-ttu-id="ba3e3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba3e3-123">The following is a JSON representation of the resource.</span></span>

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