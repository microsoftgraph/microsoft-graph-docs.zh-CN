---
title: windowsAutopilotDeviceIdentity 资源类型
description: windowsAutopilotDeviceIdentity 资源表示 Windows Autopilot 设备。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e17d665da56a9625d6b83f384904af18284d2bcd
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629405"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>windowsAutopilotDeviceIdentity 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

windowsAutopilotDeviceIdentity 资源表示 Windows Autopilot 设备。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 集合|列出 [windowsAutopilotDeviceIdentity 对象的属性和](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 关系。|
|[获取 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|读取 [windowsAutopilotDeviceIdentity 对象的属性和](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 关系。|
|[创建 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|创建新的 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 对象。|
|[删除 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|无|删除 [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)。|
|[assignUserToDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|无|将用户分配给 Autopilot 设备。|
|[unassignUserFromDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|无|取消分配 Autopilot 设备中的用户。|
|[updateDeviceProperties 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|无|更新 Autopilot 设备上的属性。|
|[assignResourceAccountToDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|无|将资源帐户分配给 Autopilot 设备。|
|[unassignResourceAccountFromDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|无|取消分配 Autopilot 设备中的资源帐户。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Windows Autopilot 设备的配置文件分配状态。 可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|配置文件分配 Windows Autopilot 设备的详细状态。 可取值为：`none`、`hardwareRequirementsNotMet`、`surfaceHubProfileNotSupported`、`holoLensProfileNotSupported`、`windowsPcProfileNotSupported`、`surfaceHub2SProfileNotSupported` 或 `unknownFutureValue`。|
|deploymentProfileAssignedDateTime|DateTimeOffset|Windows Autopilot 设备的配置文件设置时间。|
|groupTag|String|Windows autopilot 设备的组标记。|
|purchaseOrderIdentifier|String|Purchase Order Windows autopilot 设备的标识符。|
|serialNumber|String|Windows autopilot 设备序列号。|
|productKey|String|Windows autopilot 设备产品密钥。|
|manufacturer|String|Windows autopilot 设备的 Oem 制造商。|
|model|String|Windows autopilot 设备的型号名称。|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Intune Windows autopilot 设备的注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|lastContactedDateTime|DateTimeOffset|Intune Windows autopilot 设备的上次联系日期时间。|
|addressableUserName|String|可地址用户名。|
|userPrincipalName|String|用户主体名称。|
|resourceName|String|资源名称。|
|skuNumber|String|SKU 号|
|systemFamily|String|系统系列|
|azureActiveDirectoryDeviceId|String|AAD 设备 ID - 已弃用|
|azureAdDeviceId|String|AAD 设备 ID|
|managedDeviceId|String|托管设备 ID|
|displayName|String|显示名称|
|deviceAccountUpn|String|Surface Hub 设备帐户 Upn|
|deviceAccountPassword|String|Surface Hub 设备帐户密码|
|deviceFriendlyName|String|Surface Hub 设备友好名称|

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
  "deviceFriendlyName": "String"
}
```




