---
title: accessReviewHistoryScheduleSettings 资源类型
description: 在Azure AD评审中，accessReviewHistoryScheduleSettings 表示与访问评审历史记录定义系列关联的设置。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 32c8eff3229b0597a5dc05cfeffa66fe8ed2d851
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337672"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>accessReviewHistoryScheduleSettings 资源类型

命名空间：microsoft.graph

定义 [accessReviewHistoryDefinition 对象的](accessreviewhistorydefinition.md) 设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | 使用标准定期对象定期Outlook设置。 <br/><br/>**注意：** 仅 **支持 dayOfMonth****、interval** 和 **type** (`weekly`， `absoluteMonthly`) 属性。 使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的哪一天。 必需项。 |
|reportRange|String|ISO 8601 持续时间格式的持续时间字符串，用于指定生成的审阅历史记录数据的回发期。 例如，如果计划将历史记录定义在每月的 1 号运行， **则 reportRange** 为 `P1M`。 在这种情况下，在每月的第一天，将收集仅包含上个月评价数据的访问评审历史记录数据。 <br/><br/>**注意：** 仅 **支持年****、月、****日 ISO** 8601 属性。 此为必需属性。|

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
