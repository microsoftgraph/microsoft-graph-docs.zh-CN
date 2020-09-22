---
title: 架构资源类型
description: 连接架构确定如何将内容添加到连接中，以用于各种 Microsoft Graph 体验。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ff14f04adb31d99aadec15cb9368e09a098c7a26
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192866"
---
# <a name="schema-resource-type"></a>架构资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[连接](externalconnection.md)架构确定如何将外部内容用于各种 Microsoft Graph 体验。 架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。 在将项目添加到连接之前，必须注册架构。

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>方法

| 方法                                                    | 返回类型                   | 说明 |
|:----------------------------------------------------------|:------------------------------|:--|
| [创建架构](../api/externalconnection-post-schema.md) | 无*或*[架构](schema.md) | 注册连接架构。 |
| [获取架构](../api/schema-get.md)                        | [schema](schema.md)           | 读取架构对象的属性。 |

## <a name="properties"></a>属性

| 属性   | 类型                               | 描述                |
|:-----------|:-----------------------------------|:---------------------------|
| #c1   | 字符串                             | 必须设置为 `microsoft.graph.externalItem`。 必需。 |
| properties | [属性](property.md) 集合 | 为连接中的项目定义的属性。 最小属性数为1，最大值为128。 |

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


