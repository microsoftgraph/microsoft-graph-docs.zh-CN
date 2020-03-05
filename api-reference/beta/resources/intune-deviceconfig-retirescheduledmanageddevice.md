---
title: retireScheduledManagedDevice 资源类型
description: 计划停用的 ManagedDevices
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 230d688429bb98361c04ad3d28789e0e886361fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529447"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>retireScheduledManagedDevice 资源类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划停用的 ManagedDevices

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|managedDeviceId|String|托管 DeviceId|
|managedDeviceName|String|托管设备名称|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|托管设备设备类型。 可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|托管设备 ComplianceStatus。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|retireAfterDateTime|DateTimeOffset|托管设备在 DateTime 之后停用|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|托管设备 ManagementAgentType。 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。|
|所有者|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|托管设备 ManagedDeviceOwnerType。 可取值为：`unknown`、`company`、`personal`。|
|deviceCompliancePolicyName|String|设备合规性策略名称|
|deviceCompliancePolicyId|String|设备合规性 PolicyId|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.retireScheduledManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.retireScheduledManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "deviceType": "String",
  "complianceState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "managementAgent": "String",
  "ownerType": "String",
  "deviceCompliancePolicyName": "String",
  "deviceCompliancePolicyId": "String"
}
```



