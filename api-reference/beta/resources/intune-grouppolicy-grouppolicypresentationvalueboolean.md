---
title: groupPolicyPresentationValueBoolean 资源类型
description: 实体表示策略定义上 checkbox 演示文稿的布尔值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e7abc5ef2d4a9ef6af4cfbf49f24b92fa542778
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996356"
---
# <a name="grouppolicypresentationvalueboolean-resource-type"></a>groupPolicyPresentationValueBoolean 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示策略定义上 checkbox 演示文稿的布尔值。


继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationValueBooleans](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-list.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)集合|列出[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象的属性和关系。|
|[获取 groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-get.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|读取[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象的属性和关系。|
|[创建 groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-create.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|创建新的[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象。|
|[删除 groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-delete.md)|无|删除[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)。|
|[更新 groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-update.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|更新[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期和时间。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|对象的创建日期和时间。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|实体的键。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|value|Boolean|一个布尔值, 用于关联的演示文稿。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|与演示文稿值关联的组策略定义值。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|变形|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|与演示文稿值关联的组策略演示文稿。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": true
}
```





