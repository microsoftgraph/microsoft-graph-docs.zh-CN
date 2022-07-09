---
title: accessReviewStageSettings 资源类型
description: 在 Azure AD 访问评审中，accessReviewStageSettings 表示与多阶段访问评审关联的阶段的设置。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8a7e0142f7f97f608544bc4ca4fc56ab4d3f11dd
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697832"
---
# <a name="accessreviewstagesettings-resource-type"></a>accessReviewStageSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示与 [多阶段访问评审对象关联的阶段](accessreviewscheduledefinition.md) 的设置。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|decisionsThatWillMoveToNextStage|String 集合|指示下一阶段将要做出哪些决定。 可以是一个子集，`Approve`或 `Deny``Recommendation``NotReviewed`。 如果未提供，所有决策都将进入下一阶段。 可选。 |
|dependsOn|字符串集合| 定义阶段的顺序或并行顺序，并取决于 **stageId**。 目前仅支持顺序阶段。 例如，如果 **stageId** 为 `2`stageId，则 **dependsOn** 必须为 `1`。 如果 **stageId** 为 `1`stageId，请勿指定 **dependsOn**。 如果 **stageId** 不是 `1`，则为必需。 |
|durationInDays|Int32|阶段的持续时间。 必填。  <br/><br/>**注意：** 此属性在所有阶段的累积值 <br/> 1. 将覆盖 [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) 对象上的 [instanceDurationInDays 设置](accessReviewScheduleSettings.md)。 <br/>2. 不能超过一次重复周期的长度。 也就是说，如果每周重复一次评审， **则累积持续时间不能** 超过 7。 |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|如果提供，如果主要审阅者不存在，则要求回退审阅者完成审阅。 例如，如果经理被选为 **审阅者** ，并且正在审查的主体在 Azure AD 中没有经理，则要求回退审阅者评审该主体。 <br/><br/>**注意：** 此属性的值将覆盖 [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) 对象上的相应设置。|
|recommendationsEnabled|Boolean|指示是否已启用向审阅者显示建议。 必填。 <br/><br/>**注意：** 此属性的值将替代 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象上的相应 [设置](accessReviewScheduleSettings.md)。|
| recommendationInsightsSettings | [accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md) 集合 | 确定要向审阅者显示的建议。 <br/><br/>**注意：** 此属性的值将覆盖 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象上的相应 [设置](accessReviewScheduleSettings.md)。|
| recommendationLookBackDuration | 持续时间| 可选字段。 指示将从中配置建议) 评审实例的开始日期 (非活动时间段。 建议 `deny` 在回首持续时间内用户是否处于非活动状态。 对于组和 Azure AD 角色的评审，将接受任何持续时间。 对于应用程序评审，30 天是最长持续时间。 如果未指定，则持续时间为 30 天。 <br/><br/>**注意：** 此属性的值将覆盖 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象上的相应 [设置](accessReviewScheduleSettings.md)。 |
|评论家|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|定义审阅者是谁。 如果未指定任何内容，则评审是自审 (用户审阅自己的访问权限) 。  有关分配审阅者的选项示例，请参阅[使用 Microsoft 图形 API 将审阅者分配到访问评审定义](/graph/accessreviews-reviewers-concept)。 <br/><br/>**注意：** 此属性的值将覆盖 [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) 上的相应设置。 |
|stageId|String|**accessReviewStageSettings** 的唯一标识符。 **stageId** 将用于 **dependsOn** 属性以指示阶段关系。 此为必需属性。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewStageSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewStageSettings",
  "stageId": "String",
  "dependsOn": [
    "String"
  ],
  "durationInDays": "Integer",
  "recommendationsEnabled": "Boolean",
  "recommendationLookBackDuration": "String (duration)",
  "decisionsThatWillMoveToNextStage": [
    "String"
  ],
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```

