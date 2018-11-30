---
title: attributeDefinition 资源类型
description: 描述对象的属性。
ms.openlocfilehash: 2199f8dbe5c528cf3b1b73f007fdae3451833815
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048339"
---
# <a name="attributedefinition-resource-type"></a>attributeDefinition 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

描述对象的属性。

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|定位         |布尔    | `true`如果属性应用作对象的定位标记。 定位属性必须具有识别对象的唯一值，并且必须变。 默认值为 `false`。 有，并且只有一个对象的属性必须被指定为定位标记为支持同步。 |
|caseExact      |布尔    |`true`如果此属性的值应处理，区分大小写。 此设置会影响如何同步引擎检测到的属性的更改。|
|元数据       |[metadataEntry](../resources/synchronization-metadataentry.md)    |其他扩展属性。 除非明确提到，不应更改元数据值。|
|多值    |布尔    |`true`如果属性可以有多个值。 默认值为 `false`。|
|mutability     |字符串     |属性可变性。 可能的值为： `ReadWrite`， `ReadOnly`， `Immutable`， `WriteOnly`。 默认值为 `ReadWrite`。|
|name           |字符串     |属性的名称。 必须是唯一对象定义中。 不可为 null。|
|必需       |布尔    |`true`如果属性是必需的。 如果缺少任何所需的属性，则不可以创建对象。 如果同步期间，required 的属性的值，将使用的默认值。 如果未设置默认值，则同步将记录错误。|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) |使用属性的`reference`键入，列表被引用的对象 (例如，`manager`属性将列出`User`为引用的对象)。|
|type           |字符串     |属性值类型。 可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。 默认值为 `String`。|

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->