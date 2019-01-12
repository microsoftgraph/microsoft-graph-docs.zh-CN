---
title: alertTrigger 资源类型
description: 包含有关触发检测属性的信息 （警报实体中存在属性）。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991256"
---
# <a name="alerttrigger-resource-type"></a>alertTrigger 资源类型

包含有关触发检测属性的信息 （警报实体中存在属性）。

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|name|字符串|充当检测触发器属性的名称。|
|type|字符串|用于解释： 键值对中属性的类型。 例如，String、 Boolean、 等。|
|值|字符串|充当检测触发器属性的值。|

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
