---
title: accessReviewStageSettings 资源类型
description: 在Azure AD评审中，accessReviewStageSettings 表示与多阶段访问评审相关联的阶段的设置。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: daa7b139aa5a9321965bfe6391c92c16fbc52ffc
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816146"
---
# <a name="accessreviewstagesettings-resource-type"></a>accessReviewStageSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

代表与多阶段访问评审对象 [关联的阶段的](accessreviewscheduledefinition.md) 设置。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|decisionsWillMoveToNextStage|字符串集合|指示哪些决策将进入下一阶段。 可以是 、 、 `Approve`或 `Recommendation`的`Deny`子集`NotReviewed`。 如果未提供，所有决策将进入下一阶段。 可选。 |
|dependsOn|String 集合| 定义阶段的顺序或并行顺序，并取决于 **stageId**。 目前仅支持顺序阶段。 例如，如果 **stageId** 为 `2`， **则 dependsOn** 必须为 `1`。 如果 **stageId** 为 `1`，则不指定 **dependsOn**。 如果 **stageId** 不是 ，则是必需的 `1`。 |
|durationInDays|Int32|阶段的持续时间。 必需项。  <br/><br/>**注意：** 此属性在所有阶段中的累积值 <br/> 1。 将替代 [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) 对象上的 [instanceDurationInDays](accessReviewScheduleSettings.md) 设置。 <br/>2。不能超过一次重复发生的时间长度。 也就是说，如果审阅每周重复一次，则 **累积 durationInDays** 不能超过 7。 |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|如果提供，当主审阅者不存在时，会要求回退审阅者完成审阅。 例如，如果选择了经理作为审阅者，而审核中的主体没有经理Azure AD，则回退审阅者需要审阅该主体。 <br/><br/>**注意：** 此属性的值将替代 [accessReviewScheduleDefinition 对象上的相应](accessReviewScheduleDefinition.md) 设置。|
|recommendationsEnabled|Boolean|指示是否启用向审阅者显示建议。 必需项。 <br/><br/>**注意：** 此属性的值将替代 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象上的相应设置。[](accessReviewScheduleSettings.md)|
| recommendationInsightsSettings | [accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md) 集合 | 确定要向审阅者显示的建议。 <br/><br/>**注意：** 此属性的值将替代 [accessReviewScheduleDefinition 对象上的相应](accessreviewscheduledefinition.md)设置。[](accessReviewScheduleSettings.md)|
| recommendationLookBackDuration | 期限| 可选字段。 指示与将配置 (的审阅实例的开始日期) 不活动时间段。 如果用户在回看 `deny` 期间处于非活动状态，则建议为 。 对于组和角色Azure AD，接受任何持续时间。 对于应用程序审查，最长期限为 30 天。 如果未指定，持续时间为 30 天。 <br/><br/>**注意：** 此属性的值将替代 [accessReviewScheduleDefinition 对象上的相应](accessreviewscheduledefinition.md)设置。[](accessReviewScheduleSettings.md) |
|reviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|定义审阅者是谁。 如果未指定任何权限，则评论是自 (用户查看自己的访问权限) 。  有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者分配给你的访问[Graph定义](/graph/accessreviews-reviewers-concept)。 <br/><br/>**注意：** 此属性的值将替代 [accessReviewScheduleDefinition 上的相应设置](accessReviewScheduleDefinition.md)。 |
|stageId|字符串|**accessReviewStageSettings 的唯一标识符**。 **stageId** 将在 **dependsOn** 属性中用于指示阶段关系。 此为必需属性。 |

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

