---
title: synchronizationSchema 资源类型
description: 定义将同步的对象以及同步的对象。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d463fa5a00318936ef0f1612f233851e42a9db11
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846133"
---
# <a name="synchronizationschema-resource-type"></a>synchronizationSchema 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义将同步的对象以及同步的对象。 同步架构包含特定同步作业的大部分安装信息。 通常情况下，您将自定义一些[属性映射](synchronization-attributemapping.md)，或添加[作用域筛选器](synchronization-filter.md)以仅同步满足特定条件的对象。

以下各节介绍了同步架构的高级组件。

## <a name="directory-definitions"></a>目录定义

[目录定义](synchronization-directorydefinition.md)提供有关目录及其对象的同步引擎信息。 例如，目录定义告知同步引擎： Azure AD 目录包含名为**user**和**group**的对象，这些对象支持哪些属性以及这些属性的类型。 为了在同步规则/对象映射中使用特定对象和属性，必须将其定义为目录定义的一部分。

## <a name="synchronization-rules"></a>同步规则

[同步规则](synchronization-synchronizationrule.md)是同步设置的核心。 它们定义同步引擎应如何执行同步，包括应同步的对象、源目录中的对象与目标目录中的对象的匹配方式以及应如何在将属性从源同步到目标目录时转换属性。

## <a name="object-mappings"></a>对象映射

[对象映射](synchronization-objectmapping.md)是同步规则的主要部分。 每个对象映射定义应如何将给定对象从源同步到目标目录。 特别是，映射定义源目录中的对象应如何与目标目录中的对象匹配，应使用什么（如果有）作用域筛选器来决定是否设置对象，以及如何在将对象属性从源同步到目标目录时转换对象属性。

## <a name="methods"></a>Methods

| 方法                                                                                                | 返回类型                                                                                                 | 说明                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [获取架构](../api/synchronization-synchronizationschema-get.md)                                     | [synchronizationSchema](synchronization-synchronizationschema.md)                                           | 读取**synchronizationSchema**对象的属性和关系。                                                 |
| [更新架构](../api/synchronization-synchronizationschema-update.md)                               | 无                                                                                                        | 更新同步架构。                                                                                         |
| [删除架构](../api/synchronization-synchronizationschema-delete.md)                               | 无                                                                                                        | 删除自定义架构，将架构重置为默认配置。                                           |
| [列表筛选器运算符](../api/synchronization-synchronizationschema-filteroperators.md)              | [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合                      | 列出作用域筛选器支持的所有运算符。                                                                       |
| [列表属性映射函数](../api/synchronization-synchronizationschema-functions.md)         | [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合 | 列出属性映射表达式中支持的所有函数。                                                         |
| [分析属性映射表达式](../api/synchronization-synchronizationschema-parseexpression.md) | [parseExpressionResponse](synchronization-parseexpressionresponse.md)                                       | 将字符串表达式分析为[attributeMappingSource](../resources/synchronization-attributemappingsource.md)对象。 |


## <a name="properties"></a>属性

| 属性      | 类型      | Description    |
|:--------------|:----------|:---------------|
|目录名            |[directoryDefinition](synchronization-directorydefinition.md)集合   |描述作为[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)一部分的目录和对象。 |
|synchronizationRules   |[synchronizationRule](synchronization-synchronizationrule.md)集合   |为[synchronizationJob](synchronization-synchronizationjob.md)或[synchronizationTemplate](synchronization-synchronizationtemplate.md)配置的同步规则的集合。 |
|version                |String                             |架构的版本，随每个架构更改自动更新。|


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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
