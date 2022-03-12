---
title: taskViewpoint 资源类型
description: 包含任务的个人属性"
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 36590611168f34335795f6200bfe06e09436c1c0
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451525"
---
# <a name="taskviewpoint-resource-type"></a>taskViewpoint 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含任务的个人 [属性](task.md)。 共享或分配任务 **时**，其他用户不会看到这些属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要发生的提醒提醒提醒 **的** 日期和时间。|
|categories|String 集合|与任务关联的类别。 每个类别对应于用户定义的 [outlookCategory](../resources/outlookcategory.md) 的 **displayName** 属性。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.taskViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskViewpoint",
  "reminderDatetime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "categories": ["string"]
}
```

