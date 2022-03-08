---
title: accessReviewSet 资源类型
description: 公开访问评审 API 和功能的基本资源的容器。 当前仅公开 accessReviewScheduleDefinition 资源。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4964b26b1f6c415a0e822c6d47e67499876011b1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333216"
---
# <a name="accessreviewset-resource-type"></a>accessReviewSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开访问评审 API 和功能的基本资源的容器。 当前仅公开 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 关系。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|定义|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合| 表示访问评审的模板和日程安排。 |
|historyDefinitions|[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 集合| 表示访问评审历史记录数据和用于收集数据的范围的集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewSet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewSet"
}
```

