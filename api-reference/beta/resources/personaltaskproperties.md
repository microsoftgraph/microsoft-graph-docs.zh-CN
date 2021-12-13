---
title: personalTaskProperties 资源类型
description: 包含任务的个人属性"
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 56007de468b5fd06998b94f5b5256cfb170ba127
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424878"
---
# <a name="personaltaskproperties-resource-type"></a>personalTaskProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含任务的个人 [属性](task.md)。 共享或分配任务 **时**，其他用户不会看到这些属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|reminderDatetime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要发生的提醒提醒提醒 **的** 日期和时间。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.personalTaskProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personalTaskProperties",
  "reminderDatetime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  }
}
```

