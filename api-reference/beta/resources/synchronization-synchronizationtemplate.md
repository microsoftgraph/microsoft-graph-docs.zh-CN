---
title: synchronizationTemplate 资源类型
description: 为特定应用程序提供预配置的同步设置。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c08f5c3eee6225a1149ff993415f83b2e5916583
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132298"
---
# <a name="synchronizationtemplate-resource-type"></a>synchronizationTemplate 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为特定应用程序提供预配置的同步设置。 默认情况下，这些设置将用于基于模板的任何同步作业[](synchronization-synchronizationjob.md)。 应用程序开发人员指定模板;任何人都可以检索模板以查看默认设置，包括 [同步架构](synchronization-synchronizationschema.md)。

可以为应用程序提供多个模板，并指定默认模板。 如果对感兴趣的应用程序提供了多个模板，请寻找特定于应用程序的指南，以确定哪个模板最能满足你的需求。

## <a name="methods"></a>方法

| 方法        | 返回类型               | Description                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[synchronizationTemplate](synchronization-synchronizationtemplate.md) 集合  |列出可用于应用程序或应用程序实例的模板 (服务主体) 。|
|[获取](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |读取 **synchronizationTemplate** 对象的属性和关系。|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>属性

| 属性      | 类型                      | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |字符串                     |唯一模板标识符。|
|applicationId  |String                     |此模板所属的应用程序的标识符。|
| 默认值        |Boolean                    |`true` 如果建议此模板为应用程序的默认值。|
|说明    |字符串                     |模板的说明。|
|可发现   |字符串                     |`true` 如果此模板应显示在可用于应用程序实例的模板集合中， (服务主体) 。|
|factoryTag     |字符串                     |同步引擎支持的已知工厂标记之一。 **factoryTag** 告知同步引擎在基于此模板处理作业时要使用哪种实现。|
|metadata       |metadataEntry 集合   |其他扩展属性。 除非明确提到，否则不应更改元数据值。|

## <a name="relationships"></a>关系
| 关系      | 类型      |说明|
|:------------------|:----------|:----------|
|架构             |[synchronizationSchema](synchronization-synchronizationschema.md)     |基于此模板的作业的默认同步架构。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


