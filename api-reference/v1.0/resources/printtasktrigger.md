---
title: printTaskTrigger 资源类型
description: 确定根据关联的 printTaskDefinition 执行新 printTask 的条件。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c0871f936b0935e6a599e79d6fb1a75f7e28f7ed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517264"
---
# <a name="printtasktrigger-resource-type"></a><span data-ttu-id="8513e-103">printTaskTrigger 资源类型</span><span class="sxs-lookup"><span data-stu-id="8513e-103">printTaskTrigger resource type</span></span>

<span data-ttu-id="8513e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8513e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8513e-105">确定根据关联的[printTaskDefinition](printtaskdefinition.md)触发新[printTask](printtask.md)的条件。</span><span class="sxs-lookup"><span data-stu-id="8513e-105">Determines the condition under which a new [printTask](printtask.md) will be triggered based on the associated [printTaskDefinition](printtaskdefinition.md).</span></span>

<span data-ttu-id="8513e-106">有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="8513e-106">For details about how to use this resource to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="methods"></a><span data-ttu-id="8513e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="8513e-107">Methods</span></span>
|<span data-ttu-id="8513e-108">方法</span><span class="sxs-lookup"><span data-stu-id="8513e-108">Method</span></span>|<span data-ttu-id="8513e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8513e-109">Return type</span></span>|<span data-ttu-id="8513e-110">Description</span><span class="sxs-lookup"><span data-stu-id="8513e-110">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="8513e-111">List</span><span class="sxs-lookup"><span data-stu-id="8513e-111">List</span></span>](../api/printer-list-tasktriggers.md) | <span data-ttu-id="8513e-112">[printTaskTrigger](printtasktrigger.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8513e-112">[printTaskTrigger](printtasktrigger.md) collection</span></span> | <span data-ttu-id="8513e-113">获取与特定打印机相关联的 printTaskTriggers [列表](printer.md)。</span><span class="sxs-lookup"><span data-stu-id="8513e-113">Get a list of printTaskTriggers associated with a particular [printer](printer.md).</span></span> |
| [<span data-ttu-id="8513e-114">获取</span><span class="sxs-lookup"><span data-stu-id="8513e-114">Get</span></span>](../api/printtasktrigger-get.md) | [<span data-ttu-id="8513e-115">printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="8513e-115">printTaskTrigger</span></span>](printtasktrigger.md) | <span data-ttu-id="8513e-116">获取与特定 printTask 关联的[printTaskTrigger。](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="8513e-116">Get the printTaskTrigger associated with a particular [printTask](printtask.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="8513e-117">属性</span><span class="sxs-lookup"><span data-stu-id="8513e-117">Properties</span></span>
|<span data-ttu-id="8513e-118">属性</span><span class="sxs-lookup"><span data-stu-id="8513e-118">Property</span></span>|<span data-ttu-id="8513e-119">类型</span><span class="sxs-lookup"><span data-stu-id="8513e-119">Type</span></span>|<span data-ttu-id="8513e-120">说明</span><span class="sxs-lookup"><span data-stu-id="8513e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8513e-121">id</span><span class="sxs-lookup"><span data-stu-id="8513e-121">id</span></span>|<span data-ttu-id="8513e-122">String</span><span class="sxs-lookup"><span data-stu-id="8513e-122">String</span></span>|<span data-ttu-id="8513e-123">printTaskTrigger 的标识符。</span><span class="sxs-lookup"><span data-stu-id="8513e-123">The printTaskTrigger's identifier.</span></span> <span data-ttu-id="8513e-124">只读。</span><span class="sxs-lookup"><span data-stu-id="8513e-124">Read-only.</span></span>|
|<span data-ttu-id="8513e-125">event</span><span class="sxs-lookup"><span data-stu-id="8513e-125">event</span></span>|<span data-ttu-id="8513e-126">printEvent</span><span class="sxs-lookup"><span data-stu-id="8513e-126">printEvent</span></span>|<span data-ttu-id="8513e-127">将导致触发新 [printTask](printtask.md) 的通用打印事件。</span><span class="sxs-lookup"><span data-stu-id="8513e-127">The Universal Print event that will cause a new [printTask](printtask.md) to be triggered.</span></span> <span data-ttu-id="8513e-128">下表介绍了有效值。</span><span class="sxs-lookup"><span data-stu-id="8513e-128">Valid values are described in the following table.</span></span>|

### <a name="printevent-values"></a><span data-ttu-id="8513e-129">printEvent 值</span><span class="sxs-lookup"><span data-stu-id="8513e-129">printEvent values</span></span>

|<span data-ttu-id="8513e-130">成员</span><span class="sxs-lookup"><span data-stu-id="8513e-130">Member</span></span>|<span data-ttu-id="8513e-131">值</span><span class="sxs-lookup"><span data-stu-id="8513e-131">Value</span></span>|<span data-ttu-id="8513e-132">Description</span><span class="sxs-lookup"><span data-stu-id="8513e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8513e-133">jobStarted</span><span class="sxs-lookup"><span data-stu-id="8513e-133">jobStarted</span></span>|<span data-ttu-id="8513e-134">0</span><span class="sxs-lookup"><span data-stu-id="8513e-134">0</span></span>|<span data-ttu-id="8513e-135">表示启动新打印作业时发生的事件。</span><span class="sxs-lookup"><span data-stu-id="8513e-135">Represents an event that occurs when a new print job is started.</span></span>|
|<span data-ttu-id="8513e-136">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="8513e-136">unknownFutureValue</span></span>|<span data-ttu-id="8513e-137">1 </span><span class="sxs-lookup"><span data-stu-id="8513e-137">1</span></span>|<span data-ttu-id="8513e-138">可发展枚举 sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="8513e-138">Evolvable enumeration sentinel value.</span></span> <span data-ttu-id="8513e-139">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="8513e-139">Do not use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8513e-140">关系</span><span class="sxs-lookup"><span data-stu-id="8513e-140">Relationships</span></span>
|<span data-ttu-id="8513e-141">关系</span><span class="sxs-lookup"><span data-stu-id="8513e-141">Relationship</span></span>|<span data-ttu-id="8513e-142">类型</span><span class="sxs-lookup"><span data-stu-id="8513e-142">Type</span></span>|<span data-ttu-id="8513e-143">Description</span><span class="sxs-lookup"><span data-stu-id="8513e-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8513e-144">definition</span><span class="sxs-lookup"><span data-stu-id="8513e-144">definition</span></span>|[<span data-ttu-id="8513e-145">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8513e-145">printTaskDefinition</span></span>](printtaskdefinition.md)|<span data-ttu-id="8513e-146">一个抽象定义，用于在打印事件触发时创建[printTask。](printtask.md)</span><span class="sxs-lookup"><span data-stu-id="8513e-146">An abstract definition that will be used to create a [printTask](printtask.md) when triggered by a print event.</span></span> <span data-ttu-id="8513e-147">只读。</span><span class="sxs-lookup"><span data-stu-id="8513e-147">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8513e-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8513e-148">JSON representation</span></span>
<span data-ttu-id="8513e-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8513e-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "id": "String (identifier)",
  "event": "String"
}
```

