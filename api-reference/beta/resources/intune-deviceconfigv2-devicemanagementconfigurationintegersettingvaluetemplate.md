---
title: deviceManagementConfigurationIntegerSettingValueTemplate 资源类型
description: 整数设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a196cf31bbb1a7063b6d937e797d602e7481ff4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666842"
---
# <a name="devicemanagementconfigurationintegersettingvaluetemplate-resource-type"></a>deviceManagementConfigurationIntegerSettingValueTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

整数设置值模板


继承自 [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settingValueTemplateId|String|设置值模板 ID 继承自 [deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|
|defaultValue|[deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)|整数设置值默认模板。|
|recommendedValueDefinition|[deviceManagementConfigurationIntegerSettingValueDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|建议的值定义。|
|requiredValueDefinition|[deviceManagementConfigurationIntegerSettingValueDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefinitiontemplate.md)|必需的值定义。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueTemplate",
  "settingValueTemplateId": "String",
  "defaultValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
    "constantValue": 1024
  },
  "recommendedValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  },
  "requiredValueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
    "minValue": 1024,
    "maxValue": 1024
  }
}
```




