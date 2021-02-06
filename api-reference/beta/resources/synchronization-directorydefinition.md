---
title: directoryDefinition 资源类型
description: 提供有关目录及其对象的同步引擎信息。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 77af192ff09cf557eec3e73c1973c4c71dc39a96
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134048"
---
# <a name="directorydefinition-resource-type"></a>directoryDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关目录及其对象的同步引擎信息。 例如，此资源告知同步引擎，该目录包含名为 **user** 和 **group** 的对象、这些对象支持哪些属性以及这些属性的类型。 为了使对象和属性参与同步规则和[对象](synchronization-objectmapping.md)映射，[](synchronization-synchronizationrule.md)必须将它们定义为目录定义的一部分。

通常，作为同步模板[](synchronization-synchronizationschema.md)的一部分提供的默认同步架构[](synchronization-synchronizationtemplate.md)将定义该目录最常用的对象和属性。 但是，如果目录支持添加自定义属性，您可能需要使用自己的自定义对象或属性扩展默认定义。 有关详细信息，请参阅"[使用自定义属性配置同步"和](synchronization-configure-with-custom-target-attributes.md)"[配置与目录扩展属性的同步"。](synchronization-configure-with-directory-extension-attributes.md)

目录定义作为同步架构的一 [部分进行更新](synchronization-synchronizationschema.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[发现 directoryDefinition](../api/directorydefinition-discover.md) | [directoryDefinition](synchronization-directorydefinition.md) |发现目录的架构和支持的属性。|

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|id           |字符串     |目录标识符。 不可为 null。|
|metadata       |metadataEntry 集合    |其他扩展属性。 除非明确提到，否则不应更改元数据值。|
|name           |字符串     |目录的名称。 在同步架构中 [必须是唯一的](synchronization-synchronizationschema.md)。 不可为 null。|
|对象        |[objectDefinition](synchronization-objectdefinition.md) 集合    |目录支持的对象的集合。|
|version|String|指示发现的版本的只读值。 如果尚未发现，则为空。|
|discoveryDateTime|DateTimeOffset| 表示使用 ISO 8601 格式的发现日期和时间，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|discoverabilities|string| 只读值，指示应用支持哪种类型的发现。 可取值为：`AttributeDataTypes`、`AttributeNames`、`AttributeReadOnly`、`None`、`ReferenceAttributes`、`UnknownFutureValue`。| 

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


