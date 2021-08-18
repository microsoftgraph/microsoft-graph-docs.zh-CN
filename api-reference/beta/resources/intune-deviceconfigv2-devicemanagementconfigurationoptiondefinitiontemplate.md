---
title: deviceManagementConfigurationOptionDefinitionTemplate 资源类型
description: 选项定义模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 092d68545689b443fa30460bae29ffe4da946626887a7f43fa5ed092ce9af951
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54232620"
---
# <a name="devicemanagementconfigurationoptiondefinitiontemplate-resource-type"></a>deviceManagementConfigurationOptionDefinitionTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

选项定义模板

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|itemId|字符串|Option ItemId|
|children|[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) 集合|选项子项|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
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
```




