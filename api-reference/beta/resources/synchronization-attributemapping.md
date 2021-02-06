---
title: attributeMapping 资源类型
description: 定义给定目标属性的值在同步期间应该如何流动。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b5f120075b082e50a0f94f05907b413a4c4c4ec6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128748"
---
# <a name="attributemapping-resource-type"></a>attributeMapping 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义给定目标属性的值在同步期间应该如何流动。

## <a name="properties"></a>属性

| 属性                  | 类型                      | 说明    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | 字符串                    |在将源属性求值 **到的情况下使用的** 默认值 `null` 。 可选。|
|exportMissingReferences    |String                     |仅供内部使用。|
|flowBehavior               |attributeFlowBehavior      |定义应何时将此属性导出到目标目录。 可能的值是： `FlowWhenChanged` 和 `FlowAlways` 。 默认值为 `FlowWhenChanged`。 |
|flowType                   |attributeFlowType          |定义应在目标目录中更新此属性的时间。 可能的值是： (默认值) ， (仅在) 创建新对象时， (仅在更改向多值属性中添加新值时 `Always` `ObjectAddOnly` `MultiValueAddOnly`) 。 |
|matchingPriority           |Int32                      |如果大于 0，则此属性将用于在源目录和目标目录之间执行对象的初始匹配。 同步引擎将首先尝试使用具有最低匹配优先级的属性查找匹配对象。 如果未找到，则使用具有下一个匹配优先级的属性，等等，直到找到匹配项或没有更多匹配的属性。 只有预期具有唯一值的属性（如电子邮件）才应用作匹配属性。|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | 定义如何从源对象中提取 (或) 转换值。 |
|targetAttributeName        |字符串                     |目标对象上属性的名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


