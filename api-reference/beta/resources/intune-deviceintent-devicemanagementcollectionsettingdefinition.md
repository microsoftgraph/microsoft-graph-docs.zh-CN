---
title: deviceManagementCollectionSettingDefinition 资源类型
description: 表示集合设置的定义的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 27d61b1eb2f6ef3f47c1ea9f94594950e0069f6f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365494"
---
# <a name="devicemanagementcollectionsettingdefinition-resource-type"></a>deviceManagementCollectionSettingDefinition 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示集合设置的定义的实体


继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementCollectionSettingDefinitions](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-list.md)|[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)集合|列出[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)对象的属性和关系。|
|[获取 deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-get.md)|[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|读取[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)对象的属性和关系。|
|[创建 deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-create.md)|[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|创建新的[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)对象。|
|[删除 deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-delete.md)|无|删除[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)。|
|[更新 deviceManagementCollectionSettingDefinition](../api/intune-deviceintent-devicemanagementcollectionsettingdefinition-update.md)|[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)|更新[deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的设置定义的 ID|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的值的数据类型。 可取值为：`integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。|
|displayName|String|设置的显示名称继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|isTopLevel|Boolean|如果设置是顶级的, 则可以对其进行配置, 而无需将其包装在从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的集合或复杂设置中。|
|说明|String|该设置的说明继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|
|documentationUrl|String|设置从[DeviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)继承的文档的 Url|
|keywords|String collection|与继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置关联的关键字|
|施加|[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合|继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的设置值的约束集合|
|依|[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)集合|继承自[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)的其他设置的依赖项集合|
|elementDefinitionId|String|描述集合的每个元素外观的设置定义 ID|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "elementDefinitionId": "String"
}
```



