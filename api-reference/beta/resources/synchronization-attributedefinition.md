---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 34503f3edf15542db449d56e5211cd33b3d9132e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128811"
---
# <a name="attributedefinition-resource-type"></a>attributeDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述对象的属性。

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|anchor         |Boolean    | `true` 属性是否用作对象的定位标记。 定位属性必须具有标识对象的唯一值，并且必须是不可变的。 默认值为 `false`。 必须将一个（且只有一个）对象的属性指定为支持同步的定位标记。 |
|caseExact      |Boolean    |`true` 如果应当将此属性的值视为区分大小写。 此设置会影响同步引擎检测属性的更改。|
|flowNullValues |Boolean    |如果为"true"，则属性为 null 值。|
|metadata       |[metadataEntry](../resources/synchronization-metadataentry.md) 集合   |其他扩展属性。 除非明确提到，否则不应更改元数据值。|
|multivalued    |Boolean    |`true` 如果一个属性可以有多个值。 默认值为 `false`。|
|可变性     |字符串     |属性的可变性。 可能的值是：  `ReadWrite` `ReadOnly` ， ， `Immutable` `WriteOnly` 。 默认值为 `ReadWrite`。|
|name           |字符串     |属性的名称。 在对象定义中必须是唯一的。 不可为 null。|
|必需       |Boolean    |`true` 如果属性是必需的。 如果缺少任何必需的属性，则不能创建对象。 如果在同步期间，所需的属性没有值，则使用默认值。 如果未设置默认值，同步将记录错误。|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) 集合 |对于具有类型的属性，列出引用的对象 (例如，该属性将作为引用的对象列表 `reference` `manager` `User`) 。|
|type           |字符串     |属性值类型。 可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。 默认值为“`String`”。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "flowNullValues": true,
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


