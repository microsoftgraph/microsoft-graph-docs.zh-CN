---
title: synchronizationJob 资源类型
description: 通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。 同步作业始终特定于租户中的应用程序的特定实例。 作为同步作业安装程序的一部分, 您需要授予在目标目录中读取和写入对象的权限, 并自定义作业的同步架构。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a311c8ae7618778c2dbd8cdbc9a5b30af254eae4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007793"
---
# <a name="synchronizationjob-resource-type"></a>synchronizationJob 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过定期在后台运行、轮询一个目录中的更改并将它们推送到另一个目录来执行同步。 同步作业始终特定于租户中的应用程序的特定实例。 作为同步作业安装程序的一部分, 您需要授予在目标目录中读取和写入对象的权限, 并自定义作业的同步架构。

## <a name="methods"></a>方法

| 方法        | 返回类型               | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[synchronizationJob](synchronization-synchronizationjob.md)集合  |列出给定应用程序实例 (服务主体) 的现有作业。|
|[获取 synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |读取 synchronizationJob 对象的属性和关系。|
|[创建](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |为给定应用程序创建新作业。|
|[Start](../api/synchronization-synchronizationjob-start.md)          |无   |启动同步。 如果作业处于暂停状态, 则它将从作业暂停的点继续。 如果作业处于隔离状态, 则隔离状态为 "已清除"。|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |无   |强制作业重新启动并重新处理目录中的所有对象。|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |无   |临时停止同步。 所有进度 (包括作业状态) 均保持不变, 作业将从[开始](../api/synchronization-synchronizationjob-start.md)调用时停止的位置继续。|
|[删除](../api/synchronization-synchronizationjob-delete.md)        |无   |停止同步, 并永久删除与作业关联的所有状态。|
|[获取 synchronizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |检索作业的有效同步架构。|
|[更新 synchronizationSchema](../api/synchronization-synchronizationschema-update.md)    |无   |更新作业的同步架构。 |
|[验证凭据](../api/synchronization-synchronizationjob-validatecredentials.md)|无|测试提供的针对目标目录的凭据。|

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|id             |String                     |唯一的同步作业标识符。 只读。|
|schedule       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|用于运行作业的计划。 只读。|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |作业的状态, 包括上次运行作业的时间、当前作业状态和错误。|
|templateId     |String    |此作业所基于的[同步模板](synchronization-synchronizationtemplate.md)的标识符。|

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
