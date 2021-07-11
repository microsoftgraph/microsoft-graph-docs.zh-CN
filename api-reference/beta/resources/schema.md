---
title: 架构资源类型
description: 连接架构确定添加到连接的内容如何用于各种 Microsoft Graph体验。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6bcb5d7b10a71f6031a4215fe9f0c294c5af1840
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366938"
---
# <a name="schema-resource-type"></a>架构资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[连接](externalconnection.md)架构确定外部内容如何用于各种 Microsoft Graph体验。 架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。 向连接添加项目前，必须注册架构。

## <a name="methods"></a>方法

| 方法                                                    | 返回类型                   | 说明 |
|:----------------------------------------------------------|:------------------------------|:--|
| [创建架构](../api/externalconnection-post-schema.md) | 无 *或*[架构](schema.md) | 注册连接架构。 |
| [获取架构](../api/schema-get.md)                        | [schema](schema.md)           | 读取架构对象的属性。 |

## <a name="properties"></a>属性

| 属性   | 类型                               | 说明                |
|:-----------|:-----------------------------------|:---------------------------|
| baseType   | String                             | 必须设置为 `microsoft.graph.externalItem`。 必填。 |
| properties | [property](property.md) 集合 | 为连接中的项目定义的属性。 最小属性数为 1，最大值为 128。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
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


