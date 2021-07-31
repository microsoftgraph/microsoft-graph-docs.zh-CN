---
title: plannerPlanContainer 资源类型
description: 表示 plannerPlan 的容器。 容器是指定授权规则和计划的生命周期的资源。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ea0af35bf9f82928e9da3abc90670566f3cc0869
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665754"
---
# <a name="plannerplancontainer-resource-type"></a>plannerPlanContainer 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [plannerPlan 的容器](plannerPlan.md)。 容器是指定授权规则和计划的生命周期的资源。 这意味着只有有权使用包含计划的资源的人员才能使用计划及其中的任务。 删除包含的资源时，还将删除包含的计划。 **plannerPlanContainer** 的属性无法在计划创建后更改。

Planner 当前支持下表中列出的容器类型。 创建计划时，必须使用表中标识的资源的路径指定 **containerUrl** 属性。

|类型|说明|资源的路径|
|----|-----------|--------------------|
|group| 计划包含在组 [中](group.md)。| https://graph.microsoft.com/beta/groups/&lt;id&gt;|
|roster| 计划包含在 [plannerRoster 中](plannerroster.md) | https://graph.microsoft.com/beta/planner/rosters/&lt;id&gt;|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|containerId|String|包含计划的资源的标识符。|
|type|plannerContainerType| 包含计划的资源的类型。 有关支持的类型，请参阅上表。 可取值为：`group`、`unknownFutureValue`、`roster`。 请注意，您必须使用此可发展枚举中的请求标头获取以下 `Prefer: include-unknown-enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `roster` ：。|
|url|String|容器的完整规范 URL。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerPlanContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanContainer",
  "url": "String",
  "containerId": "String",
  "type": "String"
}
```

