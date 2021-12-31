---
title: accessReviewSet 资源类型
description: 公开访问评审 API 和功能的基本资源的容器。 当前仅公开 accessReviewScheduleDefinition 资源。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f1d3b28da541a365d1507cefce8d18adbc407dae
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650790"
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

