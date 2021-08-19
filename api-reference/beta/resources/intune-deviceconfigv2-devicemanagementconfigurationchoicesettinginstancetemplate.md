---
title: deviceManagementConfigurationChoiceSettingInstanceTemplate 资源类型
description: 选项设置实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75e2235f5da3073a531b0b7477ffb70ebf145703c4a86828b594ec1974c7aed9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54148090"
---
# <a name="devicemanagementconfigurationchoicesettinginstancetemplate-resource-type"></a>deviceManagementConfigurationChoiceSettingInstanceTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

选项设置实例模板


继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settingInstanceTemplateId|字符串|设置实例模板 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|settingDefinitionId|String|设置定义 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|isRequired|Boolean|指示策略是否必须指定此设置。 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|choiceSettingValueTemplate|[deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)|选项设置值模板|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
    "defaultValue": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
      "settingDefinitionOptionId": "String",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
          "settingInstanceTemplateId": "String",
          "settingDefinitionId": "String",
          "isRequired": true,
          "simpleSettingValueTemplate": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
            "settingValueTemplateId": "String",
            "defaultValue": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
              "constantValue": "String"
            }
          }
        }
      ]
    },
    "recommendedValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
              "settingInstanceTemplateId": "String",
              "settingDefinitionId": "String",
              "isRequired": true,
              "simpleSettingValueTemplate": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
                "settingValueTemplateId": "String",
                "defaultValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                  "constantValue": "String"
                }
              }
            }
          ]
        }
      ]
    },
    "requiredValueDefinition": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
      "allowedOptions": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
          "itemId": "String",
          "children": [
            {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
              "settingInstanceTemplateId": "String",
              "settingDefinitionId": "String",
              "isRequired": true,
              "simpleSettingValueTemplate": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
                "settingValueTemplateId": "String",
                "defaultValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                  "constantValue": "String"
                }
              }
            }
          ]
        }
      ]
    },
    "settingValueTemplateId": "String"
  }
}
```




