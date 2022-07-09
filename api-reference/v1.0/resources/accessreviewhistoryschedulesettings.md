---
title: accessReviewHistoryScheduleSettings 资源类型
description: 在 Azure AD 访问评审中，accessReviewHistoryScheduleSettings 表示与访问评审历史记录定义系列关联的设置。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 70483c049a555bf2315a8f0cb49bd652893bef91
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696516"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>accessReviewHistoryScheduleSettings 资源类型

命名空间：microsoft.graph

定义 [accessReviewHistoryDefinition 对象的](accessreviewhistorydefinition.md) 设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | 使用标准 Outlook 定期对象的定期的详细设置。 <br/><br/>**注意：** 仅支持 **dayOfMonth**、 **interval** 和 **type** (`weekly`， `absoluteMonthly`) 属性。 在 **recurrenceRange** 上使用属性 **startDate** 来确定审阅开始的日期。 必填。 |
|reportRange|String|ISO 8601 持续时间格式的持续时间字符串，指定生成的审阅历史记录数据的回查周期。 例如，如果历史记录定义计划在每月 1 日运行，则 **reportRange** 为 `P1M`。 在这种情况下，在每个月的第一个时间，将仅收集包含上一个月审阅数据的访问评审历史记录数据。 <br/><br/>**注意：** 仅支持 **年**、 **月** 和 **天** ISO 8601 属性。 此为必需属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewHistoryScheduleSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryScheduleSettings",
  "reportRange": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```
