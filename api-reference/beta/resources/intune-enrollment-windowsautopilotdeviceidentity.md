---
title: windowsAutopilotDeviceIdentity 资源类型
description: windowsAutopilotDeviceIdentity 资源表示Windows Autopilot 设备。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e045b10786952f2de88c7341a80212620818fe21
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211401"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>windowsAutopilotDeviceIdentity 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

windowsAutopilotDeviceIdentity 资源表示Windows Autopilot 设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 集合|列出 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象的属性和关系。|
|[获取 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|读取 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象的属性和关系。|
|[创建 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|创建新的 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。|
|[删除 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|无|删除 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)。|
|[assignUserToDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|无|将用户分配到 Autopilot 设备。|
|[unassignUserFromDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|无|从 Autopilot 设备取消分配用户。|
|[updateDeviceProperties 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|无|更新 Autopilot 设备上的属性。|
|[assignResourceAccountToDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|无|将资源帐户分配给 Autopilot 设备。|
|[unassignResourceAccountFromDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|无|从 Autopilot 设备取消分配资源帐户。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Windows autopilot 设备的配置文件分配状态。 可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|配置文件分配Windows autopilot 设备的详细状态。 可取值为：`none`、`hardwareRequirementsNotMet`、`surfaceHubProfileNotSupported`、`holoLensProfileNotSupported`、`windowsPcProfileNotSupported`、`surfaceHub2SProfileNotSupported` 或 `unknownFutureValue`。|
|deploymentProfileAssignedDateTime|DateTimeOffset|Windows autopilot 设备的配置文件设置时间。|
|groupTag|String|Windows autopilot 设备的组标记。|
|purchaseOrderIdentifier|String|Windows autopilot 设备的采购订单标识符。|
|serialNumber|String|Windows autopilot 设备序列号。|
|productKey|String|Windows autopilot 设备产品密钥。|
|manufacturer|String|Windows autopilot 设备的 Oem 制造商。|
|model|String|Windows autopilot 设备的模型名称。|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune autopilot 设备的Windows注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|lastContactedDateTime|DateTimeOffset|Intune Windows autopilot 设备的上次联系日期时间。|
|addressableUserName|String|可寻址用户名。|
|userPrincipalName|String|用户主体名称。|
|resourceName|String|资源名称。|
|skuNumber|String|SKU 编号|
|systemFamily|String|系统系列|
|azureActiveDirectoryDeviceId|字符串|AAD设备 ID - 要弃用|
|azureAdDeviceId|String|AAD设备 ID|
|managedDeviceId|String|托管设备 ID|
|displayName|String|显示名称|
|deviceAccountUpn|String|Surface Hub设备帐户更新|
|deviceAccountPassword|String|Surface Hub设备帐户密码|
|deviceFriendlyName|String|Surface Hub设备友好名称|
|remediationState|[windowsAutopilotDeviceRemediationState](../resources/intune-enrollment-windowsautopilotdeviceremediationstate.md)|设备修正状态。 可取值为：`unknown`、`noRemediationRequired`、`automaticRemediationRequired`、`manualRemediationRequired`、`unknownFutureValue`。|
|remediationStateLastModifiedDateTime|DateTimeOffset|Autopilot 设备的 RemediationState 设置时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|当前分配给 Windows autopilot 设备的部署配置文件。|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|要分配给 Windows autopilot 设备的部署配置文件。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "deploymentProfileAssignmentStatus": "String",
  "deploymentProfileAssignmentDetailedStatus": "String",
  "deploymentProfileAssignedDateTime": "String (timestamp)",
  "groupTag": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "azureAdDeviceId": "String",
  "managedDeviceId": "String",
  "displayName": "String",
  "deviceAccountUpn": "String",
  "deviceAccountPassword": "String",
  "deviceFriendlyName": "String",
  "remediationState": "String",
  "remediationStateLastModifiedDateTime": "String (timestamp)"
}
```




