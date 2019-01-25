---
title: synchronizationRule 资源类型
description: 定义同步引擎，包括要同步的对象和方向，应如何执行同步如何从源目录对象应匹配目标目录中的对象以及如何属性应转换他们正在同步时从源到目标目录。
localization_priority: Normal
ms.openlocfilehash: deaf27ec46268eebe289e502bdf3b62a659cf1fb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517923"
---
# <a name="synchronizationrule-resource-type"></a>synchronizationRule 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义同步引擎，包括要同步的对象和方向，应如何执行同步如何从源目录对象应匹配目标目录中的对象以及如何属性应转换他们正在同步时从源到目标目录。

>**注意：** 同步规则定义一个方向-从到目标目录源目录同步。 规则属性的一部分定义的源和目标目录。

同步规则更新[同步架构](synchronization-synchronizationschema.md)的一部分。

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|可编辑       |Boolean    |`true`如果可以自定义同步规则;，`false`如果此规则是只读的并且不应被更改。|
|id             |String     |同步规则标识符。 必须是同步引擎识别的标识符。 支持标识符可以找到 API 返回的同步模板中的规则。|
|元数据       |[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)集合 |其他扩展属性。 除非明确由支持团队，不应更改元数据值。|
|name           |String     |可读同步规则的名称。 不可为 null。|
|objectMappings |[objectMapping](synchronization-objectmapping.md)集合    |规则支持的对象映射的集合。 指示同步引擎应同步的对象。|
|priority       |整数    |相对于[synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。 将首先处理与最低优先级编号的规则。|
|sourceDirectoryName       |String    |源目录的名称。 必须匹配[synchronizationSchema](synchronization-synchronizationschema.md)中的目录定义之一。|
|targetDirectoryName       |String    |目标目录的名称。 必须匹配[synchronizationSchema](synchronization-synchronizationschema.md)中的目录定义之一。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationrule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
