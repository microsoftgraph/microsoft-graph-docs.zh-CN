---
title: modifiedProperty 资源类型
description: 指示已修改的 Azure AD 资源上的所有属性，包括旧值和新值。
ms.localizationpriority: medium
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4c74e492b50435b7911952ffe32107008db11330
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067071"
---
# <a name="modifiedproperty-resource-type"></a>modifiedProperty 资源类型

命名空间：microsoft.graph

指示已修改的 Azure AD 资源上的所有属性，包括旧值和新值。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String|指示已更改的目标属性的属性名称。|
|NewValue|String|指示属性的更新值。|
|oldValue|String|指示更新前 (属性) 值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

