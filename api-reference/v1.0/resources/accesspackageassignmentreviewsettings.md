---
title: accessPackageAssignmentReviewSettings 复杂类型
description: 用于访问包分配的访问评审。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8deb20e147d9572911bc94aaec83750e8972592e
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608297"
---
# <a name="accesspackageassignmentreviewsettings-complex-type"></a>accessPackageAssignmentReviewSettings 复杂类型

命名空间：microsoft.graph

设置在访问包[分配](accesspackageassignmentpolicy.md)策略中配置，用于通过该策略对访问包分配的访问评审。 提供用于选择这些工作分配的审阅者的设置，以及必须审阅这些工作分配的频繁时间。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|expirationBehavior|accessReviewExpirationBehavior|在未审查访问权限时要应用的默认决定。 可能的值包括 `keepAccess`、`removeAccess`、`acceptAccessRecommendation`、`unknownFutureValue`。|
|fallbackReviewers|[subjectSet](../resources/subjectset.md) 集合|此集合指定在主要审阅者未回复时将成为回退审阅者的用户。|
|isEnabled|Boolean|如果 `true`为 ，则通过此策略分配需要访问评审。|
|isRecommendationEnabled|布尔|指定是否向审阅者显示建议。 默认值为 `true`。|
|isReviewerJustificationRequired|布尔|指定审阅者是否必须提供审批理由。 默认值为 `true`。|
|isSelfReview|布尔|指定主体是否可以审阅其自己的工作分配。|
|primaryReviewers|[subjectSet](../resources/subjectset.md) 集合|此集合指定将审阅访问包分配的用户或用户组。|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|第一次审阅应何时开始以及应重复出现多久。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentReviewSettings",
  "isEnabled": "Boolean",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  },
  "isSelfReview": "Boolean",
  "primaryReviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "expirationBehavior": "String",
  "isRecommendationEnabled": "Boolean",
  "isReviewerJustificationRequired": "Boolean"
}
```


