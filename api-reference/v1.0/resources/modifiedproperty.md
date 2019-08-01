---
title: modifiedProperty 资源类型
description: 指示 Azure AD 资源中已修改的所有属性, 包括旧值和新值。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 0c5375ea3e188d6023e3588531e07877f6de38ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036097"
---
# <a name="modifiedproperty-resource-type"></a>modifiedProperty 资源类型

指示 Azure AD 资源中已修改的所有属性, 包括旧值和新值。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName|String|指示已更改的目标属性的属性名称。|
|NewValue|String|指示值的更新值。|
|oldValue|String|指示属性的前一个值 (在更新之前)。|

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
