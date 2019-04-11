---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: Android 应用程序的自定义配置架构内的单个配置项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 964916f9f6a46cd8b276e304bfb341d6504db0d2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785816"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>androidManagedStoreAppConfigurationSchemaItem 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 应用程序的自定义配置架构内的单个配置项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|schemaItemKey|String|应用程序用于标识项的唯一键|
|displayName|字符串|用户可读的名称|
|description|String|项在应用程序内所控制内容的说明|
|defaultBoolValue|布尔值|如果由应用开发人员指定，则为布尔类型项的默认值|
|defaultIntValue|Int32|如果由应用开发人员指定，则为整数类型项的默认值|
|defaultStringValue|String|如果由应用开发人员指定，则为字符串类型项的默认值|
|defaultStringArrayValue|String collection|如果由应用开发人员指定，则为字符串数组类型项的默认值|
|DataType|[androidManagedStoreAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|此项目描述的值的类型。 可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。|
|选择|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|可为此项（仅 Choice 和 Multiselect 项）设置的有效值的用于可读名称/值对列表|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





