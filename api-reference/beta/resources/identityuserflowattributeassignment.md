---
title: identityUserFlowAttributeAssignment 资源类型
description: identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0b1b0addc48b96eeb3f19c9acf2a8b01e8891efb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440225"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>identityUserFlowAttributeAssignment 资源类型

命名空间：microsoft.graph

identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。 这允许控制在用户流中收集的属性，并提供自定义选项，了解如何在用户流中收集属性。 您可以在单个用户流中拥有多个 identityUserFlowAttributeAssignments，该流可在要求最终用户提供用户流完成注册所需的信息时创建最终用户在注册期间看到的体验。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[获取 identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-get.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|读取 identityUserFlowAttributeAssignment 对象的属性和关系。|
|[更新 identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-update.md)|无|更新 identityUserFlowAttributeAssignment 对象的属性。|
|[删除 identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-delete.md)|无|删除特定 identityUserFlowAttributeAssignment 对象。|
|[getOrder](../api/identityuserflowattributeassignment-getorder.md)|[assignmentOrder](../resources/assignmentorder.md)|获取在用户流中收集的 identityUserFlowAttributes 的顺序。|
|[setOrder](../api/identityuserflowattributeassignment-setorder.md)|无|设置在用户流中收集的 identityUserFlowAttributes 的顺序。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|identityUserFlowAttributeAssignment 的标识符。 此标识符创建后不可变。 这是一个只读属性。|
|displayName|String|标识显示名称流中的 identityUserFlowAttribute 的项。|
|isOptional|布尔|确定 identityUserFlowAttribute 是否可选。 `true` 表示用户不必提供值。 `false` 表示用户无法在未提供值的情况下完成注册。|
|requiresVerification|布尔|确定 identityUserFlowAttribute 是否需要验证。 这仅用于验证用户的电话号码或电子邮件地址。|
|userAttributeValues|[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合|用户流属性的输入选项。 仅在 userInputType 为 `radioSingleSelect` ，或 `dropdownSingleSelect` 时适用 `checkboxMultiSelect` 。|
|userInputType|identityUserFlowAttributeInputType|用户流属性的输入类型。 可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|要添加到用户流中的用户属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
  "id": "String (identifier)",
  "isOptional": "Boolean",
  "requiresVerification": "Boolean",
  "userInputType": "String",
  "userAttributeValues": [
    {
      "@odata.type": "microsoft.graph.userAttributeValuesItem"
    }
  ],
  "displayName": "String"
}
```
