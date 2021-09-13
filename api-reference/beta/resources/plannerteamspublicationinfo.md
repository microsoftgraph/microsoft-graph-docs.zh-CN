---
title: plannerTeamsPublicationInfo 资源类型
description: 包含有关创建 plannerTask 的发布过程的详细信息。
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 77441184468a87e6d12d32adedc98a26c228db68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115042"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>plannerTeamsPublicationInfo 资源类型

命名空间：microsoft.graph

包含有关创建 [plannerTask](plannertask.md)的发布过程的详细信息。 发布过程基于模板创建任务副本。 这些任务在多个计划中创建，并且具有针对用户的受限权限;例如，无法删除这些字段，并且可能会阻止用户编辑某些字段。 发布用于在整个组织中分发任务并集中跟踪其进度。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|发布过程上次修改此任务的日期和时间。 只读。 |
|publicationId|String| 出版物的标识符。 只读。|
|publishedToPlanId|String|plannerPlan 此任务最初放置的标识符。 只读。 |
|publishingTeamId|String| 启动发布 [过程的](team.md) 团队的标识符。 只读。|
|publishingTeamName|String|启动显示名称过程的团队的组组。 此显示名称仅供参考，可能并不代表团队最新的名称。 只读。 |

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

