---
title: groupPolicyPresentationValueMultiText 资源类型
description: 实体表示策略定义上多行文本框演示文稿的字符串值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4df02ea0668d52c8ff553c8ab4c61849e923fc00a80a71264517651ed4c3ad9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152983"
---
# <a name="grouppolicypresentationvaluemultitext-resource-type"></a>groupPolicyPresentationValueMultiText 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示策略定义上多行文本框演示文稿的字符串值。


继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationValueMultiTexts](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-list.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 集合|列出 [groupPolicyPresentationValueMultiText 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 关系。|
|[获取 groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-get.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|读取 [groupPolicyPresentationValueMultiText 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 关系。|
|[创建 groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-create.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|创建新的 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 对象。|
|[删除 groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-delete.md)|无|删除 [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)。|
|[更新 groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-update.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|更新 [groupPolicyPresentationValueMultiText 对象](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期和时间。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|对象的创建日期和时间。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|实体的键。 继承自 [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|String collection|关联的演示文稿的非空字符串的集合。|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueMultiText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    "String"
  ]
}
```




