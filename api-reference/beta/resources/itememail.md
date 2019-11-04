---
title: itemEmail 资源类型
description: itemEmail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: eed73f61b281463848c8520ebdcdbc75ac26d29d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939332"
---
# <a name="itememail-resource-type"></a>itemEmail 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关与用户相关联的电子邮件地址的详细信息。

## <a name="methods"></a>方法

| 方法                                   | 返回类型               | 说明                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [Get](../api/itememail-get.md) | [itemEmail](itememail.md) | 读取**itemEmail**对象的属性和关系。 |
| [Update](../api/itememail-update.md)     | [itemEmail](itememail.md) | 更新**itemEmail**对象。                               |
| [删除](../api/itememail-delete.md)     | 无                      | 删除**itemEmail**对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型        | 描述                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|address       |String       | 电子邮件地址本身。                                                 |
|displayName   |字符串       | 用户与特定电子邮件地址相关联的名称或标签。  |
|类型          |字符串       | 可取值为：`unknown`、`work`、`personal`、`main`、`other`。      |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": ""
}-->

```json
{
  "address": "String",
  "displayName": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemEmail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
