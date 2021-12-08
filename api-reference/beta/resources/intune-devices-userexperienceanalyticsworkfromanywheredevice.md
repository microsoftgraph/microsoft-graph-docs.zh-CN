---
title: userExperienceAnalyticsWorkFromAnywhereDevice 资源类型
description: 用户体验分析设备：从任何位置工作的报告
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05ebbb411beb44d9877fd6b56b972fecb5519838
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343579"
---
# <a name="userexperienceanalyticsworkfromanywheredevice-resource-type"></a>userExperienceAnalyticsWorkFromAnywhereDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备：从任何位置工作的报告

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsWorkFromAnywhereDevices](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-list.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 集合|列出 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-get.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|读取 [userExperienceAnalyticsWorkFromAnywhereDevice 对象的属性和](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 关系。|
|[创建 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-create.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|创建新的 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象。|
|[删除 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-delete.md)|None|删除 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)。|
|[更新 userExperienceAnalyticsWorkFromAnywhereDevice](../api/intune-devices-userexperienceanalyticsworkfromanywheredevice-update.md)|[userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)|更新 [userExperienceAnalyticsWorkFromAnywhereDevice 对象](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析的唯一标识符从任何设备工作。|
|deviceId|String|用户体验从任何设备 ID 开始工作。|
|deviceName|String|来自任何设备名称的工作。|
|serialNumber|String|用户体验随设备序列号随处工作。|
|manufacturer|String|用户体验从任何设备制造商处工作。|
|model|String|用户体验从任何设备型号开始工作。|
|ownership|String|用户体验从任何设备所有权开始工作。|
|managedBy|String|用户体验从设备的任何管理代理工作。|
|autoPilotRegistered|Boolean|用户体验从 intune 设备的 autopilotRegistered 的任何位置工作。|
|autoPilotProfileAssigned|布尔|用户体验分析从 intune 设备的 autopilotProfileAssigned 的任何位置工作。|
|azureAdRegistered|布尔|用户体验从任何设备的 azureAdRegistered 工作。|
|azureAdDeviceId|String|用户体验从 Azure Ad 设备 ID 的任何位置工作。|
|azureAdJoinType|String|用户体验从任何设备的 azure Ad joinType 工作。|
|osDescription|String|用户体验从任何设备的操作系统说明工作。|
|osVersion|String|用户体验从任何设备的操作系统版本工作。|
|tenantAttached|布尔|用户体验从任何设备的 tenantAttached 工作。|
|compliancePolicySetToIntune|布尔|用户体验从任何设备的 compliancePolicySetToIntune 工作。|
|otherWorkloadsSetToIntune|Boolean|用户体验从任何设备的其他WorkloadsSetToIntune 工作。|
|isCloudManagedGatewayEnabled|Boolean|在启用了 Configuration Manager 的云管理网关的任何位置，用户体验都可用。|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|用户体验从设备的任何 Windows 升级资格状态工作。 可取值为：`upgraded`、`unknown`、`notCapable`、`capable`。|
|ramCheckFailed|Boolean|用户体验分析是否从任何设备 RAM 硬件检查失败，设备无法升级到最新版本的 Windows|
|storageCheckFailed|Boolean|用户体验适用于任何设备，设备升级到最新版本的 Windows 时存储硬件检查是否失败。|
|processorCoreCountCheckFailed|布尔|用户体验适用于任何设备，设备升级到最新版本的 Windows 时处理器硬件核心计数检查是否失败。|
|processorSpeedCheckFailed|布尔|用户体验适用于任何设备，设备升级到最新版本的 Windows 时处理器硬件速度检查是否失败。|
|tpmCheckFailed|布尔|用户体验从任何设备工作，"受信任的平台模块 (TPM) 设备升级到 Windows 的最新版本的硬件检查失败。|
|secureBootCheckFailed|布尔|用户体验适用于任何设备，安全启动硬件检查是否因设备升级到最新版本的 Windows 而失败。|
|processorFamilyCheckFailed|布尔|用户体验适用于任何设备，设备升级到最新版本的 Windows 时处理器硬件系列检查是否失败。|
|processor64BitCheckFailed|布尔|用户体验适用于任何设备，处理器硬件 64 位体系结构检查是否失败，设备无法升级到最新版本的 Windows。|
|osCheckFailed|布尔|用户体验适用于任何设备，操作系统检查是否失败，设备是否升级到最新版本的 Windows。|
|workFromAnywhereScore|双精度|用户体验从每个设备的整体分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|windowsScore|双精度|用户体验从每个设备窗口分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudManagementScore|双精度|用户体验按设备云管理分数从任意位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudIdentityScore|双精度|用户体验从每个设备云标识分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudProvisioningScore|双精度|用户体验从每个设备云预配分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验从每个设备运行状况状态的任何位置工作。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "ownership": "String",
  "managedBy": "String",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "String",
  "azureAdJoinType": "String",
  "osDescription": "String",
  "osVersion": "String",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "isCloudManagedGatewayEnabled": true,
  "upgradeEligibility": "String",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "workFromAnywhereScore": "4.2",
  "windowsScore": "4.2",
  "cloudManagementScore": "4.2",
  "cloudIdentityScore": "4.2",
  "cloudProvisioningScore": "4.2",
  "healthStatus": "String"
}
```




