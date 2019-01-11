---
title: attributeMapping 资源类型
description: 定义同步过程中流给定的目标属性的值应如何。
localization_priority: Normal
ms.openlocfilehash: 6c7a6367684b3e11013355b6d4726afe3346dab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825275"
---
# <a name="attributemapping-resource-type"></a>attributeMapping 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

定义同步过程中流给定的目标属性的值应如何。

## <a name="properties"></a>属性

| 属性                  | 类型                      | 说明    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | 字符串                    |默认值用于以防**source**属性计算结果为`null`。 可选。|
|exportMissingReferences    |字符串                     |仅供内部使用。|
|flowBehavior               |attributeFlowBehavior      |定义此属性时应可导出到目标目录。 可能的值为：`FlowWhenChanged`和`FlowAlways`。 默认值为 `FlowWhenChanged`。 |
|flowType                   |attributeFlowType          |定义此属性时应更新目标目录中。 可能的值为： `Always` （默认）， `ObjectAddOnly` （仅当创建新对象）， `MultiValueAddOnly` （仅当更改正在添加新值到多值属性）。 |
|matchingPriority           |Int32                      |如果大于 0，则此属性将用于执行源和目标目录之间的对象的初始匹配。 同步引擎将尝试查找匹配对象属性使用的第一次匹配优先级最低值。 如果找不到下, 一匹配 priority 属性将使用，依此类推直到找到匹配项，或没有匹配属性会保留。 仅对于预计具有唯一的值，如电子邮件、 属性应用作匹配的属性。|
|源                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | 定义如何值应为源对象中提取 （或转换）。 |
|targetAttributeName        |字符串                     |对目标对象的属性的名称。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
