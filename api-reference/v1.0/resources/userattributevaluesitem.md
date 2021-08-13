---
title: userAttributeValuesItem 资源类型
description: 表示用户流中的用户流属性值。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 88e19bfa02876e08df4c3040ff6bcfefae41840278719b83ccc7b57be651f5a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205211"
---
# <a name="userattributevaluesitem-resource-type"></a>userAttributeValuesItem 资源类型

命名空间：microsoft.graph

表示用户流中的用户流属性值，当有多个选择可供选择时。  userAttributeValuesItem 适用于 、 和 的 userInputTypes，适用于 `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isDefault|Boolean|确定是否将该值设置为默认值。|
|name|String|在显示名称流中向用户显示的属性的行数。|
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
