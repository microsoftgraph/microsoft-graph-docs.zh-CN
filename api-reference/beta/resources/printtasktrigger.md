---
title: printTaskTrigger 资源类型
description: 根据关联的 printTaskDefinition 确定将执行新 printTask 的条件。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0a9ca4d06f43c9dd0964f0bb4c9614bfb4a78c1e
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091575"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="4a27b-103">printTaskTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a27b-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="4a27b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a27b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a27b-105">确定根据关联的[printTaskDefinition](printtaskdefinition.md)触发新[printTask](printtask.md)时所依据的条件。</span><span class="sxs-lookup"><span data-stu-id="4a27b-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="4a27b-106">有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="4a27b-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="4a27b-107">方法</span><span class="sxs-lookup"><span data-stu-id="4a27b-107">Methods</span></span>

| <span data-ttu-id="4a27b-108">方法</span><span class="sxs-lookup"><span data-stu-id="4a27b-108">Method</span></span>       | <span data-ttu-id="4a27b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a27b-109">Return Type</span></span> | <span data-ttu-id="4a27b-110">Description</span><span class="sxs-lookup"><span data-stu-id="4a27b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4a27b-111">List</span><span class="sxs-lookup"><span data-stu-id="4a27b-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="4a27b-112">[printTaskTrigger](printtasktrigger.md)集合</span><span class="sxs-lookup"><span data-stu-id="4a27b-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="4a27b-113">获取与特定[打印机](printer.md)相关联的 printTaskTriggers 的列表。</span><span class="sxs-lookup"><span data-stu-id="4a27b-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="4a27b-114">获取</span><span class="sxs-lookup"><span data-stu-id="4a27b-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="4a27b-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="4a27b-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="4a27b-116">获取与特定[printTask](printtask.md)关联的 printTaskTrigger。</span><span class="sxs-lookup"><span data-stu-id="4a27b-116">Get the printTaskTrigger associated with a particular [printTask](printtask.md).</span></span> |


## <a name="properties"></a><span data-ttu-id="4a27b-117">属性</span><span class="sxs-lookup"><span data-stu-id="4a27b-117">Properties</span></span>
| <span data-ttu-id="4a27b-118">属性</span><span class="sxs-lookup"><span data-stu-id="4a27b-118">Property</span></span>     | <span data-ttu-id="4a27b-119">类型</span><span class="sxs-lookup"><span data-stu-id="4a27b-119">Type</span></span>        | <span data-ttu-id="4a27b-120">说明</span><span class="sxs-lookup"><span data-stu-id="4a27b-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a27b-121">id</span><span class="sxs-lookup"><span data-stu-id="4a27b-121">id</span></span>|<span data-ttu-id="4a27b-122">String</span><span class="sxs-lookup"><span data-stu-id="4a27b-122">String</span></span>|<span data-ttu-id="4a27b-123">PrintTaskTrigger 的标识符。</span><span class="sxs-lookup"><span data-stu-id="4a27b-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="4a27b-124">只读。</span><span class="sxs-lookup"><span data-stu-id="4a27b-124">Read-only.</span></span>|
|<span data-ttu-id="4a27b-125">event</span><span class="sxs-lookup"><span data-stu-id="4a27b-125">event</span></span>|<span data-ttu-id="4a27b-126">printEvent</span><span class="sxs-lookup"><span data-stu-id="4a27b-126">printEvent</span></span>|<span data-ttu-id="4a27b-127">将导致触发新[printTask](printtask.md)的通用打印事件。</span><span class="sxs-lookup"><span data-stu-id="4a27b-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="4a27b-128">有效值如下表所述。</span><span class="sxs-lookup"><span data-stu-id="4a27b-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="4a27b-129">printEvent 值</span><span class="sxs-lookup"><span data-stu-id="4a27b-129">printEvent values</span></span>

|<span data-ttu-id="4a27b-130">成员</span><span class="sxs-lookup"><span data-stu-id="4a27b-130">Member</span></span>|<span data-ttu-id="4a27b-131">值</span><span class="sxs-lookup"><span data-stu-id="4a27b-131">Value</span></span>|<span data-ttu-id="4a27b-132">说明</span><span class="sxs-lookup"><span data-stu-id="4a27b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a27b-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="4a27b-133">jobStarted</span></span>|<span data-ttu-id="4a27b-134">0</span><span class="sxs-lookup"><span data-stu-id="4a27b-134">0</span></span>|<span data-ttu-id="4a27b-135">表示启动新的打印作业时发生的事件。</span><span class="sxs-lookup"><span data-stu-id="4a27b-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="4a27b-136">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="4a27b-136">unknownFutureValue</span></span>|<span data-ttu-id="4a27b-137">1 </span><span class="sxs-lookup"><span data-stu-id="4a27b-137">1</span></span>|<span data-ttu-id="4a27b-138">Evolvable 枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="4a27b-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="4a27b-139">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="4a27b-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a27b-140">关系</span><span class="sxs-lookup"><span data-stu-id="4a27b-140">Relationships</span></span>
| <span data-ttu-id="4a27b-141">关系</span><span class="sxs-lookup"><span data-stu-id="4a27b-141">Relationship</span></span> | <span data-ttu-id="4a27b-142">类型</span><span class="sxs-lookup"><span data-stu-id="4a27b-142">Type</span></span>        | <span data-ttu-id="4a27b-143">说明</span><span class="sxs-lookup"><span data-stu-id="4a27b-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a27b-144">定义</span><span class="sxs-lookup"><span data-stu-id="4a27b-144">definition</span></span>|[<span data-ttu-id="4a27b-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="4a27b-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="4a27b-146">将用于创建[printTask](printtask.md)的抽象定义（由 print 事件触发时）。</span><span class="sxs-lookup"><span data-stu-id="4a27b-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="4a27b-147">只读。</span><span class="sxs-lookup"><span data-stu-id="4a27b-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a27b-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a27b-148">JSON representation</span></span>

<span data-ttu-id="4a27b-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a27b-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "event": {"@odata.type": "microsoft.graph.printEvent"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
