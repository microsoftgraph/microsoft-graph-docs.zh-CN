---
title: synchronizationRule 资源类型
description: 定义同步引擎应如何执行同步。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0698afb7e3584aa1d4cd6697504138f6262e5141
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217365"
---
# <a name="synchronizationrule-resource-type"></a>synchronizationRule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义同步引擎的同步执行方式，包括要同步的对象和方向、源目录中的对象与目标目录中的对象的匹配方式以及在从源同步到目标目录时应如何转换属性。

>**注意：** 同步规则将一个方向的同步定义为将源目录中的同步到目标目录。 源和目标目录定义为规则属性的一部分。

同步规则将作为[同步架构](synchronization-synchronizationschema.md)的一部分进行更新。

## <a name="properties"></a>属性

| 属性      | 类型      | Description    |
|:--------------|:----------|:---------------|
|变为       |Boolean    |`true`如果可以对同步规则进行自定义，则为  ;`false`如果此规则为只读，则不应更改。|
|id             |String     |同步规则标识符。 必须是同步引擎可识别的标识符之一。 在 API 返回的同步模板中可以找到受支持的规则标识符。|
|metadata       |[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)集合 |其他扩展属性。 除非支持团队明确指示，否则不应更改元数据值。|
|name           |字符串     |可读的同步规则名称。 不可为空。|
|objectMappings |[objectMapping](synchronization-objectmapping.md)集合    |该规则支持的对象映射的集合。 通知同步引擎应同步哪些对象。|
|priority       |整数    |相对于[synchronizationSchema](synchronization-synchronizationschema.md)中其他规则的优先级。 将首先处理具有最低优先级编号的规则。|
|sourceDirectoryName       |字符串    |源目录的名称。 必须与[synchronizationSchema](synchronization-synchronizationschema.md)中的一个目录定义相匹配。|
|targetDirectoryName       |字符串    |目标目录的名称。 必须与[synchronizationSchema](synchronization-synchronizationschema.md)中的一个目录定义相匹配。|

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
