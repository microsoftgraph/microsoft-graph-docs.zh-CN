---
title: deploymentState 资源类型
description: 描述和控制部署的当前状态。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d05bf09fbad405e93ee994858e2d6ac65a8088a7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067292"
---
# <a name="deploymentstate-resource-type"></a><span data-ttu-id="c00e5-103">deploymentState 资源类型</span><span class="sxs-lookup"><span data-stu-id="c00e5-103">deploymentState resource type</span></span>

<span data-ttu-id="c00e5-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c00e5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c00e5-105">描述和控制部署的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c00e5-105">Describes and controls the current state of a deployment.</span></span>

## <a name="properties"></a><span data-ttu-id="c00e5-106">属性</span><span class="sxs-lookup"><span data-stu-id="c00e5-106">Properties</span></span>
|<span data-ttu-id="c00e5-107">属性</span><span class="sxs-lookup"><span data-stu-id="c00e5-107">Property</span></span>|<span data-ttu-id="c00e5-108">类型</span><span class="sxs-lookup"><span data-stu-id="c00e5-108">Type</span></span>|<span data-ttu-id="c00e5-109">说明</span><span class="sxs-lookup"><span data-stu-id="c00e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c00e5-110">原因</span><span class="sxs-lookup"><span data-stu-id="c00e5-110">reasons</span></span>|<span data-ttu-id="c00e5-111">[microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c00e5-111">[microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md) collection</span></span>|<span data-ttu-id="c00e5-112">指定部署具有其状态值的原因。</span><span class="sxs-lookup"><span data-stu-id="c00e5-112">Specifies the reasons the deployment has its state value.</span></span> <span data-ttu-id="c00e5-113">只读。</span><span class="sxs-lookup"><span data-stu-id="c00e5-113">Read-only.</span></span>|
|<span data-ttu-id="c00e5-114">requestedValue</span><span class="sxs-lookup"><span data-stu-id="c00e5-114">requestedValue</span></span>|<span data-ttu-id="c00e5-115">microsoft.graph.windowsUpdates.requestedDeploymentStateValue</span><span class="sxs-lookup"><span data-stu-id="c00e5-115">microsoft.graph.windowsUpdates.requestedDeploymentStateValue</span></span>|<span data-ttu-id="c00e5-116">指定部署的请求状态。</span><span class="sxs-lookup"><span data-stu-id="c00e5-116">Specifies the requested state of the deployment.</span></span> <span data-ttu-id="c00e5-117">支持 **requestedDeploymentStateValue 值的子集**。</span><span class="sxs-lookup"><span data-stu-id="c00e5-117">Supports a subset of the values for **requestedDeploymentStateValue**.</span></span> <span data-ttu-id="c00e5-118">可取值为：`none`、`paused`。</span><span class="sxs-lookup"><span data-stu-id="c00e5-118">Possible values are: `none`, `paused`.</span></span>|
|<span data-ttu-id="c00e5-119">值</span><span class="sxs-lookup"><span data-stu-id="c00e5-119">value</span></span>|<span data-ttu-id="c00e5-120">microsoft.graph.windowsUpdates.deploymentStateValue</span><span class="sxs-lookup"><span data-stu-id="c00e5-120">microsoft.graph.windowsUpdates.deploymentStateValue</span></span>|<span data-ttu-id="c00e5-121">指定部署的状态。</span><span class="sxs-lookup"><span data-stu-id="c00e5-121">Specifies the state of the deployment.</span></span> <span data-ttu-id="c00e5-122">支持 **deploymentStateValue** 值的子集。</span><span class="sxs-lookup"><span data-stu-id="c00e5-122">Supports a subset of the values for **deploymentStateValue**.</span></span> <span data-ttu-id="c00e5-123">可取值为：`scheduled`、`offering`、`paused`。</span><span class="sxs-lookup"><span data-stu-id="c00e5-123">Possible values are: `scheduled`, `offering`, `paused`.</span></span> <span data-ttu-id="c00e5-124">只读。</span><span class="sxs-lookup"><span data-stu-id="c00e5-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c00e5-125">关系</span><span class="sxs-lookup"><span data-stu-id="c00e5-125">Relationships</span></span>
<span data-ttu-id="c00e5-126">无。</span><span class="sxs-lookup"><span data-stu-id="c00e5-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c00e5-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c00e5-127">JSON representation</span></span>
<span data-ttu-id="c00e5-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c00e5-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentState",
  "value": "String",
  "reasons": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
    }
  ],
  "requestedValue": "String",
}
```

