---
title: userAttributeValuesItem 资源类型
description: 表示用户流中的用户流属性值。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 690b9f53762359ab559fb98534525cad15e5e282
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083962"
---
# <a name="userattributevaluesitem-resource-type"></a>userAttributeValuesItem 资源类型

命名空间：microsoft.graph

表示用户流中的用户流属性值，当有多个选择可供选择时。  userAttributeValuesItem 适用于 、 和 的 userInputTypes，适用于 `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isDefault|Boolean|确定是否将该值设置为默认值。|
|name|String|在显示名称流中向用户显示的属性的列表。|
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
