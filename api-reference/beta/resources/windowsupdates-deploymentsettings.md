---
title: deploymentSettings 资源类型
description: 设置控制服务何时以及如何部署更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f7c00ec8e880e7fd7ae9109fd1ac015868da902a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067856"
---
# <a name="deploymentsettings-resource-type"></a><span data-ttu-id="72d06-103">deploymentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="72d06-103">deploymentSettings resource type</span></span>

<span data-ttu-id="72d06-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="72d06-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d06-105">设置控制服务何时以及如何部署更新。</span><span class="sxs-lookup"><span data-stu-id="72d06-105">Settings controlling when and how the service deploys an update.</span></span>

<span data-ttu-id="72d06-106">[windowsDeploymentSettings 的基本类型](../resources/windowsupdates-windowsdeploymentsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="72d06-106">Base type of [windowsDeploymentSettings](../resources/windowsupdates-windowsdeploymentsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="72d06-107">属性</span><span class="sxs-lookup"><span data-stu-id="72d06-107">Properties</span></span>
|<span data-ttu-id="72d06-108">属性</span><span class="sxs-lookup"><span data-stu-id="72d06-108">Property</span></span>|<span data-ttu-id="72d06-109">类型</span><span class="sxs-lookup"><span data-stu-id="72d06-109">Type</span></span>|<span data-ttu-id="72d06-110">说明</span><span class="sxs-lookup"><span data-stu-id="72d06-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72d06-111">monitoring</span><span class="sxs-lookup"><span data-stu-id="72d06-111">monitoring</span></span>|[<span data-ttu-id="72d06-112">microsoft.graph.windowsUpdates.monitoringSettings</span><span class="sxs-lookup"><span data-stu-id="72d06-112">microsoft.graph.windowsUpdates.monitoringSettings</span></span>](../resources/windowsupdates-monitoringsettings.md)|<span data-ttu-id="72d06-113">设置管理条件，以监视要采取的自动操作。</span><span class="sxs-lookup"><span data-stu-id="72d06-113">Settings governing conditions to monitor and automated actions to take.</span></span>|
|<span data-ttu-id="72d06-114">推出</span><span class="sxs-lookup"><span data-stu-id="72d06-114">rollout</span></span>|[<span data-ttu-id="72d06-115">microsoft.graph.windowsUpdates.rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="72d06-115">microsoft.graph.windowsUpdates.rolloutSettings</span></span>](../resources/windowsupdates-rolloutsettings.md)|<span data-ttu-id="72d06-116">设置如何推出内容。</span><span class="sxs-lookup"><span data-stu-id="72d06-116">Settings governing how the content is rolled out.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72d06-117">关系</span><span class="sxs-lookup"><span data-stu-id="72d06-117">Relationships</span></span>
<span data-ttu-id="72d06-118">无。</span><span class="sxs-lookup"><span data-stu-id="72d06-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72d06-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72d06-119">JSON representation</span></span>
<span data-ttu-id="72d06-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72d06-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  }
}
```

