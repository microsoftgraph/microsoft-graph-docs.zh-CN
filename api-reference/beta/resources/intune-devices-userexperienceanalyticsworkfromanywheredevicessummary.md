---
title: userExperienceAnalyticsWorkFromAnywhereDevicesSummary 资源类型
description: 用户体验分析从 Anywhere 指标设备摘要工作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8be606cb2cc291adf878b5194c4b9063d993464e
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60481053"
---
# <a name="userexperienceanalyticsworkfromanywheredevicessummary-resource-type"></a>userExperienceAnalyticsWorkFromAnywhereDevicesSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析从 Anywhere 指标设备摘要工作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|autopilotDevicesSummary|[userExperienceAnalyticsAutopilotDevicesSummary](../resources/intune-devices-userexperienceanalyticsautopilotdevicessummary.md)|来自任何 Autopilot 设备的工作值摘要。|
|cloudManagementDevicesSummary|[userExperienceAnalyticsCloudManagementDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudmanagementdevicessummary.md)|用户体验从任意位置云管理设备摘要工作。|
|windows10DevicesSummary|[userExperienceAnalyticsWindows10DevicesSummary](../resources/intune-devices-userexperienceanalyticswindows10devicessummary.md)|用户体验分析从任意位置到设备Windows 10工作。|
|cloudIdentityDevicesSummary|[userExperienceAnalyticsCloudIdentityDevicesSummary](../resources/intune-devices-userexperienceanalyticscloudidentitydevicessummary.md)|用户体验分析从任意位置云标识设备摘要工作。|
|totalDevices|Int32|设备总数。 有效值 -2147483648 to 2147483647|
|coManagedDevices|Int32|共同管理的设备的总数。 有效值 -2147483648 to 2147483647|
|intuneDevices|Int32|未注册 autopilot 的 intune 设备计数。 有效值 -2147483648 to 2147483647|
|tenantAttachDevices|Int32|租户附加设备总数。 有效值 -2147483648 to 2147483647|
|windows10Devices|Int32|Windows 10 设备计数。 有效值 -2147483648 to 2147483647|
|windows10DevicesWithoutTenantAttach|Int32|Intune 和 Comanaged 的 Windows 10 设备计数。 有效值 -2147483648 to 2147483647|
|unsupportedOSversionDevices|Int32|操作系统Windows 10不支持的设备数量。 有效值 -2147483648 to 2147483647|
|devicesWithoutCloudIdentity|Int32|非云标识的设备计数。 有效值 -2147483648 to 2147483647|
|devicesNotAutopilotRegistered|Int32|未注册 autopilot 的 intune 设备计数。 有效值 -2147483648 to 2147483647|
|devicesWithoutAutopilotProfileAssigned|Int32|未分配 autopilot 配置文件的 intune 设备计数。 有效值 -2147483648 to 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
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
    "devicesWithoutAutopilotProfileAssigned": 1024,
    "totalWindows10DevicesWithoutTenantAttached": 1024
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
  },
  "cloudIdentityDevicesSummary": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary",
    "deviceWithoutCloudIdentityCount": 1024
  },
  "totalDevices": 1024,
  "coManagedDevices": 1024,
  "intuneDevices": 1024,
  "tenantAttachDevices": 1024,
  "windows10Devices": 1024,
  "windows10DevicesWithoutTenantAttach": 1024,
  "unsupportedOSversionDevices": 1024,
  "devicesWithoutCloudIdentity": 1024,
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024
}
```



