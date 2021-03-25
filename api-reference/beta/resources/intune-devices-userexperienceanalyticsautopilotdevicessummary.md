---
title: userExperienceAnalyticsAutopilotDevicesSummary 资源类型
description: 未准备好 Windows Autopilot 的设备用户体验分析摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 27faa3cf52ba5b0118137b1d64c63552d9e4f127
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159369"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a><span data-ttu-id="a9945-103">userExperienceAnalyticsAutopilotDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9945-103">userExperienceAnalyticsAutopilotDevicesSummary resource type</span></span>

<span data-ttu-id="a9945-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9945-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9945-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9945-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9945-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9945-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9945-107">未准备好 Windows Autopilot 的设备用户体验分析摘要。</span><span class="sxs-lookup"><span data-stu-id="a9945-107">The user experience analytics summary of Devices not windows autopilot ready.</span></span>

## <a name="properties"></a><span data-ttu-id="a9945-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9945-108">Properties</span></span>
|<span data-ttu-id="a9945-109">属性</span><span class="sxs-lookup"><span data-stu-id="a9945-109">Property</span></span>|<span data-ttu-id="a9945-110">类型</span><span class="sxs-lookup"><span data-stu-id="a9945-110">Type</span></span>|<span data-ttu-id="a9945-111">说明</span><span class="sxs-lookup"><span data-stu-id="a9945-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9945-112">devicesNotAutopilotRegistered</span><span class="sxs-lookup"><span data-stu-id="a9945-112">devicesNotAutopilotRegistered</span></span>|<span data-ttu-id="a9945-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a9945-113">Int32</span></span>|<span data-ttu-id="a9945-114">未注册 autopilot 的 intune 设备计数。</span><span class="sxs-lookup"><span data-stu-id="a9945-114">The count of intune devices that are not autopilot registerd.</span></span>|
|<span data-ttu-id="a9945-115">devicesWithoutAutopilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="a9945-115">devicesWithoutAutopilotProfileAssigned</span></span>|<span data-ttu-id="a9945-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a9945-116">Int32</span></span>|<span data-ttu-id="a9945-117">未分配 autopilot 配置文件的 intune 设备计数。</span><span class="sxs-lookup"><span data-stu-id="a9945-117">The count of intune devices not autopilot profile assigned.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9945-118">关系</span><span class="sxs-lookup"><span data-stu-id="a9945-118">Relationships</span></span>
<span data-ttu-id="a9945-119">无</span><span class="sxs-lookup"><span data-stu-id="a9945-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9945-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9945-120">JSON Representation</span></span>
<span data-ttu-id="a9945-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9945-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```




