---
title: printOperationStatus 资源类型
description: 表示长时间运行的通用打印操作的当前状态。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 787a584b32c6f34d78d14fa4d676b1be30a62c25
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516991"
---
# <a name="printoperationstatus-resource-type"></a><span data-ttu-id="981ae-103">printOperationStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="981ae-103">printOperationStatus resource type</span></span>

<span data-ttu-id="981ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="981ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="981ae-105">表示长时间运行的通用打印操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="981ae-105">Represents the current status of a long-running Universal Print operation.</span></span>

## <a name="properties"></a><span data-ttu-id="981ae-106">属性</span><span class="sxs-lookup"><span data-stu-id="981ae-106">Properties</span></span>
|<span data-ttu-id="981ae-107">属性</span><span class="sxs-lookup"><span data-stu-id="981ae-107">Property</span></span>|<span data-ttu-id="981ae-108">类型</span><span class="sxs-lookup"><span data-stu-id="981ae-108">Type</span></span>|<span data-ttu-id="981ae-109">Description</span><span class="sxs-lookup"><span data-stu-id="981ae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="981ae-110">state</span><span class="sxs-lookup"><span data-stu-id="981ae-110">state</span></span>|<span data-ttu-id="981ae-111">printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="981ae-111">printOperationProcessingState</span></span>|<span data-ttu-id="981ae-112">printOperation 的当前处理状态。</span><span class="sxs-lookup"><span data-stu-id="981ae-112">The printOperation's current processing state.</span></span> <span data-ttu-id="981ae-113">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="981ae-113">Valid values are described in the following table.</span></span> <span data-ttu-id="981ae-114">只读。</span><span class="sxs-lookup"><span data-stu-id="981ae-114">Read-only.</span></span>|
|<span data-ttu-id="981ae-115">说明</span><span class="sxs-lookup"><span data-stu-id="981ae-115">description</span></span>|<span data-ttu-id="981ae-116">String</span><span class="sxs-lookup"><span data-stu-id="981ae-116">String</span></span>|<span data-ttu-id="981ae-117">可读的 printOperation 当前处理状态的说明。</span><span class="sxs-lookup"><span data-stu-id="981ae-117">A human-readable description of the printOperation's current processing state.</span></span> <span data-ttu-id="981ae-118">只读。</span><span class="sxs-lookup"><span data-stu-id="981ae-118">Read-only.</span></span>|

### <a name="printoperationprocessingstate-values"></a><span data-ttu-id="981ae-119">printOperationProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="981ae-119">printOperationProcessingState values</span></span>

|<span data-ttu-id="981ae-120">成员</span><span class="sxs-lookup"><span data-stu-id="981ae-120">Member</span></span>|<span data-ttu-id="981ae-121">值</span><span class="sxs-lookup"><span data-stu-id="981ae-121">Value</span></span>|<span data-ttu-id="981ae-122">Description</span><span class="sxs-lookup"><span data-stu-id="981ae-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="981ae-123">notStarted</span><span class="sxs-lookup"><span data-stu-id="981ae-123">notStarted</span></span>|<span data-ttu-id="981ae-124">0</span><span class="sxs-lookup"><span data-stu-id="981ae-124">0</span></span>|<span data-ttu-id="981ae-125">操作尚未启动。</span><span class="sxs-lookup"><span data-stu-id="981ae-125">The operation has not yet started.</span></span>|
|<span data-ttu-id="981ae-126">正在运行</span><span class="sxs-lookup"><span data-stu-id="981ae-126">running</span></span>|<span data-ttu-id="981ae-127">1 </span><span class="sxs-lookup"><span data-stu-id="981ae-127">1</span></span>|<span data-ttu-id="981ae-128">操作正在运行。</span><span class="sxs-lookup"><span data-stu-id="981ae-128">The operation is running.</span></span>|
|<span data-ttu-id="981ae-129">succeeded</span><span class="sxs-lookup"><span data-stu-id="981ae-129">succeeded</span></span>|<span data-ttu-id="981ae-130">2 </span><span class="sxs-lookup"><span data-stu-id="981ae-130">2</span></span>|<span data-ttu-id="981ae-131">操作成功完成。</span><span class="sxs-lookup"><span data-stu-id="981ae-131">The operation completed successfully.</span></span>|
|<span data-ttu-id="981ae-132">failed</span><span class="sxs-lookup"><span data-stu-id="981ae-132">failed</span></span>|<span data-ttu-id="981ae-133">3 </span><span class="sxs-lookup"><span data-stu-id="981ae-133">3</span></span>|<span data-ttu-id="981ae-134">操作失败。</span><span class="sxs-lookup"><span data-stu-id="981ae-134">The operation failed.</span></span>|
|<span data-ttu-id="981ae-135">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="981ae-135">unknownFutureValue</span></span>|<span data-ttu-id="981ae-136">4 </span><span class="sxs-lookup"><span data-stu-id="981ae-136">4</span></span>|<span data-ttu-id="981ae-137">可发展枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="981ae-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="981ae-138">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="981ae-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="981ae-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="981ae-139">JSON representation</span></span>
<span data-ttu-id="981ae-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="981ae-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printOperationStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperationStatus",
  "state": "String",
  "description": "String"
}
```

