---
title: requestSchedule 资源类型
description: 请求计划可以包含在访问包分配请求中，并且存在于访问包分配中。 在 PIM 中，使用此资源来定义主体何时具有合格或活动角色分配的计划。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1e8988f70ba9ee108248bbb7ce2322bb0136d00f
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899126"
---
# <a name="requestschedule-resource-type"></a>requestSchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-overview.md)中，访问包分配请求由想要获取访问包分配的用户创建。 此请求可以包含用户想要分配时间的计划。  来自此类请求的访问包分配也有计划。

在 PIM 中，使用此资源来定义主体何时具有合格或活动角色分配的计划。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|startDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 在 PIM 中，当符合条件或活动分配变得活动时。|
|到期|[expirationPattern](expirationpattern.md)|在权利管理中，访问应到期的时间。|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|对于定期访问，或符合条件或活动分配。 此属性目前在 PIM 和权利管理中都不受支持。|

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


