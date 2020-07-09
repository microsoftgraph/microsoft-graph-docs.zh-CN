---
title: printTaskStatus 资源类型
description: 表示 printTask 的当前执行状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c5d46cd0c8d14b6dc07873bc503d024928e2b2e3
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091577"
---
# <a name="printtaskstatus-resource-type"></a><span data-ttu-id="cf70b-103">printTaskStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf70b-103">printTaskStatus resource type</span></span>

<span data-ttu-id="cf70b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf70b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf70b-105">表示[printTask](printtask.md)的当前执行状态。</span><span class="sxs-lookup"><span data-stu-id="cf70b-105">Represents the current execution status of a [printTask](printtask.md).</span></span> 

><span data-ttu-id="cf70b-106">**注意：** 注册任务触发器的应用程序负责在处理完成时更新任务状态，除非相关的打印作业已重定向到另一台打印机。</span><span class="sxs-lookup"><span data-stu-id="cf70b-106">**Note:** Applications that register task triggers are responsible for updating task statuses when processing is finished, unless the related print job has been redirected to another printer.</span></span>

<span data-ttu-id="cf70b-107">有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="cf70b-107">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="properties"></a><span data-ttu-id="cf70b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf70b-108">Properties</span></span>
| <span data-ttu-id="cf70b-109">属性</span><span class="sxs-lookup"><span data-stu-id="cf70b-109">Property</span></span>     | <span data-ttu-id="cf70b-110">类型</span><span class="sxs-lookup"><span data-stu-id="cf70b-110">Type</span></span>        | <span data-ttu-id="cf70b-111">说明</span><span class="sxs-lookup"><span data-stu-id="cf70b-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf70b-112">state</span><span class="sxs-lookup"><span data-stu-id="cf70b-112">state</span></span>|<span data-ttu-id="cf70b-113">printTaskProcessingState</span><span class="sxs-lookup"><span data-stu-id="cf70b-113">printTaskProcessingState</span></span>|<span data-ttu-id="cf70b-114">[PrintTask](printtask.md)的当前处理状态。</span><span class="sxs-lookup"><span data-stu-id="cf70b-114">The current processing state of the [printTask](printtask.md).</span></span> <span data-ttu-id="cf70b-115">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="cf70b-115">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="cf70b-116">description</span><span class="sxs-lookup"><span data-stu-id="cf70b-116">description</span></span>|<span data-ttu-id="cf70b-117">String</span><span class="sxs-lookup"><span data-stu-id="cf70b-117">String</span></span>|<span data-ttu-id="cf70b-118">[PrintTask](printtask.md)的当前处理状态的可读说明。</span><span class="sxs-lookup"><span data-stu-id="cf70b-118">A human-readable description of the current processing state of the [printTask](printtask.md).</span></span>|

### <a name="printtaskprocessingstate-values"></a><span data-ttu-id="cf70b-119">printTaskProcessingState 值</span><span class="sxs-lookup"><span data-stu-id="cf70b-119">printTaskProcessingState values</span></span>

|<span data-ttu-id="cf70b-120">成员</span><span class="sxs-lookup"><span data-stu-id="cf70b-120">Member</span></span>|<span data-ttu-id="cf70b-121">值</span><span class="sxs-lookup"><span data-stu-id="cf70b-121">Value</span></span>|<span data-ttu-id="cf70b-122">说明</span><span class="sxs-lookup"><span data-stu-id="cf70b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf70b-123">决</span><span class="sxs-lookup"><span data-stu-id="cf70b-123">pending</span></span>|<span data-ttu-id="cf70b-124">0</span><span class="sxs-lookup"><span data-stu-id="cf70b-124">0</span></span>|<span data-ttu-id="cf70b-125">任务执行挂起。</span><span class="sxs-lookup"><span data-stu-id="cf70b-125">Task execution is pending.</span></span>|
|<span data-ttu-id="cf70b-126">处理</span><span class="sxs-lookup"><span data-stu-id="cf70b-126">processing</span></span>|<span data-ttu-id="cf70b-127">1 </span><span class="sxs-lookup"><span data-stu-id="cf70b-127">1</span></span>|<span data-ttu-id="cf70b-128">正在执行任务。</span><span class="sxs-lookup"><span data-stu-id="cf70b-128">Task execution is in progress.</span></span>|
|<span data-ttu-id="cf70b-129">后</span><span class="sxs-lookup"><span data-stu-id="cf70b-129">completed</span></span>|<span data-ttu-id="cf70b-130">2 </span><span class="sxs-lookup"><span data-stu-id="cf70b-130">2</span></span>|<span data-ttu-id="cf70b-131">任务执行已完成。</span><span class="sxs-lookup"><span data-stu-id="cf70b-131">Task execution has completed.</span></span>|
|<span data-ttu-id="cf70b-132">其间</span><span class="sxs-lookup"><span data-stu-id="cf70b-132">aborted</span></span>|<span data-ttu-id="cf70b-133">3 </span><span class="sxs-lookup"><span data-stu-id="cf70b-133">3</span></span>|<span data-ttu-id="cf70b-134">任务执行已中止。</span><span class="sxs-lookup"><span data-stu-id="cf70b-134">Task execution was aborted.</span></span>|
|<span data-ttu-id="cf70b-135">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="cf70b-135">unknownFutureValue</span></span>|<span data-ttu-id="cf70b-136">4 </span><span class="sxs-lookup"><span data-stu-id="cf70b-136">4</span></span>|<span data-ttu-id="cf70b-137">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="cf70b-137">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="cf70b-138">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="cf70b-138">Do not use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf70b-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf70b-139">JSON representation</span></span>

<span data-ttu-id="cf70b-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf70b-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskStatus"
}-->

```json
{
  "state": {"@odata.type": "microsoft.graph.printTaskProcessingState"},
  "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
