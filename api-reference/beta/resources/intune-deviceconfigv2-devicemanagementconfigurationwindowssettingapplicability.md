---
title: deviceManagementConfigurationWindowsSettingApplicability 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f74a93faaca7e70d775dab8e39f19fc05f907d0f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210778"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a>deviceManagementConfigurationWindowsSettingApplicability 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录


继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|从 [deviceManagementConfigurationSettingApplicability 继承的](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)设置说明|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|平台设置可以在从 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md) 继承上应用。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`、`linux`、`unknownFutureValue`。|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|可以在从 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md) 继承的设备模式上应用该设置。 可取值为：`none`、`kiosk`。|
|技术|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|可以通过从 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md) 继承来部署此设置的技术通道。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`appleRemoteManagement`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`unknownFutureValue`。|
|configurationServiceProviderVersion|String|CSP 设置的版本是其中的一部分|
|maximumSupportedVersion|String|支持的最大版本Windows|
|minimumSupportedVersion|String|支持的最小版本Windows|
|windowsSkus|[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) 集合|设置适用于的Windows SKU 列表|
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




