---
title: androidForWorkAppConfigurationSchemaItem 资源类型
description: Android for Work 应用程序的自定义配置架构内的单个配置项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05d3ff594ceecd90d91c3d413d38d0828f3bfec4
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266707"
---
# <a name="androidforworkappconfigurationschemaitem-resource-type"></a>androidForWorkAppConfigurationSchemaItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android for Work 应用程序的自定义配置架构内的单个配置项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|schemaItemKey|String|应用程序用于标识项的唯一键|
|displayName|String|用户可读的名称|
|description|字符串|项在应用程序内所控制内容的说明|
|defaultBoolValue|布尔值|如果由应用开发人员指定，则为布尔类型项的默认值|
|defaultIntValue|Int32|如果由应用开发人员指定，则为整数类型项的默认值|
|defaultStringValue|String|如果由应用开发人员指定，则为字符串类型项的默认值|
|defaultStringArrayValue|String collection|如果由应用开发人员指定，则为字符串数组类型项的默认值|
|DataType|[androidForWorkAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidforworkappconfigurationschemaitemdatatype.md)|此项描述的值的类型。 可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。|
|选择|[keyValuePair](../resources/intune-androidforwork-keyvaluepair.md) 集合|可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




