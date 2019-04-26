---
title: attributeMapping 资源类型
description: 定义如何在同步过程中传递给定目标属性的值。
localization_priority: Normal
ms.openlocfilehash: 5e44570440790c98755bc5c02091e8fe31f3fc26
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345621"
---
# <a name="attributemapping-resource-type"></a>attributeMapping 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义如何在同步过程中传递给定目标属性的值。

## <a name="properties"></a>属性

| 属性                  | 类型                      | 说明    |
|:--------------------------|:--------------------------|:---------------|
|默认               | String                    |要在对`null`**源**属性进行求值的情况下使用的默认值。 可选。|
|exportMissingReferences    |String                     |仅供内部使用。|
|flowBehavior               |attributeFlowBehavior      |定义何时应将此属性导出到目标目录。 可能的值为`FlowWhenChanged` : `FlowAlways`和。 默认值为 `FlowWhenChanged`。 |
|flowType                   |attributeFlowType          |定义应何时在目标目录中更新此属性。 可能的值为`Always` : (默认值`ObjectAddOnly` ), (仅在创建新对象时`MultiValueAddOnly` ) (仅当更改将新值添加到多值属性时)。 |
|matchingPriority           |Int32                      |如果高于 0, 则此属性将用于执行源目录和目标目录之间的对象的初始匹配。 同步引擎将尝试使用具有最小匹配优先级值的属性来查找匹配的对象。 如果未找到, 则将使用具有下一个匹配的优先级的属性, 在找到匹配项或不留下更多匹配属性的情况下, 将使用该属性。 应仅将应具有唯一值的属性 (如电子邮件) 用作匹配属性。|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | 定义应如何从源对象提取 (或转换) 值。 |
|targetAttributeName        |String                     |目标对象上的属性的名称。 |

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
