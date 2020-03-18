---
title: windowsAutopilotDeviceIdentity 资源类型
description: WindowsAutopilotDeviceIdentity 资源表示 Windows Autopilot 设备。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e3fb3e7c70fe41f353ea4816dc9f97d57cd86b4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783387"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>windowsAutopilotDeviceIdentity 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WindowsAutopilotDeviceIdentity 资源表示 Windows Autopilot 设备。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合|列出[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象的属性和关系。|
|[获取 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|读取[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象的属性和关系。|
|[创建 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|创建新的[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象。|
|[删除 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|None|删除[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)。|
|[更新 windowsAutopilotDeviceIdentity](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|更新[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)对象的属性。|
|[assignUserToDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|None|将用户分配给 Autopilot 设备。|
|[unassignUserFromDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|None|将用户从 Autopilot 设备取消分配。|
|[updateDeviceProperties 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-updatedeviceproperties.md)|None|更新 Autopilot 设备上的属性。|
|[assignResourceAccountToDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|None|向 Autopilot 设备分配资源帐户。|
|[unassignResourceAccountFromDevice 操作](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|None|取消分配 Autopilot 设备中的资源帐户。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Windows autopilot 设备的配置文件分配状态。 可取值为：`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending` 或 `failed`。|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|配置文件分配 Windows autopilot 设备的详细状态。 可取值为：`none`、`hardwareRequirementsNotMet`、`surfaceHubProfileNotSupported`、`holoLensProfileNotSupported`、`windowsPcProfileNotSupported`。|
|deploymentProfileAssignedDateTime|DateTimeOffset|Windows autopilot 设备的配置文件设置时间。|
|orderIdentifier|String|Windows autopilot 设备的顺序标识符-已弃用|
|groupTag|String|Windows autopilot 设备的 Group 标记。|
|purchaseOrderIdentifier|String|Windows autopilot 设备的采购订单标识符。|
|serialNumber|String|Windows autopilot 设备序列号。|
|productKey|字符串|Windows autopilot 设备产品密钥。|
|manufacturer|String|Windows autopilot 设备的 Oem 制造商。|
|model|String|Windows autopilot 设备的模型名称。|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Windows autopilot 设备的 Intune 注册状态。 可取值为：`unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|lastContactedDateTime|DateTimeOffset|Intune 上次联系 Windows autopilot 设备的日期时间。|
|addressableUserName|String|可寻址的用户名。|
|userPrincipalName|String|用户主体名称。|
|resourceName|String|资源名称。|
|skuNumber|String|SKU 编号|
|systemFamily|String|系统系列|
|azureActiveDirectoryDeviceId|String|AAD 设备 ID|
|managedDeviceId|String|托管设备 ID|
|displayName|String|显示名称|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|当前分配给 Windows autopilot 设备的部署配置文件。|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|准备分配给 Windows autopilot 设备的部署配置文件。|

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
  "orderIdentifier": "String",
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
  "managedDeviceId": "String",
  "displayName": "String"
}
```



