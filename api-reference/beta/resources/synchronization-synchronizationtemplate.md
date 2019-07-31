---
title: synchronizationTemplate 资源类型
description: " 任何人都可以检索模板以查看默认设置, 包括同步架构。"
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9176c092d62b4ee43d15d29884a3882fd3c627e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964597"
---
# <a name="synchronizationtemplate-resource-type"></a>synchronizationTemplate 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为特定应用程序提供预先配置的同步设置。 默认情况下, 将对基于该模板的任何[同步作业](synchronization-synchronizationjob.md)使用这些设置。 应用程序开发人员指定模板;任何人都可以检索模板以查看默认设置, 包括[同步架构](synchronization-synchronizationschema.md)。

您可以为应用程序提供多个模板, 并指定一个默认模板。 如果有多个模板可用于您感兴趣的应用程序, 请查找特定于应用程序的指南, 以确定哪一个模板最符合您的需求。

## <a name="methods"></a>方法

| 方法        | 返回类型               | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[synchronizationTemplate](synchronization-synchronizationtemplate.md)集合  |列出可用于应用程序实例或应用程序实例 (服务主体) 的模板。|
|[获取](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |读取**synchronizationTemplate**对象的属性和关系。|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>属性

| 属性      | 类型                      | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |字符串                     |唯一的模板标识符。|
|applicationId  |String                     |此模板所属应用程序的标识符。|
|设置        |Boolean                    |`true`如果建议将此模板作为应用程序的默认模板。|
|说明    |String                     |模板的说明。|
|被   |String                     |`true`如果此模板应显示在可用于应用程序实例 (服务主体) 的模板集合中。|
|factoryTag     |String                     |同步引擎支持的已知工厂标记之一。 **FactoryTag**告知同步引擎在处理基于此模板的作业时要使用的实现。|
|metadata       |metadataEntry 集合   |其他扩展属性。 除非明确提到, 否则不应更改元数据值。|

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
