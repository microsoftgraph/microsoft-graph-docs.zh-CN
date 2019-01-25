---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514339"
---
# <a name="attributedefinition-resource-type"></a>attributeDefinition 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述对象的属性。

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|Anchor         |Boolean    | `true`如果属性应用作对象的定位标记。 定位属性必须具有识别对象的唯一值，并且必须变。 默认值为 `false`。 有，并且只有一个对象的属性必须被指定为定位标记为支持同步。 |
|caseExact      |Boolean    |`true`如果此属性的值应处理，区分大小写。 此设置会影响如何同步引擎检测到的属性的更改。|
|元数据       |[metadataEntry](../resources/synchronization-metadataentry.md)    |其他扩展属性。 除非明确提到，不应更改元数据值。|
|多值    |Boolean    |`true`如果属性可以有多个值。 默认值为 `false`。|
|mutability     |String     |属性可变性。 可取值为：`ReadWrite`、`ReadOnly`、`Immutable`、`WriteOnly`。 默认值为 `ReadWrite`。|
|name           |String     |属性的名称。 必须是唯一对象定义中。 不可为 null。|
|必需       |Boolean    |`true`如果属性是必需的。 如果缺少任何所需的属性，则不可以创建对象。 如果同步期间，required 的属性的值，将使用的默认值。 如果未设置默认值，则同步将记录错误。|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) |使用属性的`reference`键入，列表被引用的对象 (例如，`manager`属性将列出`User`为引用的对象)。|
|type           |String     |属性值类型。 可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。 默认值为 `String`。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
