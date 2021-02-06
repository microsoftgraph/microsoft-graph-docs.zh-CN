---
title: synchronizationJob 资源类型
description: 通过定期在后台运行、轮询一个目录中的更改，以及将它们推送到另一个目录执行同步。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f0036cd26a72effba41085d9a4638647fd4060e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132039"
---
# <a name="synchronizationjob-resource-type"></a>synchronizationJob 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过定期在后台运行、轮询一个目录中的更改，以及将它们推送到另一个目录执行同步。 同步作业始终特定于租户中应用程序的特定实例。 作为同步作业设置的一部分，您需要授权读取和写入目标目录中的对象，并自定义作业的同步架构。

## <a name="methods"></a>方法

| 方法        | 返回类型               | Description                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[synchronizationJob](synchronization-synchronizationjob.md) 集合  |列出给定应用程序实例的现有作业 (服务主体) 。|
|[获取 synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |读取 synchronizationJob 对象的属性和关系。|
|[创建](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |为给定应用程序创建新作业。|
|[开始](../api/synchronization-synchronizationjob-start.md)          |无   |启动同步。 如果作业已暂停，则从作业暂停时开始继续。 如果作业被隔离，则清除隔离状态。|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |无   |强制作业重新开始并重新处理目录中的所有对象。|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |无   |暂时停止同步。 所有进度（包括作业状态）都将保持，并且作业将在启动调用时从它离开的地方继续。 [](../api/synchronization-synchronizationjob-start.md)|
|[删除](../api/synchronization-synchronizationjob-delete.md)        |无   |停止同步，并永久删除与作业关联的所有状态。|
|[获取 synchronizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |检索作业的有效同步架构。|
|[更新 synchronizationSchema](../api/synchronization-synchronizationschema-update.md)    |无   |更新作业的同步架构。 |
|[验证凭据](../api/synchronization-synchronizationjob-validatecredentials.md)|无|针对目标目录测试提供的凭据。|
|[provisionOnDemand](../api/synchronization-synchronizationjob-provision-on-demand.md)|[synchronizationJobApplicationParameters](../resources/synchronization-synchronizationjobapplicationparameters.md) 集合|表示将设置的对象和执行同步规则。 资源主要用于按需预配。 |
## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|id             |字符串                     |唯一同步作业标识符。 只读。|
|schedule       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|用于运行作业的计划。 只读。|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |作业的状态，包括上次运行作业时、当前作业状态和错误。|
|synchronizationJobSettings   |[keyValuePair](keyvaluepair.md)    |与作业关联的设置。 某些设置是从模板继承的。|
|templateId     |字符串    |此作业 [所基于的](synchronization-synchronizationtemplate.md) 同步模板的标识符。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|架构|[synchronizationSchema](synchronization-synchronizationschema.md)| 为作业配置的同步架构。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "synchronizationJobSettings": {"@odata.type": "microsoft.graph.keyValuePair"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


