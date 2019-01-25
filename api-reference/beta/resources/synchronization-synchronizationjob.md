---
title: synchronizationJob 资源类型
description: 通过在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改执行同步。 同步作业始终是特定于您的租户中的应用程序的特定实例。 作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510566"
---
# <a name="synchronizationjob-resource-type"></a>synchronizationJob 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过在后台定期运行、 轮询一个目录，并将其推送到另一个目录中的更改执行同步。 同步作业始终是特定于您的租户中的应用程序的特定实例。 作为同步作业设置的一部分，您需要提供读取和写入您的目标目录中的对象的授权和自定义的作业同步架构。

## <a name="methods"></a>方法

| 方法        | 返回类型               | 说明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationjob-list.md)             |[synchronizationJob](synchronization-synchronizationjob.md)集合  |列出现有作业的给定应用程序实例 （服务主体）。|
|[获取 synchronizationJob](../api/synchronization-synchronizationjob-get.md) | [synchronizationJob](synchronization-synchronizationjob.md) |读取属性和 synchronizationJob 对象的关系。|
|[Create](../api/synchronization-synchronizationjob-post.md)         |[synchronizationJob](synchronization-synchronizationjob.md)   |创建新作业给定应用程序。|
|[Start](../api/synchronization-synchronizationjob-start.md)          |无   |启动同步。 如果该作业暂停状态，继续从该作业已暂停其中时间点。 如果该作业在隔离，清除隔离状态。|
|[Restart](../api/synchronization-synchronizationjob-restart.md)      |无   |强制该作业重新开始重新处理的目录中的所有对象。|
|[Pause](../api/synchronization-synchronizationjob-pause.md)          |无   |暂时停止同步。 所有的进度，包括作业状态保持不变，且该作业将继续从停止时[启动](../api/synchronization-synchronizationjob-start.md)调用的地方。|
|[删除](../api/synchronization-synchronizationjob-delete.md)        |无   |停止同步并永久删除所有与作业相关联的状态。|
|[获取 synchrnoizationSchema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |检索该作业的有效同步架构。|
|[更新 synchroizationSchema](../api/synchronization-synchronizationschema-update.md)    |无   |更新作业的同步架构。 |
|[验证凭据](../api/synchronization-synchronizationjob-validatecredentials.md)|无|测试针对目标目录提供的凭据。|

## <a name="properties"></a>属性

| 属性      | 类型      | 说明    |
|:--------------|:----------|:---------------|
|id             |String                     |唯一同步作业标识符。 只读。|
|Schedule       |[synchronizationSchedule](synchronization-synchronizationschedule.md)|用于运行作业的计划。 只读。|
|status         |[synchronizationStatus](synchronization-synchronizationstatus.md)     |作业，其中包括上次运行作业、 当前作业状态和错误的状态。|
|templateId     |字符串    |基于此作业[同步模板](synchronization-synchronizationtemplate.md)的标识符。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|架构|[synchronizationSchema](synchronization-synchronizationschema.md)| 配置作业同步架构。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
