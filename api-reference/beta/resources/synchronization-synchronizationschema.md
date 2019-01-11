---
title: synchronizationSchema 资源类型
description: 定义对象将同步和同步方式。 同步架构包含特定同步作业的设置信息的大部分。 通常情况下，您将自定义某些属性的映射，或添加范围筛选器同步只有满足特定条件的对象。
localization_priority: Normal
ms.openlocfilehash: 696bdbbc6fa2d96965d11a12fb09fdfc0ce16106
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847318"
---
# <a name="synchronizationschema-resource-type"></a>synchronizationSchema 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

定义对象将同步和同步方式。 同步架构包含特定同步作业的设置信息的大部分。 通常情况下，您将自定义某些[属性映射](synchronization-attributemapping.md)，或添加[范围筛选器](synchronization-filter.md)以同步只有满足特定条件的对象。

以下各节介绍了同步架构的高级组件。

## <a name="directory-definitions"></a>目录定义

[目录定义](synchronization-directorydefinition.md)提供有关目录和其对象的同步引擎信息。 例如，目录定义告知同步引擎 Azure AD 目录具有名为**用户**和**组**，这些对象，并为这些属性的类型支持哪些属性的对象。 为了在同步规则/对象映射中使用的特定对象和属性，他们必须定义为目录定义的一部分。

## <a name="synchronization-rules"></a>同步规则

[同步规则](synchronization-synchronizationrule.md)是同步安装程序的核心。 它们为同步引擎定义应如何执行的同步、 包括哪些对象应保持同步，从源目录对象与目标目录中的对象的匹配方式，并且应属性的方式转换他们正在同步时从源到目标目录。 

## <a name="object-mappings"></a>对象映射

[对象映射](synchronization-objectmapping.md)是同步规则的主要部分。 每个对象映射定义如何给定的对象应同步从源到目标目录。 具体而言，映射定义源目录中的对象与目标目录中某个对象的匹配方式什么 （如果有） 范围筛选器应使用决定是否设置一个对象，以及应如何转换对象属性他们正在同步时从源到目标目录。

## <a name="methods"></a>方法

| 方法        | 返回类型               | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|[获取架构](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |读取属性和**synchronizationSchema**对象的关系。|
|[更新架构](../api/synchronization-synchronizationschema-update.md)    |无   |更新同步架构。 |
|[删除架构](../api/synchronization-synchronizationschema-delete.md)    |无   |删除自定义的架构，重置为默认配置的架构。 |
|[列表筛选器运算符](../api/synchronization-synchronizationschema-filteroperators.md)    |[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合   |列出所有支持的范围筛选器中的运算符。 |
|[List 属性映射函数](../api/synchronization-synchronizationschema-functions.md)    |[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合   |列出属性映射表达式中支持的所有功能。 |
|[分析属性映射表达式](../api/synchronization-synchronizationschema-parseexpression.md)|[parseExpressionResponse](synchronization-parseexpressionresponse.md)|分析 [attributeMappingSource 字符串表达式|(../ resources/synchronization_attributemappingsource.md) 对象。|


## <a name="properties"></a>属性

| 属性      | 类型      | Description    |
|:--------------|:----------|:---------------|
|directories            |[directoryDefinition](synchronization-directorydefinition.md)集合   |描述目录和[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)的一部分的对象。 |
|synchronizationRules   |[synchronizationRule](synchronization-synchronizationrule.md)集合   |同步规则[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)，配置的集合 |
|version                |String                             |架构，每次架构更改自动更新的版本。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
