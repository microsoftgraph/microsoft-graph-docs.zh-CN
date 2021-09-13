---
title: groupPolicyPresentationValueText 资源类型
description: 实体表示策略定义上的下拉列表、组合框或文本框演示文稿的字符串值。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 138bae586ee8fc714ff836ddfb6b67db97eaea3b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033481"
---
# <a name="grouppolicypresentationvaluetext-resource-type"></a>groupPolicyPresentationValueText 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示策略定义上的下拉列表、组合框或文本框演示文稿的字符串值。


继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationValueTexts](../api/intune-grouppolicy-grouppolicypresentationvaluetext-list.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 集合|列出 [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 对象的属性和关系。|
|[获取 groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-get.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|读取 [groupPolicyPresentationValueText 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 关系。|
|[创建 groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-create.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|创建新的 [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 对象。|
|[删除 groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-delete.md)|无|删除 [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)。|
|[更新 groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-update.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|更新 [groupPolicyPresentationValueText 对象](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期和时间。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|对象的创建日期和时间。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|实体的键。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|value|String|关联的演示文稿的字符串值。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|与演示文稿值关联的组策略定义值。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|presentation|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|与演示文稿值关联的组策略演示文稿。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": "String"
}
```



