---
title: plannerTeamsPublicationInfo 资源类型
description: 包含有关创建 plannerTask 的发布过程的详细信息。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9db73bb5a914a848f3e19e079321681b22510e8e
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883235"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>plannerTeamsPublicationInfo 资源类型

命名空间：microsoft.graph

包含有关创建 [plannerTask](plannertask.md)的发布过程的详细信息。 发布过程基于模板创建任务副本。 这些任务在多个计划中创建，并且用户具有受限权限;例如，无法删除它们，并且可能会阻止用户编辑某些字段。 出版物用于在整个组织中分发任务并集中跟踪任务的进度。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|上次由发布过程修改此任务的日期和时间。 只读。 |
|publicationId|String| 出版物的标识符。 只读。|
|publishedToPlanId|String|plannerPlan **此任务最初** 放置的标识符。 只读。 |
|publishingTeamId|String| 启动发布 [过程的](team.md) 团队的标识符。 只读。|
|publishingTeamName|String|启动显示名称流程的团队的订阅。 此显示名称仅供参考，可能不会表示团队的最新版本名称。 只读。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTeamsPublicationInfo",
  "publicationId": "String",
  "publishingTeamId": "String",
  "publishingTeamName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishedToPlanId": "String"
}
```

