---
title: yomiPersonName 资源类型
description: yomiPersonName 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8117dd71947fea41508ccbe7d50d49a4f78b335d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939766"
---
# <a name="yomipersonname-resource-type"></a>yomiPersonName 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为用户提供了一种机制，用于存储有关如何对表示[contact.personname](personname.md)资源的语言的非本机扬声器的名称进行发音的信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                             |
|:-------------|:------------|:--------------------------------------------------------|
|displayName   |String       | 姓和名的发音参考线组合。  |
|前         |字符串       | 用户名字的发音指南。     |
|末          |字符串       | 用户姓氏的发音指南。      |
|maiden        |字符串       | 用户的 maiden 名称的发音指南。    |
|中间        |字符串       | 用户中间名的发音指南。    |

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
