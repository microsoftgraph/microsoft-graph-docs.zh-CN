---
title: 架构资源类型
description: 介绍内容的类型，以及如何在 Microsoft Search 连接中对项目中的每个属性编制索引。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8bd5d47f444d7054aecbf7b0a63e57643837a340
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938784"
---
# <a name="schema-resource-type"></a>架构资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍内容的类型，以及如何在 Microsoft Search[连接](externalconnection.md)中对项目中的每个属性编制索引。

## <a name="methods"></a>方法

| 方法                                                    | 返回类型                   | 说明 |
|:----------------------------------------------------------|:------------------------------|:--|
| [创建架构](../api/externalconnection-post-schema.md) | 无*或*[架构](schema.md) | 注册连接架构。 |
| [获取架构](../api/schema-get.md)                        | [架构](schema.md)           | 读取架构对象的属性。 |

## <a name="properties"></a>属性

| 属性   | 类型                               | 描述                |
|:-----------|:-----------------------------------|:---------------------------|
| #c1   | 字符串                             | 可能的值为 `microsoft.graph.externalItem` 和 `microsoft.graph.externalFile`。 必填。 |
| properties | [属性](property.md)集合 | 为连接中的项目定义的属性。 最小属性数为1，最大值为64。 在设置`baseType`为`microsoft.graph.externalItem`时所需的。 当设置`baseType`为时， `microsoft.graph.externalFile`将忽略。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [{"@odata.type": "microsoft.graph.property"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
