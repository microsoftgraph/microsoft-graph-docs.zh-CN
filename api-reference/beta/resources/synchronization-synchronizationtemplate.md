---
title: synchronizationTemplate 资源类型
description: " 任何人都可以检索要查看默认设置，包括同步架构的模板。"
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516551"
---
# <a name="synchronizationtemplate-resource-type"></a>synchronizationTemplate 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供了为特定应用程序预配置的同步设置。 将基于模板的任何[同步作业，](synchronization-synchronizationjob.md)默认情况下使用这些设置。 应用程序开发人员指定的模板;任何人都可以检索要查看默认设置，包括[同步架构](synchronization-synchronizationschema.md)的模板。

您可以提供多个模板的应用程序，并指定默认模板。 如果多个模板可供您感兴趣的应用程序，seek 特定于应用程序的指南，以确定哪一个最能满足您的需求。

## <a name="methods"></a>方法

| 方法        | 返回类型               | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[synchronizationTemplate](synchronization-synchronizationtemplate.md)集合  |列表的模板可供应用程序或应用程序实例 （服务主体）。|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |读取的属性和**synchronizationTemplate**对象的关系。|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>属性

| 属性      | 类型                      | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |String                     |唯一的模板标识符。|
|applicationId  |String                     |此模板所属的应用程序的标识符。|
|default        |Boolean                    |`true`如果此模板建议为默认的应用程序。|
|说明    |字符串                     |模板描述|
|可供搜索   |String                     |`true`如果此模板应出现在可用应用程序实例 （服务主体） 的模板的集合。|
|factoryTag     |String                     |同步引擎支持的已知工厂标记之一。 **FactoryTag**告知同步引擎处理在基于此模板的作业时使用的实现。|
|元数据       |metadataEntry 集合   |其他扩展属性。 除非明确提到，不应更改元数据值。|

## <a name="relationships"></a>关系
| 关系      | 类型      |说明|
|:------------------|:----------|:----------|
|架构             |[synchronizationSchema](synchronization-synchronizationschema.md)     |在基于此模板的作业的默认同步架构。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
