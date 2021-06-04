---
title: editionUpgradeConfiguration 资源类型
description: Windows 10 版本升级配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f69131852c0774048855ca8037312c8d91675a19
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754746"
---
# <a name="editionupgradeconfiguration-resource-type"></a>editionUpgradeConfiguration 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 10 版本升级配置。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List editionUpgradeConfigurations](../api/intune-deviceconfig-editionupgradeconfiguration-list.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 集合|列出 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性和关系。|
|[Get editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-get.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|读取 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性和关系。|
|[Create editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-create.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。|
|[Delete editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-delete.md)|无|删除 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)。|
|[Update editionUpgradeConfiguration](../api/intune-deviceconfig-editionupgradeconfiguration-update.md)|[editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md)|更新 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|说明|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|licenseType|[editionUpgradeLicenseType](../resources/intune-deviceconfig-editionupgradelicensetype.md)|版本升级许可证类型。 可取值为：`productKey`、`licenseFile`。|
|targetEdition|[windows10EditionType](../resources/intune-deviceconfig-windows10editiontype.md)|版本升级目标版本。 可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。|
|license|String|版本升级许可证文件内容。|
|productKey|String|版本升级产品密钥。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.editionUpgradeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "licenseType": "String",
  "targetEdition": "String",
  "license": "String",
  "productKey": "String"
}
```




