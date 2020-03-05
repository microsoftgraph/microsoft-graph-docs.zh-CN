---
title: personAnniversary 资源类型
description: personAnniversary 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7dad5536eb78b2d7119ace63eb0f7ce16880e85f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521923"
---
# <a name="personanniversary-resource-type"></a>personAnniversary 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示与用户[配置文件](profile.md)中的人员关联的有意义日期的详细信息。

继承自[itemFacet](itemFacet.md)。

## <a name="methods"></a>方法

| 方法                                                   | 返回类型                               | 说明                                                    |
|:---------------------------------------------------------|:------------------------------------------|:---------------------------------------------------------------|
| [获取 personAnniversary](../api/personanniversary-get.md) | [personAnniversary](personanniversary.md) | 读取**personAnniversary**对象的属性和关系。 |
| [更新](../api/personanniversary-update.md)             | [personAnniversary](personanniversary.md) | 更新**personAnniversary**对象。                               |
| [删除](../api/personanniversary-delete.md)             | 无                                      | 删除**personAnniversary**对象。                               |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|date          |Date         | 包含与周年纪念类型相关联的日期。         |
|类型          |string       | 可取值为：`birthday`、`wedding`、`unknownFutureValue`。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": ""
}-->

```json
{
  "date": "String (timestamp)",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personAnniversary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
