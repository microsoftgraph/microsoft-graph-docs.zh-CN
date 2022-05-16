---
title: plannerPlanContainer 资源类型
description: 表示 plannerPlan 的容器。 容器是一个资源，用于指定授权规则和计划的生存期。
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: dbb95f1124461e12b36d6c4f69dac193aa349b15
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420782"
---
# <a name="plannerplancontainer-resource-type"></a>plannerPlanContainer 资源类型

命名空间：microsoft.graph

表示 [plannerPlan](plannerplan.md) 的容器。 容器是一个资源，用于指定授权规则和计划的生存期。 这意味着只有有权使用包含该计划的资源的人员才能处理计划及其中的任务。 删除包含该计划的资源时，也会删除所包含的计划。 创建计划后，无法更改 **plannerPlanContainer** 的属性。

Microsoft Planner 当前支持下表中列出的容器类型。 创建计划时，必须使用下表中标识的资源的路径指定 **containerUrl** 属性。

|类型|说明|获取资源的路径|
|----|-----------|--------------------|
|组| 计划包含在[组](group.md)中。| https://graph.microsoft.com/v1.0/groups/{id}|
|名单| 计划包含在 **plannerRoster** 中 | https://graph.microsoft.com/beta/planner/rosters/{id}. 目前只能使用 beta 版本访问 **plannerRosters**。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|containerId|String|包含计划的资源的标识符。|
|type|plannerContainerType| 包含计划的资源的类型。 有关支持的类型，请参阅上表。 可取值为：`group`、`unknownFutureValue`、`roster`。 请注意，必须使用 `Prefer: include-unknown-enum-members` 请求标头获取此 [可进化枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) 中的以下值: `roster`。|
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
  "containerId": "String",
  "type": "String",
  "url": "String"
}
```

