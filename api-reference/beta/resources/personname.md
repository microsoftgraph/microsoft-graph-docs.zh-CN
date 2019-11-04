---
title: Contact.personname 资源类型
description: Contact.personname 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aad97177a06933d2dd98c5cc94744450197f7dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939598"
---
# <a name="personname-resource-type"></a>Contact.personname 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用户提供的、与其相关联的帐户的扩展名称信息。

继承自[itemFacet](itemfacet.md)。

## <a name="methods"></a>方法

| 方法                                     | 返回类型                 | 说明                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [获取 Contact.personname](../api/personname-get.md) | [Contact.personname](personname.md) | 读取 Contact.personname 对象的属性和关系。 |
| [Update](../api/personname-update.md)      | [Contact.personname](personname.md) | 更新 Contact.personname 对象。                               |
| [删除](../api/personname-delete.md)      | 无                        | 删除 Contact.personname 对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型                              | 说明 |
|:-------------|:----------------------------------|:------------|
|displayName   |String                             | 根据用户或其设备的区域设置，提供 firstName 和 lastName 的顺序呈现。 |
|前         |字符串                             | 用户的名字。                                                                                      |
|initials      |String                             | 用户的首字母缩写。                                                                                        |
|languageTag   |字符串                             | 包含遵循 IETF BCP47 格式的语言（en-us，无 NB，en-us）的名称。                        |
|末          |字符串                             | 用户的姓氏。                                                                                       |
|maiden        |字符串                             | Maiden 用户的名称。                                                                                     |
|中间        |字符串                             | Middlie 用户的名称。                                                                                    | 
|昵称      |字符串                             | 用户的昵称。                                                                                        |
|拼音 |[yomiPersonName](yomipersonname.md)| 有关如何对用户名称进行发音的指南。                                                                 |
|后缀        |字符串                             | Users 名称之后使用的指示符（例如：博士）。                                                             |
|title         |字符串                             | Honorifics 用于为用户名称加前缀（例如： Dr.、罗德、Madam、Mrs）                                            |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personName",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "languageTag": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "pronunciation": {"@odata.type": "microsoft.graph.yomiPersonName"},
  "suffix": "String",
  "title": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->