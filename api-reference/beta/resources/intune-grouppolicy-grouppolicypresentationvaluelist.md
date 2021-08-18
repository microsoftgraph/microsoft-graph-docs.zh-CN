---
title: groupPolicyPresentationValueList 资源类型
description: 实体表示策略定义上列表框演示文稿的名称/值对的集合。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a12ec32440d028a0423e5b9acb409214db84f28
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266833"
---
# <a name="grouppolicypresentationvaluelist-resource-type"></a>groupPolicyPresentationValueList 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示策略定义上列表框演示文稿的名称/值对的集合。


继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationValueLists](../api/intune-grouppolicy-grouppolicypresentationvaluelist-list.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) 集合|列出 [groupPolicyPresentationValueList 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) 关系。|
|[获取 groupPolicyPresentationValueList](../api/intune-grouppolicy-grouppolicypresentationvaluelist-get.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|读取 [groupPolicyPresentationValueList 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) 关系。|
|[创建 groupPolicyPresentationValueList](../api/intune-grouppolicy-grouppolicypresentationvaluelist-create.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|创建新的 [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) 对象。|
|[删除 groupPolicyPresentationValueList](../api/intune-grouppolicy-grouppolicypresentationvaluelist-delete.md)|无|删除 [groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)。|
|[更新 groupPolicyPresentationValueList](../api/intune-grouppolicy-grouppolicypresentationvaluelist-update.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|更新 [groupPolicyPresentationValueList 对象](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期和时间。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|对象的创建日期和时间。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|实体的键。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|[keyValuePair](../resources/intune-grouppolicy-keyvaluepair.md) 集合|关联的演示文稿的对列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|与演示文稿值关联的组策略定义值。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|presentation|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|与演示文稿值关联的组策略演示文稿。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




