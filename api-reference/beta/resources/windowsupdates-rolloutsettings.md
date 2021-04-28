---
title: rolloutSettings 资源类型
description: 设置控制服务如何随着时间的推移部署更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 705eeae189d9159c07d3c115c77383a207eae6db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067851"
---
# <a name="rolloutsettings-resource-type"></a><span data-ttu-id="3acbd-103">rolloutSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="3acbd-103">rolloutSettings resource type</span></span>

<span data-ttu-id="3acbd-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3acbd-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3acbd-105">设置控制服务如何随着时间的推移部署更新。</span><span class="sxs-lookup"><span data-stu-id="3acbd-105">Settings controlling how the service deploys an update over time.</span></span>

## <a name="properties"></a><span data-ttu-id="3acbd-106">属性</span><span class="sxs-lookup"><span data-stu-id="3acbd-106">Properties</span></span>
|<span data-ttu-id="3acbd-107">属性</span><span class="sxs-lookup"><span data-stu-id="3acbd-107">Property</span></span>|<span data-ttu-id="3acbd-108">类型</span><span class="sxs-lookup"><span data-stu-id="3acbd-108">Type</span></span>|<span data-ttu-id="3acbd-109">说明</span><span class="sxs-lookup"><span data-stu-id="3acbd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3acbd-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3acbd-110">startDateTime</span></span>|<span data-ttu-id="3acbd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acbd-111">DateTimeOffset</span></span>|<span data-ttu-id="3acbd-112">部署中的设备开始接收更新的日期。</span><span class="sxs-lookup"><span data-stu-id="3acbd-112">Date on which devices in the deployment start receiving the update.</span></span> <span data-ttu-id="3acbd-113">未设置时，一旦分配设备，部署就会开始。</span><span class="sxs-lookup"><span data-stu-id="3acbd-113">When not set, the deployment starts as soon as devices are assigned.</span></span>|
|<span data-ttu-id="3acbd-114">devicesPerOffer</span><span class="sxs-lookup"><span data-stu-id="3acbd-114">devicesPerOffer</span></span>|<span data-ttu-id="3acbd-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3acbd-115">Int32</span></span>| <span data-ttu-id="3acbd-116">指定同时提供的设备数。</span><span class="sxs-lookup"><span data-stu-id="3acbd-116">Specifies the number of devices that are offered at the same time.</span></span> <span data-ttu-id="3acbd-117">设置 **endDateTime 时** 不起作用。</span><span class="sxs-lookup"><span data-stu-id="3acbd-117">Has no effect when **endDateTime** is set.</span></span> <span data-ttu-id="3acbd-118">当 **未设置 endDateTime** 和 **devicesPerOffer** 时，将同时提供部署中所有设备的内容。</span><span class="sxs-lookup"><span data-stu-id="3acbd-118">When **endDateTime** and **devicesPerOffer** are both not set, all devices in the deployment are offered content at the same time.</span></span>|
|<span data-ttu-id="3acbd-119">durationBetweenOffers</span><span class="sxs-lookup"><span data-stu-id="3acbd-119">durationBetweenOffers</span></span>|<span data-ttu-id="3acbd-120">String</span><span class="sxs-lookup"><span data-stu-id="3acbd-120">String</span></span>|<span data-ttu-id="3acbd-121">指定提供更新的每组设备之间的持续时间。</span><span class="sxs-lookup"><span data-stu-id="3acbd-121">Specifies duration between each set of devices being offered the update.</span></span> <span data-ttu-id="3acbd-122">定义 **endDateTime 或** **devicesPerOffer 时** 有效。</span><span class="sxs-lookup"><span data-stu-id="3acbd-122">Has an effect when **endDateTime** or **devicesPerOffer** are defined.</span></span> <span data-ttu-id="3acbd-123">默认值为 (`P1D` 1 天) 。</span><span class="sxs-lookup"><span data-stu-id="3acbd-123">Default value is `P1D` (1 day).</span></span>|
|<span data-ttu-id="3acbd-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3acbd-124">endDateTime</span></span>|<span data-ttu-id="3acbd-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acbd-125">DateTimeOffset</span></span>|<span data-ttu-id="3acbd-126">指定向当前部署中所有设备提供更新的日期。</span><span class="sxs-lookup"><span data-stu-id="3acbd-126">Specifies the date before which all devices currently in the deployment are offered the update.</span></span> <span data-ttu-id="3acbd-127">在此日期之后添加的设备将立即提供。</span><span class="sxs-lookup"><span data-stu-id="3acbd-127">Devices added after this date are offered immediately.</span></span> <span data-ttu-id="3acbd-128">当 **未设置 endDateTime** 和 **devicesPerOffer** 时，将同时提供部署中所有设备的内容。</span><span class="sxs-lookup"><span data-stu-id="3acbd-128">When **endDateTime** and **devicesPerOffer** are both not set, all devices in the deployment are offered content at the same time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3acbd-129">关系</span><span class="sxs-lookup"><span data-stu-id="3acbd-129">Relationships</span></span>
<span data-ttu-id="3acbd-130">无。</span><span class="sxs-lookup"><span data-stu-id="3acbd-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3acbd-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3acbd-131">JSON representation</span></span>
<span data-ttu-id="3acbd-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3acbd-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.rolloutSettings",
  "startDateTime": "String",
  "durationBetweenOffers": "String",
  "endDateTime": "String (timestamp)",
  "devicesPerOffer": "Integer"
}
```

