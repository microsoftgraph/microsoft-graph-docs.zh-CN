---
title: printTaskTrigger 资源类型
description: 确定根据关联的 printTaskDefinition 执行新 printTask 的条件。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2da4f94894d9744fdfdd302b310251cd91fdb3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766320"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="26aa6-103">printTaskTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="26aa6-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="26aa6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26aa6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26aa6-105">确定根据关联的[printTaskDefinition](printtaskdefinition.md)触发新[printTask](printtask.md)的条件。</span><span class="sxs-lookup"><span data-stu-id="26aa6-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="26aa6-106">有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="26aa6-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="26aa6-107">方法</span><span class="sxs-lookup"><span data-stu-id="26aa6-107">Methods</span></span>

| <span data-ttu-id="26aa6-108">方法</span><span class="sxs-lookup"><span data-stu-id="26aa6-108">Method</span></span>       | <span data-ttu-id="26aa6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="26aa6-109">Return Type</span></span> | <span data-ttu-id="26aa6-110">Description</span><span class="sxs-lookup"><span data-stu-id="26aa6-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="26aa6-111">List</span><span class="sxs-lookup"><span data-stu-id="26aa6-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="26aa6-112">[printTaskTrigger](printtasktrigger.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26aa6-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="26aa6-113">获取与特定打印机相关联的 printTaskTriggers [列表](printer.md)。</span><span class="sxs-lookup"><span data-stu-id="26aa6-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="26aa6-114">Get</span><span class="sxs-lookup"><span data-stu-id="26aa6-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="26aa6-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="26aa6-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="26aa6-116">获取与特定打印机关联的特定 printTaskTrigger。 [](printer.md)</span><span class="sxs-lookup"><span data-stu-id="26aa6-116">Get a particular printTaskTrigger associated with a particular [printer](printer.md).</span></span>|


## <a name="properties"></a><span data-ttu-id="26aa6-117">属性</span><span class="sxs-lookup"><span data-stu-id="26aa6-117">Properties</span></span>
| <span data-ttu-id="26aa6-118">属性</span><span class="sxs-lookup"><span data-stu-id="26aa6-118">Property</span></span>     | <span data-ttu-id="26aa6-119">类型</span><span class="sxs-lookup"><span data-stu-id="26aa6-119">Type</span></span>        | <span data-ttu-id="26aa6-120">说明</span><span class="sxs-lookup"><span data-stu-id="26aa6-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26aa6-121">id</span><span class="sxs-lookup"><span data-stu-id="26aa6-121">id</span></span>|<span data-ttu-id="26aa6-122">String</span><span class="sxs-lookup"><span data-stu-id="26aa6-122">String</span></span>|<span data-ttu-id="26aa6-123">printTaskTrigger 的标识符。</span><span class="sxs-lookup"><span data-stu-id="26aa6-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="26aa6-124">只读。</span><span class="sxs-lookup"><span data-stu-id="26aa6-124">Read-only.</span></span>|
|<span data-ttu-id="26aa6-125">event</span><span class="sxs-lookup"><span data-stu-id="26aa6-125">event</span></span>|<span data-ttu-id="26aa6-126">printEvent</span><span class="sxs-lookup"><span data-stu-id="26aa6-126">printEvent</span></span>|<span data-ttu-id="26aa6-127">将导致触发新 [printTask](printtask.md) 的通用 Print 事件。</span><span class="sxs-lookup"><span data-stu-id="26aa6-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="26aa6-128">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="26aa6-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="26aa6-129">printEvent 值</span><span class="sxs-lookup"><span data-stu-id="26aa6-129">printEvent values</span></span>

|<span data-ttu-id="26aa6-130">成员</span><span class="sxs-lookup"><span data-stu-id="26aa6-130">Member</span></span>|<span data-ttu-id="26aa6-131">值</span><span class="sxs-lookup"><span data-stu-id="26aa6-131">Value</span></span>|<span data-ttu-id="26aa6-132">说明</span><span class="sxs-lookup"><span data-stu-id="26aa6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26aa6-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="26aa6-133">jobStarted</span></span>|<span data-ttu-id="26aa6-134">0</span><span class="sxs-lookup"><span data-stu-id="26aa6-134">0</span></span>|<span data-ttu-id="26aa6-135">表示启动新打印作业时发生的事件。</span><span class="sxs-lookup"><span data-stu-id="26aa6-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="26aa6-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="26aa6-136">unknownFutureValue</span></span>|<span data-ttu-id="26aa6-137">1</span><span class="sxs-lookup"><span data-stu-id="26aa6-137">1</span></span>|<span data-ttu-id="26aa6-138">可发展枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="26aa6-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="26aa6-139">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="26aa6-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26aa6-140">关系</span><span class="sxs-lookup"><span data-stu-id="26aa6-140">Relationships</span></span>
| <span data-ttu-id="26aa6-141">关系</span><span class="sxs-lookup"><span data-stu-id="26aa6-141">Relationship</span></span> | <span data-ttu-id="26aa6-142">类型</span><span class="sxs-lookup"><span data-stu-id="26aa6-142">Type</span></span>        | <span data-ttu-id="26aa6-143">说明</span><span class="sxs-lookup"><span data-stu-id="26aa6-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26aa6-144">definition</span><span class="sxs-lookup"><span data-stu-id="26aa6-144">definition</span></span>|[<span data-ttu-id="26aa6-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="26aa6-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="26aa6-146">一个抽象定义，用于在打印事件触发时创建[printTask。](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="26aa6-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="26aa6-147">只读。</span><span class="sxs-lookup"><span data-stu-id="26aa6-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26aa6-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26aa6-148">JSON representation</span></span>

<span data-ttu-id="26aa6-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26aa6-149">The following is a JSON representation of the resource.</span></span>

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


