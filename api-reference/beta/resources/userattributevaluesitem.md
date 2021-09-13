---
title: userAttributeValuesItem 资源类型
description: 用于在用户流中有多个选项可供选择时填充用户流属性的值。
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3468ed1545c8be12f906182f34f5260897f461ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056996"
---
# <a name="userattributevaluesitem-resource-type"></a>userAttributeValuesItem 资源类型

命名空间：microsoft.graph

用于在用户流中有多个选项可供选择时填充用户流属性的值。 userAttributeValuesItem 适用于 userInputTypes `radioSingleSelect` 、 `dropdownSingleSelect` 和 `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|isDefault|Boolean|用于将该值设置为默认值。|
|name|String|在显示名称流中向最终用户显示的属性的列表。|
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
