---
title: windowsDeploymentSettings 资源类型
description: 设置控制服务何时以及如何部署Windows 10更新。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: bc55f0643e789c802254064797bf8a5c2047cb64
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067300"
---
# <a name="windowsdeploymentsettings-resource-type"></a><span data-ttu-id="7e757-103">windowsDeploymentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e757-103">windowsDeploymentSettings resource type</span></span>

<span data-ttu-id="7e757-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="7e757-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e757-105">设置控制服务何时以及如何部署Windows 10更新。</span><span class="sxs-lookup"><span data-stu-id="7e757-105">Settings controlling when and how the service deploys a Windows 10 update.</span></span>

<span data-ttu-id="7e757-106">继承自 [deploymentSettings](../resources/windowsupdates-deploymentsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="7e757-106">Inherits from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7e757-107">属性</span><span class="sxs-lookup"><span data-stu-id="7e757-107">Properties</span></span>
|<span data-ttu-id="7e757-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e757-108">Property</span></span>|<span data-ttu-id="7e757-109">类型</span><span class="sxs-lookup"><span data-stu-id="7e757-109">Type</span></span>|<span data-ttu-id="7e757-110">说明</span><span class="sxs-lookup"><span data-stu-id="7e757-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e757-111">monitoring</span><span class="sxs-lookup"><span data-stu-id="7e757-111">monitoring</span></span>|[<span data-ttu-id="7e757-112">microsoft.graph.windowsUpdates.monitoringSettings</span><span class="sxs-lookup"><span data-stu-id="7e757-112">microsoft.graph.windowsUpdates.monitoringSettings</span></span>](../resources/windowsupdates-monitoringsettings.md)|<span data-ttu-id="7e757-113">设置管理条件，以监视要采取的自动操作。</span><span class="sxs-lookup"><span data-stu-id="7e757-113">Settings governing conditions to monitor and automated actions to take.</span></span> <span data-ttu-id="7e757-114">继承自 [deploymentSettings](../resources/windowsupdates-deploymentsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="7e757-114">Inherited from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>|
|<span data-ttu-id="7e757-115">推出</span><span class="sxs-lookup"><span data-stu-id="7e757-115">rollout</span></span>|[<span data-ttu-id="7e757-116">microsoft.graph.windowsUpdates.rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="7e757-116">microsoft.graph.windowsUpdates.rolloutSettings</span></span>](../resources/windowsupdates-rolloutsettings.md)|<span data-ttu-id="7e757-117">设置如何推出内容。继承自[deploymentSettings](../resources/windowsupdates-deploymentsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="7e757-117">Settings governing how the content is rolled out. Inherited from [deploymentSettings](../resources/windowsupdates-deploymentsettings.md).</span></span>|
|<span data-ttu-id="7e757-118">userExperience</span><span class="sxs-lookup"><span data-stu-id="7e757-118">userExperience</span></span>|[<span data-ttu-id="7e757-119">microsoft.graph.windowsUpdates.userExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="7e757-119">microsoft.graph.windowsUpdates.userExperienceSettings</span></span>](../resources/windowsupdates-userexperiencesettings.md)|<span data-ttu-id="7e757-120">设置在设备上管理用户的更新体验。</span><span class="sxs-lookup"><span data-stu-id="7e757-120">Settings governing the user's update experience on a device.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e757-121">关系</span><span class="sxs-lookup"><span data-stu-id="7e757-121">Relationships</span></span>
<span data-ttu-id="7e757-122">无。</span><span class="sxs-lookup"><span data-stu-id="7e757-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e757-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e757-123">JSON representation</span></span>
<span data-ttu-id="7e757-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e757-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsDeploymentSettings",
  "rollout": {
    "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
  },
  "monitoring": {
    "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
  },
  "userExperience": {
    "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
  }
}
```

