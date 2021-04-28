---
title: deploymentStateReason 资源类型
description: 特定部署状态的原因。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 19a5063cd4f103b0f065311118bc5d8ac97a3c7a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067977"
---
# <a name="deploymentstatereason-resource-type"></a><span data-ttu-id="2cff8-103">deploymentStateReason 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cff8-103">deploymentStateReason resource type</span></span>

<span data-ttu-id="2cff8-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="2cff8-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cff8-105">特定部署状态的原因。</span><span class="sxs-lookup"><span data-stu-id="2cff8-105">A reason for a particular deployment state.</span></span>

## <a name="properties"></a><span data-ttu-id="2cff8-106">属性</span><span class="sxs-lookup"><span data-stu-id="2cff8-106">Properties</span></span>
|<span data-ttu-id="2cff8-107">属性</span><span class="sxs-lookup"><span data-stu-id="2cff8-107">Property</span></span>|<span data-ttu-id="2cff8-108">类型</span><span class="sxs-lookup"><span data-stu-id="2cff8-108">Type</span></span>|<span data-ttu-id="2cff8-109">说明</span><span class="sxs-lookup"><span data-stu-id="2cff8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cff8-110">值</span><span class="sxs-lookup"><span data-stu-id="2cff8-110">value</span></span>|<span data-ttu-id="2cff8-111">microsoft.graph.windowsUpdates.deploymentStateReasonValue</span><span class="sxs-lookup"><span data-stu-id="2cff8-111">microsoft.graph.windowsUpdates.deploymentStateReasonValue</span></span>|<span data-ttu-id="2cff8-112">指定部署状态的原因。</span><span class="sxs-lookup"><span data-stu-id="2cff8-112">Specifies a reason for the deployment state.</span></span> <span data-ttu-id="2cff8-113">可取值为：`scheduledByOfferWindow`、`offeringByRequest`、`pausedByRequest`、`pausedByMonitoring`。</span><span class="sxs-lookup"><span data-stu-id="2cff8-113">Possible values are: `scheduledByOfferWindow`, `offeringByRequest`, `pausedByRequest`, `pausedByMonitoring`.</span></span> <span data-ttu-id="2cff8-114">只读。</span><span class="sxs-lookup"><span data-stu-id="2cff8-114">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cff8-115">关系</span><span class="sxs-lookup"><span data-stu-id="2cff8-115">Relationships</span></span>
<span data-ttu-id="2cff8-116">无。</span><span class="sxs-lookup"><span data-stu-id="2cff8-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cff8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cff8-117">JSON representation</span></span>
<span data-ttu-id="2cff8-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cff8-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentStateReason",
  "value": "String"
}
```

