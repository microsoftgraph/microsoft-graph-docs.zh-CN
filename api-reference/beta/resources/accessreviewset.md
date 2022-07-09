---
title: accessReviewSet 资源类型
description: 公开访问评审 API 和功能的基础资源的容器。 当前仅公开 accessReviewScheduleDefinition 资源。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ca33119169ed61604b0c9deed18ecad33bd76069
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697839"
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
|决定|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合| 表示对审阅实例的 Azure AD 访问评审决策。|
|定义|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合| 表示访问评审的模板和计划。 |
|historyDefinitions|[accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) 集合| 表示访问评审历史记录数据的集合以及用于收集该数据的范围。|
|策略|[accessReviewPolicy](../resources/accessreviewpolicy.md)| 使管理员能够管理其租户中的目录级访问评审策略的资源。|

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

