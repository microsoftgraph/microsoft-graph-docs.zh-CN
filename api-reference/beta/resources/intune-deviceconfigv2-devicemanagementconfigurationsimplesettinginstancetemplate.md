---
title: deviceManagementConfigurationSimpleSettingInstanceTemplate 资源类型
description: 简单设置实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b09e26ef14e20c1cbc95013beb09f9111ddf123e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868420"
---
# <a name="devicemanagementconfigurationsimplesettinginstancetemplate-resource-type"></a>deviceManagementConfigurationSimpleSettingInstanceTemplate 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

简单设置实例模板


继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|settingInstanceTemplateId|String|设置实例模板 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|settingDefinitionId|String|设置定义 ID 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|isRequired|Boolean|指示策略是否必须指定此设置。 继承自 [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|
|simpleSettingValueTemplate|[deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|简单设置值模板|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
    "settingValueTemplateId": "String"
  }
}
```




