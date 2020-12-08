---
title: userAttributeValuesItem 资源类型
description: 当有多个选择可供选择时，用于填充用户流中用户流属性的值。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6fd0d582ef4dcdd83dba6947536c5acdbc14a8cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581323"
---
# <a name="userattributevaluesitem-resource-type"></a>userAttributeValuesItem 资源类型

命名空间：microsoft.graph

当有多个选择可供选择时，用于填充用户流中用户流属性的值。 userAttributeValuesItem 适用于 userInputTypes `radioSingleSelect` 、 `dropdownSingleSelect` 和 `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md)。

## <a name="properties"></a>属性

|属性|类型|Description|
|:---|:---|:---|
|isDefault|Boolean|用于将值设置为默认值。|
|name|String|在用户流中向最终用户显示的属性的显示名称。|
|value|String|选择此项时设置的值。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAttributeValuesItem"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userAttributeValuesItem",
  "name": "String",
  "value": "String",
  "isDefault": "Boolean"
}
```
