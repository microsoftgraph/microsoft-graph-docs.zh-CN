---
title: synchronizationRule 资源类型
description: 定义如何对同步引擎执行同步。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 94697fede9ab9055b1a477cfd94edea88f207331
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135994"
---
# <a name="synchronizationrule-resource-type"></a>synchronizationRule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义应为同步引擎执行同步的方式，包括要同步的对象以及方向、源目录中的对象如何与目标目录中的对象匹配，以及属性从源目录同步到目标目录时如何转换属性。

>**注意：** 同步规则在一个方向定义同步 - 从源目录到目标目录。 源目录和目标目录定义为规则属性的一部分。

同步规则作为同步架构的一 [部分进行更新](synchronization-synchronizationschema.md)。

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|可编辑       |Boolean    |`true` 同步规则是否可自定义; `false` 如果此规则是只读的且不应更改。|
|id             |字符串     |同步规则标识符。 必须是同步引擎识别的标识符之一。 可以在 API 返回的同步模板中找到受支持的规则标识符。|
|metadata       |[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md) 集合 |其他扩展属性。 除非支持团队明确指示，否则不应更改元数据值。|
|name           |字符串     |同步规则的可读名称。 不可为 null。|
|objectMappings |[objectMapping](synchronization-objectmapping.md) 集合    |规则支持的对象映射的集合。 告知同步引擎应同步哪些对象。|
|priority       |整数    |相对于 [synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。 优先级最低的规则将首先进行处理。|
|sourceDirectoryName       |字符串    |源目录的名称。 必须与 synchronizationSchema 中的目录定义 [之一匹配](synchronization-synchronizationschema.md)。|
|targetDirectoryName       |字符串    |目标目录的名称。 必须与 synchronizationSchema 中的目录定义 [之一匹配](synchronization-synchronizationschema.md)。|

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
  "suppressions": []
}
-->


