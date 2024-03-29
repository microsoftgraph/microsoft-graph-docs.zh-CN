---
title: alertTrigger 资源类型
description: 包含有关触发检测的属性的信息， (警报实体中的属性) 。
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 78cfe6afd2495291dd3d4b358ab500b41dab25d0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089877"
---
# <a name="alerttrigger-resource-type"></a>alertTrigger 资源类型

命名空间：microsoft.graph

包含有关触发检测的属性的信息， (警报实体中的属性) 。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|name|String|充当检测触发器的属性的名称。|
|type|String|用于解释的 key：value 对中的属性类型。 例如，String、Boolean 等。|
|value|String|用作检测触发器的属性的值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}
```

## <a name="example"></a>示例

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

