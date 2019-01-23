---
title: groupPolicyPresentationValueDecimal 资源类型
description: 实体表示上策略定义的小数文本框演示文稿的无符号的整数值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07f0e1c93b3c0b134f90c2512514dd50e711cac5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429315"
---
# <a name="grouppolicypresentationvaluedecimal-resource-type"></a>groupPolicyPresentationValueDecimal 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示上策略定义的小数文本框演示文稿的无符号的整数值。


继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 groupPolicyPresentationValueDecimals](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-list.md)|[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)集合|列出属性和[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)对象之间的关系。|
|[获取 groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-get.md)|[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|读取属性和[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)对象的关系。|
|[创建 groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-create.md)|[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|创建新的[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)对象。|
|[删除 groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-delete.md)|无|删除[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)。|
|[更新 groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-update.md)|[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|更新[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|日期和时间上次修改对象。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|日期和时间创建对象。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|实体的键。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|值|Int64|关联的演示文稿无符号的整数值。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|关联的演示文稿值的组策略定义值。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|演示文稿|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|组策略演示的演示文稿值相关联。 继承自[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueDecimal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": 1024
}
```




