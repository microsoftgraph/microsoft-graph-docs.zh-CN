---
title: accessReviewSet 资源类型
description: 公开访问评审 API 和功能的基础资源的容器。 当前仅公开 accessReviewScheduleDefinition 资源。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a4310978c8c3578604523f9fa299581f5b24039a
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697972"
---
# <a name="accessreviewset-resource-type"></a>accessReviewSet 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开访问评审 API 和功能的基础资源的容器。 当前仅公开 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 关系。

继承自 [entity](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|定义|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合| 表示访问评审的模板和计划。 |
|historyDefinitions|[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 集合| 表示访问评审历史记录数据的集合以及用于收集该数据的范围。|

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

