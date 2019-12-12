---
title: retireScheduledManagedDevice 资源类型
description: 计划停用的 ManagedDevices
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8b79f0541450f4d3c00e4f89f02405cd74545b49
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955516"
---
# <a name="retirescheduledmanageddevice-resource-type"></a>retireScheduledManagedDevice 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

计划停用的 ManagedDevices

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|managedDeviceId|字符串|托管 DeviceId|
|managedDeviceName|String|托管设备名称|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|托管设备设备类型。 可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry`|
|complianceState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|托管设备 ComplianceStatus。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|
|retireAfterDateTime|DateTimeOffset|托管设备在 DateTime 之后停用|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|托管设备 ManagementAgentType。 可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm`。|
|所有者|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|托管设备 ManagedDeviceOwnerType。 可取值为：`unknown`、`company`、`personal`。|
|deviceCompliancePolicyName|字符串|设备合规性策略名称|
|deviceCompliancePolicyId|字符串|设备合规性 PolicyId|

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



