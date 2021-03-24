---
title: userExperienceAnalyticsWorkFromAnywhereDevicesSummary 资源类型
description: 用户体验分析从 Anywhere 指标设备摘要工作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6448bbc89ebe8357fa14a375f82fb73938f6634
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146747"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a><span data-ttu-id="4c4eb-103">userExperienceAnalyticsWorkFromAnywhereDevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c4eb-103">userExperienceAnalyticsWorkFromAnywhereDevicesSummary resource type</span></span>

<span data-ttu-id="4c4eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c4eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c4eb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c4eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c4eb-107">用户体验分析从 Anywhere 指标设备摘要工作。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-107">The user experience analytics Work From Anywhere metrics devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="4c4eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c4eb-108">Properties</span></span>
|<span data-ttu-id="4c4eb-109">属性</span><span class="sxs-lookup"><span data-stu-id="4c4eb-109">Property</span></span>|<span data-ttu-id="4c4eb-110">类型</span><span class="sxs-lookup"><span data-stu-id="4c4eb-110">Type</span></span>|<span data-ttu-id="4c4eb-111">说明</span><span class="sxs-lookup"><span data-stu-id="4c4eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c4eb-112">autopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="4c4eb-112">autopilotDevicesSummary</span></span>|[<span data-ttu-id="4c4eb-113">userExperienceAnalyticsAutopilotDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="4c4eb-113">userExperienceAnalyticsAutopilotDevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|<span data-ttu-id="4c4eb-114">来自任何 Autopilot 设备的工作值摘要。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-114">The value of work from anywhere autopilot devices summary.</span></span>|
|<span data-ttu-id="4c4eb-115">cloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="4c4eb-115">cloudManagementDevicesSummary</span></span>|[<span data-ttu-id="4c4eb-116">userExperienceAnalyticsCloudManagementDevicesSummary</span><span class="sxs-lookup"><span data-stu-id="4c4eb-116">userExperienceAnalyticsCloudManagementDevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|<span data-ttu-id="4c4eb-117">用户体验从任意位置云管理设备摘要工作。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-117">The user experience work from anywhere Cloud management devices summary.</span></span>|
|<span data-ttu-id="4c4eb-118">windows10DevicesSummary</span><span class="sxs-lookup"><span data-stu-id="4c4eb-118">windows10DevicesSummary</span></span>|[<span data-ttu-id="4c4eb-119">userExperienceAnalyticsWindows10DevicesSummary</span><span class="sxs-lookup"><span data-stu-id="4c4eb-119">userExperienceAnalyticsWindows10DevicesSummary</span></span>](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|<span data-ttu-id="4c4eb-120">用户体验分析可随时随地使用 Windows 10 设备摘要。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-120">The user experience analytics work from anywhere Windows 10 devices summary.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c4eb-121">关系</span><span class="sxs-lookup"><span data-stu-id="4c4eb-121">Relationships</span></span>
<span data-ttu-id="4c4eb-122">无</span><span class="sxs-lookup"><span data-stu-id="4c4eb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c4eb-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c4eb-123">JSON Representation</span></span>
<span data-ttu-id="4c4eb-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c4eb-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
  "autopilotDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
    "devicesNotAutopilotRegistered": 1024,
    "devicesWithoutAutopilotProfileAssigned": 1024
  },
  "cloudManagementDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
    "coManagedDeviceCount": 1024,
    "intuneDeviceCount": 1024,
    "tenantAttachDeviceCount": 1024
  },
  "windows10DevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
    "unsupportedOSversionDeviceCount": 1024
  }
}
```




