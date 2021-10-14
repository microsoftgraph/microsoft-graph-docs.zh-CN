---
title: assignmentReviewSettings 资源类型
description: assignmentReviewSettings 类型（用于访问包分配策略的 accessReviewSettings 属性）提供其他设置，以选择必须从此策略查看访问包分配以及必须查看它们多久查看一次。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7bb8afe847a9ceca9f11a54cc7f9c69a44ac0cde
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2021
ms.locfileid: "60290265"
---
# <a name="assignmentreviewsettings-resource-type"></a>assignmentReviewSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于访问 **包分配策略 的 accessReviewSettings** [属性](accesspackageassignmentpolicy.md)。 提供其他设置，以选择必须从此策略查看访问包分配以及必须查看它们多久查看一次。  

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| accessReviewTimeoutBehavior | [accessReviewTimeoutBehavior](#accessreviewtimeoutbehavior-values) | 如果未在 **durationInDays** 中指定的时段内审阅请求，则应用的默认决定。 可能的值是 `acceptAccessRecommendation` `keepAccess` ：、、 `removeAccess` 和 `unknownFutureValue` 。 |
| durationInDays | Int32 | 审阅者应提供输入的天数。|
| isAccessRecommendationEnabled | Boolean | 指定是否向审阅者显示建议。 默认值为 `true` |
| isApprovalJustificationRequired | Boolean | 指定审阅者是否必须提供审批理由。 默认值为 `true`。 |
| isEnabled| Boolean | 如果为 true，则此策略中的分配需要访问评审。 |
| recurrenceType | 字符串 | 重复周期的间隔，例如 `monthly` 或 `quarterly` 。 |
| reviewerType | String | Who或 请求用户 `Self` 执行审阅 `Reviewers` 。 |
| reviewers | [userSet](userset.md) 集合 | 如果 reviewerType 为 ，则此集合使用 `Reviewers` [singleUser](singleuser.md) 和 [groupMembers](groupmembers.md)的集合指定将按 ID 或作为组的成员作为审阅者的用户。 |
| startDateTime | DateTimeOffset | 第一次审阅应何时开始。 |

### <a name="accessreviewtimeoutbehavior-values"></a>accessReviewTimeoutBehavior 值

| 成员 | 说明 |
|:---------------|:--------|:----------|
| acceptAccessRecommendation | 从访问评审中接受建议以接受/删除对访问包的访问的审阅决定。 AR 建议的一般规则是，如果上次用户登录时间超过 30 天，建议删除对该用户的访问权限。 |
| keepAccess | 审查决定是保留当前访问权限。 |
| removeAccess | 审查决定是删除对访问包的访问权限。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentReviewSettings",
  "isEnabled": "Boolean",
  "recurrenceType": "String",
  "reviewerType": "String",
  "startDateTime": "String (timestamp)",
  "durationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "isAccessRecommendationEnabled": "Boolean",
  "isApprovalJustificationRequired": "Boolean",
  "accessReviewTimeoutBehavior": "String"
}
```


