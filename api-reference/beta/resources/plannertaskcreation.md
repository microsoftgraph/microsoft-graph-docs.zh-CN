---
title: plannerTaskCreation 资源类型
description: 包含有关 plannerTask 来源的信息。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e8a2a4bf3aae5f23a04c7ecb8ad043631f946b20
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883236"
---
# <a name="plannertaskcreation-resource-type"></a>plannerTaskCreation 资源类型

命名空间：microsoft.graph

包含有关 [plannerTask](plannerTask.md)的源的信息。 此资源将设置其所有属性，或者只有一个属性将具有一个值，该值指示任务由该属性描述的进程 `null` 创建。 所有 `null` 属性都表示该任务不是由任何专用进程创建的。 应用无需知道任务的来源，就可以处理它;但是，某些应用可以使用其他信息来提供有关这些任务的特定体验。 有关详细信息，请参阅特定资源的文档。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|teamsPublicationInfo|[plannerTeamsPublicationInfo](../resources/plannerteamspublicationinfo.md)|有关创建此任务的发布过程的信息。 `null` 值表示该任务不是由发布过程创建的。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTaskCreation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskCreation",
  "teamsPublicationInfo": {
    "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
  }
}
```

