---
title: entitlementManagementSchedule 资源类型
description: 权限管理计划可包含在访问包分配请求中，并且存在于访问包分配中。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18c814c0426deaa89709505816f21282c75b1757
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650900"
---
# <a name="entitlementmanagementschedule-complex-type"></a>entitlementManagementSchedule 复杂类型

命名空间：microsoft.graph

在[Azure AD中](entitlementmanagement-overview.md)，访问包分配请求由想要获取访问包分配的用户创建。 此请求可包括用户希望何时进行工作分配的计划。  由此类请求导致的访问包分配也具有计划。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|expiration|[expirationPattern](../resources/expirationpattern.md)|访问应过期的时间。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|对于定期访问。 目前未使用。|
|startDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.entitlementManagementSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagementSchedule",
  "startDateTime": "String (timestamp)",
  "expiration": {
    "@odata.type": "microsoft.graph.expirationPattern"
  },
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```


