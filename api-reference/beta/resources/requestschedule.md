---
title: requestSchedule 资源类型
description: 请求计划可包含在访问包分配请求中，并且存在于访问包分配中。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 33abd221d22d37cc58bcf3770b4e28fa78b77064
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718462"
---
# <a name="requestschedule-resource-type"></a>requestSchedule 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配请求由想要获取访问包分配的用户创建。 此请求可以包括用户希望何时进行工作分配的计划。  来自此类请求的访问包分配也具有计划。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|startDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|expiration|[expirationPattern](expirationpattern.md)|访问应过期的时间。|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|对于定期访问。 目前未使用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestSchedule"
}-->

```json
{
    "startDateTime": "2020-08-11T23:06:53.307Z",
    "expiration": {
        "endDateTime": "2020-09-10T23:06:53.307Z",
        "type": "afterDateTime"
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


