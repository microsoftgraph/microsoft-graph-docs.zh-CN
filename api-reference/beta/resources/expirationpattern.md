---
title: expirationPattern 资源类型
description: 请求计划中的过期模式可包含在访问包分配请求中，并存在于访问包分配中。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f9200d336ae69ae02c45ab1d6fc3d9df86691ebc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026971"
---
# <a name="expirationpattern-resource-type"></a>expirationPattern 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求由要获取访问包分配的用户创建。 此请求可以包括用户想要进行分配的日程安排。  通过此类请求生成的访问包分配也有计划。  [RequestSchedule](requestschedule.md)的 "过期" 字段指示访问包分配应何时过期。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|duration|持续时间|请求者所需的 access 持续时间。 如果在请求中指定，则 endDateTime 不应存在。|
|type|expirationPatternType|请求者所需的过期模式类型。|

### <a name="expirationpatterntype-values"></a>expirationPatternType 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|notSpecified|0|未指定任何过期计划。|
|noExpiration|1 |请求者不希望访问过期。|
|afterDateTime|2 |访问将在指定的日期和时间后过期。|
|afterDuration|第三章|访问将在相对于要授予访问权限的指定持续时间之后过期。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern",
  "baseType": ""
}-->

```json
{
    "endDateTime": "2020-09-10T23:06:53.307Z",
    "type": "afterDateTime"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expirationPattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


