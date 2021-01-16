---
title: plannerPlanContainer 资源类型
description: 表示 plannerPlan 的容器。 容器是指定授权规则和计划的生存期的资源。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8b3abb10892077159e6f02c33a31d501a75dba2a
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883231"
---
# <a name="plannerplancontainer-resource-type"></a>plannerPlanContainer 资源类型

命名空间：microsoft.graph

表示 [plannerPlan 的容器](plannerPlan.md)。 容器是指定授权规则和计划的生存期的资源。 这意味着只有有权使用包含计划的资源的人员才能使用计划及其中的任务。 删除包含的资源时，也会删除包含的计划。 **plannerPlanContainer** 的属性在计划创建后无法更改。

Planner 当前支持下表中列出的容器类型。 创建计划时，必须使用表中标识的资源的路径指定 **containerUrl** 属性。

|类型|Description|资源的路径|
|----|-----------|--------------------|
|group| 计划包含在组内。| https://graph.microsoft.com/v1.0/groups/&lt;id&gt;|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|containerId|String|包含计划的资源的标识符。|
|type|plannerContainerType| 包含计划的资源的类型。 有关支持的类型，请参阅上表。 可取值为：`group`、`unknownFutureValue`。|
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

