---
title: deviceManagementConfigurationExchangeOnlineSettingApplicability 资源类型
description: 适用于Exchange Online设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bffecb49896ec16d1225fa3e44678429f8f7694
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671504"
---
# <a name="devicemanagementconfigurationexchangeonlinesettingapplicability-resource-type"></a>deviceManagementConfigurationExchangeOnlineSettingApplicability 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于Exchange Online设置


继承自 [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|从 [deviceManagementConfigurationSettingApplicability 继承的](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md)设置说明|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-shared-devicemanagementconfigurationplatforms.md)|平台设置可以在从 [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md) 继承上应用。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`、`linux`、`unknownFutureValue`。|
|deviceMode|[deviceManagementConfigurationDeviceMode](../resources/intune-shared-devicemanagementconfigurationdevicemode.md)|可以在从 [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md) 继承的设备模式上应用该设置。 可取值为：`none`、`kiosk`。|
|技术|[deviceManagementConfigurationTechnologies](../resources/intune-mam-devicemanagementconfigurationtechnologies.md)|可以通过从 [deviceManagementConfigurationSettingApplicability](../resources/intune-mam-devicemanagementconfigurationsettingapplicability.md) 继承来部署此设置的技术通道。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`appleRemoteManagement`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`unknownFutureValue`。|

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




