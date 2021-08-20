---
title: plannerTaskCreation 资源类型
description: 包含有关 plannerTask 来源的信息。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 738067895a60b79684ef3f0356f59e777363d8140bc2734d2b38bf036c0feb84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226117"
---
# <a name="plannertaskcreation-resource-type"></a>plannerTaskCreation 资源类型

命名空间：microsoft.graph

包含有关 [plannerTask 的来源的信息](plannerTask.md)。 此资源的所有属性都设置为 ，或者只有一个属性将具有一个值，该值指示任务是由该属性描述 `null` 的进程创建的。 所有 `null` 属性都表示该任务不是由任何专用进程创建的。 应用无需知道任务的来源，就可以使用任务;但是，某些应用可以使用其他信息来提供有关这些任务的特定体验。 有关详细信息，请参阅特定资源的文档。

## <a name="properties"></a>属性
|属性|类型|说明|
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

