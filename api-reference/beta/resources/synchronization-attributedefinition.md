---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a9c50721c1ee19505edc2507313cc346a6adabfd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956811"
---
# <a name="attributedefinition-resource-type"></a>attributeDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述对象的属性。

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|anchor         |Boolean    | `true` 属性是否用作对象的定位标记。 定位属性必须具有标识对象的唯一值，并且必须是不可变的。 默认值为 `false`。 必须将对象属性中的一个（且只有一个）指定为支持同步的定位标记。 |
|caseExact      |Boolean    |`true` 如果此属性的值应视为区分大小写。 此设置会影响同步引擎检测属性更改。|
|flowNullValues |Boolean    |"true"表示允许属性为 null 值。|
|metadata       |[metadataEntry](../resources/synchronization-metadataentry.md) 集合   |其他扩展属性。 除非明确提到，否则不应更改元数据值。|
|多值    |Boolean    |`true` 如果一个属性可以有多个值。 默认值为 `false`。|
|可变性     |可变性     |属性的可变性。 可能的值是 `ReadWrite` `ReadOnly` `Immutable` ：、、、。 `WriteOnly` 默认值为 `ReadWrite`。|
|name           |String     |属性的名称。 在对象定义中必须是唯一的。 不可为 null。|
|必需       |Boolean    |`true` 如果 属性是必需的。 如果缺少任何必需的属性，则不能创建对象。 如果在同步期间，所需的属性没有值，则使用默认值。 如果未设置默认值，则同步将记录错误。|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) 集合 |对于类型为 的属性，列出引用 (例如，该属性将列出为引用 `reference` `manager` `User` 的对象) 。|
|type           |attributeType     |属性值类型。 可能的值是 `String` `Integer` `Reference` ：、、、、、。 `Binary` `Boolean` `DateTime` 默认值为“`String`”。|

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


