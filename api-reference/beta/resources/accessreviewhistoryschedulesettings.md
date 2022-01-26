---
title: accessReviewHistoryScheduleSettings 资源类型
description: 在Azure AD评审中，accessReviewHistoryScheduleSettings 表示与访问评审历史记录定义系列关联的设置。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7f1e10372fbd2db23ae70ea413e007993c6f85a0
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226298"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>accessReviewHistoryScheduleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义 [accessReviewHistoryDefinition 对象的](accessreviewhistorydefinition.md) 设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | 使用标准定期对象定期Outlook设置。 <br/><br/>**注意：** 仅 **支持 dayOfMonth** **、interval** 和 **type** (`weekly` `absoluteMonthly` ，) 属性。 使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的哪一天。  必需。 |
|reportRange|String|ISO 8601 持续时间格式的持续时间字符串，用于指定生成的审阅历史记录数据的回发期。 例如，如果计划将历史记录定义在每月的 1 号运行， **则 reportRange** 为 `P1M` 。 在这种情况下，在每月的第一天，将收集仅包含上个月评价数据的访问评审历史记录数据。 <br/><br/>**注意：** 仅 **支持** **years、months** 和 **days** ISO 8601 属性。 此为必需属性。|

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
