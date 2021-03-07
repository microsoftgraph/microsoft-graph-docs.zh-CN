---
title: printTaskStatus 资源类型
description: 表示 printTask 的当前执行状态。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: ef5587050926fef5fa924f6d541de63d5b1d33aa
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517265"
---
# <a name="printtaskstatus-resource-type"></a><span data-ttu-id="ebe7d-103">printTaskStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebe7d-103">printTaskStatus resource type</span></span>

<span data-ttu-id="ebe7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebe7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="ebe7d-105">表示 [printTask 的当前执行状态](printtask.md)。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-105">Represents the current execution status of a [printTask](printtask.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="ebe7d-106">属性</span><span class="sxs-lookup"><span data-stu-id="ebe7d-106">Properties</span></span>
|<span data-ttu-id="ebe7d-107">属性</span><span class="sxs-lookup"><span data-stu-id="ebe7d-107">Property</span></span>|<span data-ttu-id="ebe7d-108">类型</span><span class="sxs-lookup"><span data-stu-id="ebe7d-108">Type</span></span>|<span data-ttu-id="ebe7d-109">Description</span><span class="sxs-lookup"><span data-stu-id="ebe7d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe7d-110">state</span><span class="sxs-lookup"><span data-stu-id="ebe7d-110">state</span></span>|<span data-ttu-id="ebe7d-111">printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="ebe7d-111">printTaskProcessingState</span></span>|<span data-ttu-id="ebe7d-112">[printTask 的当前处理状态](printtask.md)。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-112">The current processing state of the [printTask](printtask.md).</span></span> <span data-ttu-id="ebe7d-113">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-113">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="ebe7d-114">说明</span><span class="sxs-lookup"><span data-stu-id="ebe7d-114">description</span></span>|<span data-ttu-id="ebe7d-115">String</span><span class="sxs-lookup"><span data-stu-id="ebe7d-115">String</span></span>|<span data-ttu-id="ebe7d-116">打印 [Task](printtask.md)的当前处理状态的人读说明。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-116">A human-readable description of the current processing state of the [printTask](printtask.md).</span></span>|

### <a name="printtaskprocessingstate-values"></a><span data-ttu-id="ebe7d-117">printTaskProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="ebe7d-117">printTaskProcessingState values</span></span>

|<span data-ttu-id="ebe7d-118">成员</span><span class="sxs-lookup"><span data-stu-id="ebe7d-118">Member</span></span>|<span data-ttu-id="ebe7d-119">值</span><span class="sxs-lookup"><span data-stu-id="ebe7d-119">Value</span></span>|<span data-ttu-id="ebe7d-120">Description</span><span class="sxs-lookup"><span data-stu-id="ebe7d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebe7d-121">挂起</span><span class="sxs-lookup"><span data-stu-id="ebe7d-121">pending</span></span>|<span data-ttu-id="ebe7d-122">0</span><span class="sxs-lookup"><span data-stu-id="ebe7d-122">0</span></span>|<span data-ttu-id="ebe7d-123">任务执行挂起。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-123">Task execution is pending.</span></span>|
|<span data-ttu-id="ebe7d-124">processing</span><span class="sxs-lookup"><span data-stu-id="ebe7d-124">processing</span></span>|<span data-ttu-id="ebe7d-125">1 </span><span class="sxs-lookup"><span data-stu-id="ebe7d-125">1</span></span>|<span data-ttu-id="ebe7d-126">任务执行正在进行中。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-126">Task execution is in progress.</span></span>|
|<span data-ttu-id="ebe7d-127">已完成</span><span class="sxs-lookup"><span data-stu-id="ebe7d-127">completed</span></span>|<span data-ttu-id="ebe7d-128">2 </span><span class="sxs-lookup"><span data-stu-id="ebe7d-128">2</span></span>|<span data-ttu-id="ebe7d-129">任务执行已完成。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-129">Task execution has completed.</span></span>|
|<span data-ttu-id="ebe7d-130">已中止</span><span class="sxs-lookup"><span data-stu-id="ebe7d-130">aborted</span></span>|<span data-ttu-id="ebe7d-131">3 </span><span class="sxs-lookup"><span data-stu-id="ebe7d-131">3</span></span>|<span data-ttu-id="ebe7d-132">任务执行已中止。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-132">Task execution was aborted.</span></span>|
|<span data-ttu-id="ebe7d-133">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="ebe7d-133">unknownFutureValue</span></span>|<span data-ttu-id="ebe7d-134">4 </span><span class="sxs-lookup"><span data-stu-id="ebe7d-134">4</span></span>|<span data-ttu-id="ebe7d-135">可发展枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-135">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="ebe7d-136">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-136">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebe7d-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebe7d-137">JSON representation</span></span>
<span data-ttu-id="ebe7d-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebe7d-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printTaskStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskStatus",
  "state": "String",
  "description": "String"
}
```

