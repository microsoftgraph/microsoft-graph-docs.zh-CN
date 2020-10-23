---
title: deviceManagementSettingDefinition 资源类型
description: 表示给定设置的定义的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 782986bac762ff434cb35955f7811eb71de6bf61
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733998"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a>deviceManagementSettingDefinition 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示给定设置的定义的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementSettingDefinitions](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 集合|列出 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象的属性和关系。|
|[获取 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|读取 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象的属性和关系。|
|[创建 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|创建新的 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象。|
|[删除 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|无|删除 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)。|
|[更新 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|更新 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设置定义的 ID|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|值的数据类型。 可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。|
|displayName|String|设置的显示名称|
|isTopLevel|布尔|如果设置是顶级的，则可以对其进行配置，而无需将其包装在集合或复杂设置中|
|说明|String|设置的说明|
|placeholderText|String|作为有效输入的示例的占位符文本|
|documentationUrl|String|设置文档的 Url|
|headerTitle|String|设置标头的标题代表设置/设置的类别/部分|
|headerSubtitle|String|设置标头的副标题，以获取有关 category/节的更多详细信息|
|keywords|String collection|与设置相关联的关键字|
|施加|[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合|设置值的约束集合|
|依|[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合|对其他设置的依赖项的集合|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "placeholderText": "String",
  "documentationUrl": "String",
  "headerTitle": "String",
  "headerSubtitle": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
          "supportedTypes": [
            "String"
          ]
        }
      ]
    }
  ]
}
```





