---
title: deviceManagementConfigurationExchangeOnlineSettingApplicability 资源类型
description: 应用程序设置Exchange Online性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ad4a50d15780c1507303aad8548c6e513f05b50
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60492256"
---
# <a name="devicemanagementconfigurationexchangeonlinesettingapplicability-resource-type"></a>deviceManagementConfigurationExchangeOnlineSettingApplicability 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用程序设置Exchange Online性


继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|设置说明 继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|可以在继承自 [deviceManagementConfigurationSettingApplicability 上应用平台设置](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`。|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|可以在继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)上应用设置的设备模式。 可取值为：`none`、`kiosk`。|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|可通过继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)部署此设置的技术通道。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationExchangeOnlineSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationExchangeOnlineSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String"
}
```



