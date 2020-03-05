---
title: 架构资源类型
description: 介绍内容的类型，以及如何在 Microsoft Search 连接中对项目中的每个属性编制索引。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 40c31536f8d53c46563fda4205d34deee0501beb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520954"
---
# <a name="schema-resource-type"></a>架构资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍内容的类型，以及如何在 Microsoft Search[连接](externalconnection.md)中对项目中的每个属性编制索引。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法                                                    | 返回类型                   | 说明 |
|:----------------------------------------------------------|:------------------------------|:--|
| [创建架构](../api/externalconnection-post-schema.md) | 无*或*[架构](schema.md) | 注册连接架构。 |
| [获取架构](../api/schema-get.md)                        | [schema](schema.md)           | 读取架构对象的属性。 |

## <a name="properties"></a>属性

| 属性   | 类型                               | 说明                |
|:-----------|:-----------------------------------|:---------------------------|
| #c1   | String                             | 可能的值为 `microsoft.graph.externalItem` 和 `microsoft.graph.externalFile`。 必填。 |
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
