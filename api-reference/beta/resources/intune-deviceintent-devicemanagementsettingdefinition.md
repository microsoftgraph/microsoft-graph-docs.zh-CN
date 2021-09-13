---
title: deviceManagementSettingDefinition 资源类型
description: 表示给定设置定义的实体
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a424a11e5a86b175a405e405253d776166b9b9ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134953"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a>deviceManagementSettingDefinition 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示给定设置定义的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementSettingDefinitions](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 集合|列出 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象的属性和关系。|
|[获取 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|读取 [deviceManagementSettingDefinition 对象的属性和](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 关系。|
|[创建 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|创建新的 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象。|
|[删除 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|无|删除 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)。|
|[更新 deviceManagementSettingDefinition](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|更新 [deviceManagementSettingDefinition 对象](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|设置定义的 ID|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|值的数据类型。 可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。|
|displayName|String|设置显示名称|
|isTopLevel|Boolean|如果设置是顶级设置，则无需封装在集合或复杂设置中即可进行配置|
|说明|String|设置的说明|
|placeholderText|String|占位符文本作为有效输入的示例|
|documentationUrl|String|设置文档的 URL|
|headerTitle|String|设置标头的标题表示设置/设置的类别/部分|
|headerSubtitle|String|有关类别/节的更多详细信息，请参阅设置标头的副标题|
|keywords|字符串集合|与设置关联的关键字|
|约束|[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合|设置值的约束集合|
|依赖项|[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) 集合|其他设置上依赖项的集合|

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



