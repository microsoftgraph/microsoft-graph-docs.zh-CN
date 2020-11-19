---
title: deviceManagementConfigurationWindowsSettingApplicability 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca3b520a194a09d178790f5a82f3ca21c1e00d2d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301509"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>deviceManagementConfigurationWindowsSettingApplicability 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录


继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|从[DeviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)继承的设置的说明|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|平台设置可应用于继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)。 可取值为：`none`、`macOS`、`windows10X`、`windows10`。|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|可在继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)时应用设置的设备模式。 可取值为：`none`、`kiosk`。|
|技术|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|可以通过从 [DeviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)继承来部署此设置的技术通道。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。|
|configurationServiceProviderVersion|String|CSP 的版本设置属于|
|maximumSupportedVersion|String|最大支持的 Windows 版本|
|minimumSupportedVersion|String|支持的最低版本的 Windows|
|windowsSkus|[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) 集合|该设置适用于的 Windows Sku 列表|
|requiresAzureAd|Boolean|AzureAD 设置要求|
|requiredAzureAdTrustType|[deviceManagementConfigurationAzureAdTrustType](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|必需的 AzureAD 信任类型。 可取值为：`none`、`azureAdJoined`、`addWorkAccount`、`mdmOnly`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String",
  "configurationServiceProviderVersion": "String",
  "maximumSupportedVersion": "String",
  "minimumSupportedVersion": "String",
  "windowsSkus": [
    "String"
  ],
  "requiresAzureAd": true,
  "requiredAzureAdTrustType": "String"
}
```




