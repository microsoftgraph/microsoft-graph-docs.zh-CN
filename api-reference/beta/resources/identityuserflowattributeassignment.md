---
title: identityUserFlowAttributeAssignment 资源类型
description: identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80bc6547307914e0d206ea9b5c79073f96fce19c
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581291"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>identityUserFlowAttributeAssignment 资源类型

命名空间：microsoft.graph

identityUserFlowAttributeAssignments 用于收集用户流中的特定 identityUserFlowAttributes。 这允许控制在用户流中收集的属性，并提供有关如何在用户流中收集属性的自定义选项。 您可以在单个用户流中拥有多个 identityUserFlowAttributeAssignments，以创建最终用户在注册过程中看到的体验，如果要求提供用户流完成注册所需的信息。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[获取 identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-get.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|读取 identityUserFlowAttributeAssignment 对象的属性和关系。|
|[更新 identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-update.md)|无|更新 identityUserFlowAttributeAssignment 对象的属性。|
|[删除 identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-delete.md)|无|删除特定的 identityUserFlowAttributeAssignment 对象。|
|[getOrder](../api/identityuserflowattributeassignment-getorder.md)|[assignmentOrder](../resources/assignmentorder.md)|获取在用户流中收集的 identityUserFlowAttributes 的顺序。|
|[setOrder](../api/identityuserflowattributeassignment-setorder.md)|无|设置在用户流中收集的 identityUserFlowAttributes 的顺序。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|IdentityUserFlowAttributeAssignment 的标识符。 此标识符在创建后是不可变的。 这是一个只读属性。|
|displayName|String|用户流中的 identityUserFlowAttribute 的显示名称。|
|isOptional|布尔值|确定 identityUserFlowAttribute 是否为可选。 `true` 表示用户不必提供值。 `false` 表示用户无法完成注册，而无需提供值。|
|requiresVerification|布尔值|确定 identityUserFlowAttribute 是否需要验证。 这仅用于验证用户的电话号码或电子邮件地址。|
|userAttributeValues|[userAttributeValuesItem](../resources/userattributevaluesitem.md) 集合|用户流属性的输入选项。 仅当 userInputType 为、或时才适用 `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` 。|
|userInputType|identityUserFlowAttributeInputType|用户流属性的输入类型。 可取值为：`textBox`、`dateTimeDropdown`、`radioSingleSelect`、`dropdownSingleSelect`、`emailBox`、`checkboxMultiSelect`。|

## <a name="relationships"></a>关系

|关系|类型|Description|
|:---|:---|:---|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|要添加到用户流中的用户属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "baseType": "",
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
