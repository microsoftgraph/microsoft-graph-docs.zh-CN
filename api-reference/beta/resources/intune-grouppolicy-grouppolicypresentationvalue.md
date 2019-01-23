---
title: groupPolicyPresentationValue 资源类型
description: 基本演示文稿值实体存储的一个组策略演示文稿的值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec299eccc29ddcb39ece0d1f6c0e063a02192909
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429287"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>groupPolicyPresentationValue 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

基本演示文稿值实体存储的一个组策略演示文稿的值。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 groupPolicyPresentationValues](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)集合|列出属性和[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象之间的关系。|
|[获取 groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|读取属性和[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的关系。|
|[创建 groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|创建新的[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象。|
|[删除 groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|无|删除[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)。|
|[更新 groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|更新[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|日期和时间上次修改对象。|
|createdDateTime|DateTimeOffset|日期和时间创建对象。|
|id|String|实体的键。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|关联的演示文稿值的组策略定义值。|
|演示文稿|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|组策略演示的演示文稿值相关联。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```




