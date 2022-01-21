---
title: userLastSignInRecommendationInsightSetting 资源类型
description: 在 Azure AD 访问评审中，userLastSignInRecommendationInsightSetting 表示与基于用户上次登录日期和时间的见解关联的设置，这些设置用于帮助审阅者做出决策。
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa1467ee59bbedd4765e2a64c22009e713a7e71a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137257"
---
# <a name="userlastsigninrecommendationinsightsetting-resource-type"></a>userlastsignInrecommendationinsightsetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**userLastSignInRecommendationInsightSetting** 允许你将用户的最后登录日期和时间配置为见解，帮助审阅者对 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)对象做出决策。

继承自 [accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md)。

## <a name="properties"></a>属性
| 属性    | 类型   | Description |
| :---------------| :---------- | :---------- |
| recommendationLookBackDuration | 期限 | 可选。 指示与将配置 (的审阅实例的开始日期) 不活动时间段。 如果用户在回看持续时间处于非活动状态， `deny` 则建议为 。 对于组和角色Azure AD，接受任何持续时间。 对于应用程序审查，最长期限为 30 天。 如果未指定，持续时间为 30 天。 |
| signInScope | userSignInRecommendationScope | 指示是否根据用户在租户或应用程序中的不活动状态计算不活动。 可能的值为 `tenant` `application` `unknownFutureValue` 、、。 `application` 仅在访问评审对应用程序的分配进行审阅时相关。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userLastSignInRecommendationInsightSetting",
  "baseType": "microsoft.graph.accessReviewRecommendationInsightSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userlastsignInrecommendationinsightsetting",
  "recommendationLookBackDuration": "Duration",
  "signInScope": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "userlastsignInrecommendationinsightsetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
