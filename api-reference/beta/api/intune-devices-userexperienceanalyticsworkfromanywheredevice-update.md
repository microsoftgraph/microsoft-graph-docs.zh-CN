---
title: 更新 userExperienceAnalyticsWorkFromAnywhereDevice
description: 更新 userExperienceAnalyticsWorkFromAnywhereDevice 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2dfdfd64aa892ce5668ddd267a4f20ece31e4a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59058990"
---
# <a name="update-userexperienceanalyticsworkfromanywheredevice"></a>更新 userExperienceAnalyticsWorkFromAnywhereDevice

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsWorkFromAnywhereDevice 对象](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsWorkFromAnywhereDevice 时所需的属性](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析的唯一标识符从任何设备工作。|
|deviceName|String|来自任何设备名称的工作。|
|serialNumber|String|用户体验随设备序列号随处工作。|
|manufacturer|String|用户体验从任何设备制造商处工作。|
|model|String|用户体验从任何设备型号开始工作。|
|ownership|String|用户体验从任何设备所有权开始工作。|
|managedBy|String|用户体验从设备的任何管理代理工作。|
|autoPilotRegistered|Boolean|用户体验从 intune 设备的 autopilotRegistered 的任何位置工作。|
|autoPilotProfileAssigned|Boolean|用户体验分析从 intune 设备的 autopilotProfileAssigned 的任何位置工作。|
|azureAdRegistered|Boolean|用户体验从任何设备的 azureAdRegistered 工作。|
|azureAdDeviceId|String|用户体验从 Azure Ad 设备 ID 的任何位置工作。|
|azureAdJoinType|String|用户体验从任何设备的 azure Ad joinType 工作。|
|osDescription|String|用户体验从任何设备的操作系统说明工作。|
|osVersion|String|用户体验从任何设备的操作系统版本工作。|
|tenantAttached|Boolean|用户体验从任何设备的 tenantAttached 工作。|
|compliancePolicySetToIntune|Boolean|用户体验从任何设备的 compliancePolicySetToIntune 工作。|
|otherWorkloadsSetToIntune|Boolean|用户体验从任何设备的其他WorkloadsSetToIntune 工作。|
|upgradeEligibility|[operatingSystemUpgradeEligibility](../resources/intune-devices-operatingsystemupgradeeligibility.md)|用户体验从设备的任何 Windows 升级资格状态工作。 可取值为：`upgraded`、`unknown`、`notCapable`、`capable`。|
|ramCheckFailed|Boolean|用户体验分析是否从任何设备 RAM 硬件检查失败，设备无法升级到最新版本的 Windows|
|storageCheckFailed|Boolean|用户体验适用于任何设备，设备升级到最新版本的 Windows 时存储硬件检查是否失败。|
|processorCoreCountCheckFailed|Boolean|用户体验适用于任何设备，设备升级到最新版本的 Windows 时处理器硬件核心计数检查是否失败。|
|processorSpeedCheckFailed|Boolean|用户体验适用于任何设备，设备升级到最新版本的 Windows 时处理器硬件速度检查是否失败。|
|tpmCheckFailed|Boolean|用户体验从任何设备工作，"受信任的平台模块 (TPM) 设备升级到 Windows 的最新版本的硬件检查失败。|
|secureBootCheckFailed|Boolean|用户体验适用于任何设备，安全启动硬件检查是否因设备升级到最新版本的 Windows 而失败。|
|processorFamilyCheckFailed|Boolean|用户体验适用于任何设备，设备升级到最新版本的 Windows 时处理器硬件系列检查是否失败。|
|processor64BitCheckFailed|Boolean|用户体验适用于任何设备，处理器硬件 64 位体系结构检查是否失败，设备无法升级到最新版本的 Windows。|
|osCheckFailed|Boolean|用户体验适用于任何设备，操作系统检查是否失败，设备是否升级到最新版本的 Windows。|
|windowsScore|双精度|用户体验从每个设备窗口分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudManagementScore|双精度|用户体验按设备云管理分数从任意位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudIdentityScore|双精度|用户体验从每个设备云标识分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|cloudProvisioningScore|双精度|用户体验从每个设备云预配分数的任何位置工作。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验从每个设备运行状况状态的任何位置工作。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
Content-type: application/json
Content-length: 1215

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1264

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value",
  "osDescription": "Os Description value",
  "osVersion": "Os Version value",
  "tenantAttached": true,
  "compliancePolicySetToIntune": true,
  "otherWorkloadsSetToIntune": true,
  "upgradeEligibility": "unknown",
  "ramCheckFailed": true,
  "storageCheckFailed": true,
  "processorCoreCountCheckFailed": true,
  "processorSpeedCheckFailed": true,
  "tpmCheckFailed": true,
  "secureBootCheckFailed": true,
  "processorFamilyCheckFailed": true,
  "processor64BitCheckFailed": true,
  "osCheckFailed": true,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```



