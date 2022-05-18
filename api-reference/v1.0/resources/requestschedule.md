---
title: requestSchedule 资源类型
description: 在 PIM 中，使用此资源定义主体何时具有合格或活动角色的计划。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 59adc6589ea351d565248797aeb9384b9ae3f890
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461441"
---
# <a name="requestschedule-resource-type"></a>requestSchedule 资源类型

命名空间：microsoft.graph

在 PIM 中，在创建或更新 [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) 或 [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) 对象时，使用此资源定义主体何时具有合格或活动角色分配的计划。 此对象允许的设置取决于 [Azure AD 角色的设置](../api/unifiedrolemanagementpolicy-list-rules.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|到期|[expirationPattern](../resources/expirationpattern.md)|当符合条件或活动分配过期时。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|符合条件或活动分配的频率。 此属性当前在 PIM 中不受支持。|
|startDateTime|DateTimeOffset|当符合条件或活动的分配变为活动时。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.requestSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.requestSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```

