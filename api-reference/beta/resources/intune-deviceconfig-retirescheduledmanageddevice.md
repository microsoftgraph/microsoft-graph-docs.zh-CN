---
title: retireScheduledManagedDevice 资源类型
description: 计划停用的 ManagedDevices
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92c9097d47501599935fdda46b93428d4bb59369
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266448"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>retireScheduledManagedDevice 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划停用的 ManagedDevices

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|managedDeviceId|字符串|托管 DeviceId|
|managedDeviceName|String|托管设备名称|
|deviceType|[deviceType](../resources/intune-deviceconfig-devicetype.md)|托管设备设备类型。 可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` `unknown` 、|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|托管设备 ComplianceStatus。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|retireAfterDateTime|DateTimeOffset|托管设备在 DateTime 后停用|
|managementAgent|[managementAgentType](../resources/intune-deviceconfig-managementagenttype.md)|托管设备管理AgentType。 可能的值是：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`、`windowsManagementCloudApi`。|
|ownerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|托管设备 ManagedDeviceOwnerType。 可取值为：`unknown`、`company`、`personal`。|
|deviceCompliancePolicyName|String|设备合规性策略名称|
|deviceCompliancePolicyId|String|设备合规性策略Id|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。|

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
  "deviceCompliancePolicyId": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




