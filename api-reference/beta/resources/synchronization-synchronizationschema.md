---
title: synchronizationSchema 资源类型
description: 定义要同步的对象及其同步的方式。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b16e892c44cb69fb5039418a4a246e8b6f32ae9f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131591"
---
# <a name="synchronizationschema-resource-type"></a>synchronizationSchema 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义要同步的对象及其同步的方式。 同步架构包含特定同步作业的多数设置信息。 通常，您将自定义某些[属性](synchronization-attributemapping.md)映射，或添加范围筛选器以仅同步满足[](synchronization-filter.md)特定条件的对象。

以下各节介绍同步架构的高级别组件。

## <a name="directory-definitions"></a>目录定义

[目录定义](synchronization-directorydefinition.md) 提供有关目录及其对象的同步引擎信息。 例如，目录定义告知同步引擎，Azure AD 目录具有名为 user 和 **group** 的对象、这些对象支持哪些属性以及这些属性的类型。 为了使特定对象和属性用于同步规则/对象映射，它们必须定义为目录定义的一部分。

## <a name="synchronization-rules"></a>同步规则

[同步](synchronization-synchronizationrule.md) 规则是同步设置的核心。 它们为同步引擎定义如何执行同步，包括应同步哪些对象、源目录中的对象应该如何与目标目录中的对象匹配，以及属性在从源目录同步到目标目录时如何转换。

## <a name="object-mappings"></a>对象映射

[对象映射](synchronization-objectmapping.md) 是同步规则的主要部分。 每个对象映射都定义给定对象如何从源目录同步到目标目录。 具体而言，该映射定义源目录中的对象如何与目标目录中的对象匹配，使用什么 (（如果有) 范围筛选器）决定是否设置对象，以及当对象属性从源目录同步到目标目录时，如何转换它们。

## <a name="methods"></a>方法

| 方法                                                                                                | 返回类型                                                                                                 | 说明                                                                                                                |
|:------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------|
| [获取架构](../api/synchronization-synchronizationschema-get.md)                                     | [synchronizationSchema](synchronization-synchronizationschema.md)                                           | 读取 **synchronizationSchema** 对象的属性和关系。                                                 |
| [更新架构](../api/synchronization-synchronizationschema-update.md)                               | 无                                                                                                        | 更新同步架构。                                                                                         |
| [删除架构](../api/synchronization-synchronizationschema-delete.md)                               | 无                                                                                                        | 删除自定义架构，将架构重置为默认配置。                                           |
| [列出筛选器运算符](../api/synchronization-synchronizationschema-filteroperators.md)              | [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) 集合                      | 列出范围筛选器中支持的所有运算符。                                                                       |
| [列表属性映射函数](../api/synchronization-synchronizationschema-functions.md)         | [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) 集合 | 列出属性映射表达式中支持的所有函数。                                                         |
| [分析属性映射表达式](../api/synchronization-synchronizationschema-parseexpression.md) | [parseExpressionResponse](synchronization-parseexpressionresponse.md)                                       | 将字符串表达式解析为 [attributeMappingSource](../resources/synchronization-attributemappingsource.md) 对象。 |


## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|id|字符串|架构的唯一标识符。|
|synchronizationRules   |[synchronizationRule](synchronization-synchronizationrule.md) 集合   |为 [synchronizationJob](synchronization-synchronizationjob.md) 或 [synchronizationTemplate](synchronization-synchronizationtemplate.md)配置的同步规则的集合。 |
|version                |String                             |架构版本，随每个架构更改自动更新。|


## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|目录|[directoryDefinition](../resources/synchronization-directorydefinition.md) 集合|包含目录及其所有对象的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchema",
  "id": "String (identifier)",
  "synchronizationRules": [
    {
      "@odata.type": "microsoft.graph.synchronizationRule"
    }
  ],
  "version": "String"
}
```


