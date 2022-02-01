---
title: deviceManagementConfigurationWindowsSettingApplicability 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a8b60afa3fde438467ba9b822fae4b852407a33b
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291132"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>deviceManagementConfigurationWindowsSettingApplicability 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录


继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|设置说明 继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|可以在继承自 [deviceManagementConfigurationSettingApplicability 上应用平台设置](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`、`linux`、`unknownFutureValue`。|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|可在继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md) 上应用设置的设备模式。 可取值为：`none`、`kiosk`。|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|可通过继承自 [deviceManagementConfigurationSettingApplicability 部署此设置的技术通道](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`unknownFutureValue`。|
|configurationServiceProviderVersion|String|云解决方案提供商设置的版本是其中一部分|
|maximumSupportedVersion|String|支持的最大版本Windows|
|minimumSupportedVersion|字符串|支持的最低版本Windows|
|windowsSkus|[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) 集合|设置Windows适用的 SUS 列表|
|requiresAzureAd|Boolean|AzureAD 设置要求|
|requiredAzureAdTrustType|[deviceManagementConfigurationAzureAdTrustType](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|必需属性，类型为 AzureAD 信任。 可取值为：`none`、`azureAdJoined`、`addWorkAccount`、`mdmOnly`。|

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




