---
title: monitoringRule 资源类型
description: 定义要监视的信号和阈值的规则，以及满足时要执行的操作。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 305db31c935329574a2b7d52403dc7664ff53f66
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067855"
---
# <a name="monitoringrule-resource-type"></a><span data-ttu-id="f05c6-103">monitoringRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f05c6-103">monitoringRule resource type</span></span>

<span data-ttu-id="f05c6-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="f05c6-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f05c6-105">定义要监视的信号和阈值的规则，以及满足时要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="f05c6-105">Rule defining a signal and threshold to monitor, and the action to perform when met.</span></span>

## <a name="properties"></a><span data-ttu-id="f05c6-106">属性</span><span class="sxs-lookup"><span data-stu-id="f05c6-106">Properties</span></span>
|<span data-ttu-id="f05c6-107">属性</span><span class="sxs-lookup"><span data-stu-id="f05c6-107">Property</span></span>|<span data-ttu-id="f05c6-108">类型</span><span class="sxs-lookup"><span data-stu-id="f05c6-108">Type</span></span>|<span data-ttu-id="f05c6-109">说明</span><span class="sxs-lookup"><span data-stu-id="f05c6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f05c6-110">action</span><span class="sxs-lookup"><span data-stu-id="f05c6-110">action</span></span>|<span data-ttu-id="f05c6-111">microsoft.graph.windowsUpdates.monitoringAction</span><span class="sxs-lookup"><span data-stu-id="f05c6-111">microsoft.graph.windowsUpdates.monitoringAction</span></span>|    <span data-ttu-id="f05c6-112">达到给定信号的阈值时触发的操作。</span><span class="sxs-lookup"><span data-stu-id="f05c6-112">The action triggered when the threshold for the given signal is met.</span></span> <span data-ttu-id="f05c6-113">可取值为：`alertError`、`pauseDeployment`。</span><span class="sxs-lookup"><span data-stu-id="f05c6-113">Possible values are: `alertError`, `pauseDeployment`.</span></span>|
|<span data-ttu-id="f05c6-114">signal</span><span class="sxs-lookup"><span data-stu-id="f05c6-114">signal</span></span>|<span data-ttu-id="f05c6-115">microsoft.graph.windowsUpdates.monitoringSignal</span><span class="sxs-lookup"><span data-stu-id="f05c6-115">microsoft.graph.windowsUpdates.monitoringSignal</span></span>|<span data-ttu-id="f05c6-116">要监视的信号。</span><span class="sxs-lookup"><span data-stu-id="f05c6-116">The signal to monitor.</span></span> <span data-ttu-id="f05c6-117">可能的值是 `rollback` ：。</span><span class="sxs-lookup"><span data-stu-id="f05c6-117">Possible values are: `rollback`.</span></span>|
|<span data-ttu-id="f05c6-118">阈值</span><span class="sxs-lookup"><span data-stu-id="f05c6-118">threshold</span></span>|<span data-ttu-id="f05c6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f05c6-119">Int32</span></span>|<span data-ttu-id="f05c6-120">要触发操作的信号的阈值。</span><span class="sxs-lookup"><span data-stu-id="f05c6-120">The threshold for a signal at which to trigger action.</span></span> <span data-ttu-id="f05c6-121">从 1 到 100 的整数 (包含) 。</span><span class="sxs-lookup"><span data-stu-id="f05c6-121">An integer from 1 to 100 (inclusive).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f05c6-122">关系</span><span class="sxs-lookup"><span data-stu-id="f05c6-122">Relationships</span></span>
<span data-ttu-id="f05c6-123">无。</span><span class="sxs-lookup"><span data-stu-id="f05c6-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f05c6-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f05c6-124">JSON representation</span></span>
<span data-ttu-id="f05c6-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f05c6-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
  "signal": "String",
  "threshold": "Integer",
  "action": "String"
}
```

