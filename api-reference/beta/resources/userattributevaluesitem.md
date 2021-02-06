---
title: userAttributeValuesItem 资源类型
description: 用于在用户流中有多个选项可供选择时填充用户流属性的值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64b2416cd6fd0e8c92d9a00ff2d599226e3cd02c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133019"
---
# <a name="userattributevaluesitem-resource-type"></a>userAttributeValuesItem 资源类型

命名空间：microsoft.graph

用于在用户流中有多个选项可供选择时填充用户流属性的值。 userAttributeValuesItem 适用于 userInputTypes `radioSingleSelect` `dropdownSingleSelect` 和 `checkboxMultiSelect` [identityUserFlowAttributeAssignment。](..\resources\identityuserflowattributeassignment.md)

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isDefault|Boolean|用于将值设置为默认值。|
|name|字符串|在显示名称流中向最终用户显示的属性的列表。|
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
