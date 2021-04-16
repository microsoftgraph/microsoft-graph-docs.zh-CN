---
title: deviceManagementConfigurationChoiceSettingValueDefinitionTemplate 资源类型
description: 选项设置值定义模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b4caada35c50a0d3e804a66f1556f13fbc88bfa
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868436"
---
# <a name="devicemanagementconfigurationchoicesettingvaluedefinitiontemplate-resource-type"></a>deviceManagementConfigurationChoiceSettingValueDefinitionTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

选项设置值定义模板

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedOptions|[deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md) 集合|选项设置允许的选项|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
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
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
            "settingValueTemplateId": "String"
          }
        }
      ]
    }
  ]
}
```




