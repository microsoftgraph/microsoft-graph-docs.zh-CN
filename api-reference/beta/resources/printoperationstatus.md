---
title: printOperationStatus 资源类型
description: 表示长时间运行的通用打印操作的当前状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a7400a3170b104646607c16852a796d01b64200e
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007185"
---
# <a name="printoperationstatus-complex-type"></a><span data-ttu-id="96650-103">printOperationStatus 复杂类型</span><span class="sxs-lookup"><span data-stu-id="96650-103">printOperationStatus complex type</span></span>

<span data-ttu-id="96650-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96650-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96650-105">表示长时间运行的通用打印操作的当前状态。</span><span class="sxs-lookup"><span data-stu-id="96650-105">Represents the current status of a long-running Universal Print operation.</span></span>

## <a name="properties"></a><span data-ttu-id="96650-106">属性</span><span class="sxs-lookup"><span data-stu-id="96650-106">Properties</span></span>
| <span data-ttu-id="96650-107">属性</span><span class="sxs-lookup"><span data-stu-id="96650-107">Property</span></span>     | <span data-ttu-id="96650-108">类型</span><span class="sxs-lookup"><span data-stu-id="96650-108">Type</span></span>        | <span data-ttu-id="96650-109">说明</span><span class="sxs-lookup"><span data-stu-id="96650-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96650-110">state</span><span class="sxs-lookup"><span data-stu-id="96650-110">state</span></span>|<span data-ttu-id="96650-111">printOperationProcessingState</span><span class="sxs-lookup"><span data-stu-id="96650-111">printOperationProcessingState</span></span>|<span data-ttu-id="96650-112">PrintOperation 的当前处理状态。</span><span class="sxs-lookup"><span data-stu-id="96650-112">The printOperation's current processing state.</span></span> <span data-ttu-id="96650-113">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="96650-113">Valid values are described in the following table.</span></span> <span data-ttu-id="96650-114">只读。</span><span class="sxs-lookup"><span data-stu-id="96650-114">Read-only.</span></span>|
|<span data-ttu-id="96650-115">说明</span><span class="sxs-lookup"><span data-stu-id="96650-115">description</span></span>|<span data-ttu-id="96650-116">String</span><span class="sxs-lookup"><span data-stu-id="96650-116">String</span></span>|<span data-ttu-id="96650-117">PrintOperation 的当前处理状态的可读说明。</span><span class="sxs-lookup"><span data-stu-id="96650-117">A human-readable description of the printOperation's current processing state.</span></span> <span data-ttu-id="96650-118">只读。</span><span class="sxs-lookup"><span data-stu-id="96650-118">Read-only.</span></span>|

### <a name="printoperationprocessingstate-values"></a><span data-ttu-id="96650-119">printOperationProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="96650-119">printOperationProcessingState values</span></span>

|<span data-ttu-id="96650-120">成员</span><span class="sxs-lookup"><span data-stu-id="96650-120">Member</span></span>|<span data-ttu-id="96650-121">值</span><span class="sxs-lookup"><span data-stu-id="96650-121">Value</span></span>|<span data-ttu-id="96650-122">说明</span><span class="sxs-lookup"><span data-stu-id="96650-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96650-123">notStarted</span><span class="sxs-lookup"><span data-stu-id="96650-123">notStarted</span></span>|<span data-ttu-id="96650-124">0</span><span class="sxs-lookup"><span data-stu-id="96650-124">0</span></span>|<span data-ttu-id="96650-125">该操作尚未启动。</span><span class="sxs-lookup"><span data-stu-id="96650-125">The operation has not yet started.</span></span>|
|<span data-ttu-id="96650-126">运行</span><span class="sxs-lookup"><span data-stu-id="96650-126">running</span></span>|<span data-ttu-id="96650-127">1 </span><span class="sxs-lookup"><span data-stu-id="96650-127">1</span></span>|<span data-ttu-id="96650-128">操作正在运行。</span><span class="sxs-lookup"><span data-stu-id="96650-128">The operation is running.</span></span>|
|<span data-ttu-id="96650-129">完成</span><span class="sxs-lookup"><span data-stu-id="96650-129">succeeded</span></span>|<span data-ttu-id="96650-130">2 </span><span class="sxs-lookup"><span data-stu-id="96650-130">2</span></span>|<span data-ttu-id="96650-131">操作已成功完成。</span><span class="sxs-lookup"><span data-stu-id="96650-131">The operation completed successfully.</span></span>|
|<span data-ttu-id="96650-132">未能</span><span class="sxs-lookup"><span data-stu-id="96650-132">failed</span></span>|<span data-ttu-id="96650-133">3 </span><span class="sxs-lookup"><span data-stu-id="96650-133">3</span></span>|<span data-ttu-id="96650-134">操作失败。</span><span class="sxs-lookup"><span data-stu-id="96650-134">The operation failed.</span></span>|
|<span data-ttu-id="96650-135">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="96650-135">unknownFutureValue</span></span>|<span data-ttu-id="96650-136">4 </span><span class="sxs-lookup"><span data-stu-id="96650-136">4</span></span>|<span data-ttu-id="96650-137">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="96650-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="96650-138">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="96650-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96650-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96650-139">JSON representation</span></span>

<span data-ttu-id="96650-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96650-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperationStatus"
}-->

```json
{
    "state": "String",
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->