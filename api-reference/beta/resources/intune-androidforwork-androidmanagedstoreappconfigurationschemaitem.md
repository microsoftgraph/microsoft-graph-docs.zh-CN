---
title: androidManagedStoreAppConfigurationSchemaItem 资源类型
description: 在 Android 应用程序的自定义配置架构的单个配置项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a12c8f4dc0a07dbf74c92193ac73fdcfe9bfd883
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398917"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>androidManagedStoreAppConfigurationSchemaItem 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在 Android 应用程序的自定义配置架构的单个配置项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|schemaItemKey|String|应用程序用于标识项的唯一键|
|displayName|String|用户可读的名称|
|说明|String|项在应用程序内所控制内容的说明|
|defaultBoolValue|布尔值|如果由应用开发人员指定，则为布尔类型项的默认值|
|defaultIntValue|Int32|如果由应用开发人员指定，则为整数类型项的默认值|
|defaultStringValue|String|如果由应用开发人员指定，则为字符串类型项的默认值|
|defaultStringArrayValue|String collection|如果由应用开发人员指定，则为字符串数组类型项的默认值|
|DataType|[androidManagedStoreAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|描述此项的值的类型。 可取值为：`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden`。|
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




