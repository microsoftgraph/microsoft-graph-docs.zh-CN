---
title: yomiPersonName 资源类型
description: yomiPersonName 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a598c4b5e999b03aeb7201c6eae3a230d3160a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518971"
---
# <a name="yomipersonname-resource-type"></a>yomiPersonName 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为用户提供了一种机制，用于存储有关如何对表示[contact.personname](personname.md)资源的语言的非本机扬声器的名称进行发音的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |String       | 姓和名的发音参考线组合。  |
|前         |String       | 用户名字的发音指南。     |
|末          |String       | 用户姓氏的发音指南。      |
|maiden        |String       | 用户的 maiden 名称的发音指南。    |
|中间        |String       | 用户中间名的发音指南。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.yomiPersonName",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "yomiPersonName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
