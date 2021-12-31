---
title: expirationPattern 资源类型
description: 请求计划中的过期模式可包含在访问包分配请求中，并且存在于访问包分配中。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 10be33677d61c5cfe00d64922845c7fa167fd9b7
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649764"
---
# <a name="expirationpattern-resource-type"></a>expirationPattern 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](entitlementmanagement-overview.md)，访问包分配请求由想要获取访问包分配的用户创建。 此请求可包括用户希望何时进行工作分配的计划。  由此类请求导致的访问包分配也具有计划。  [requestSchedule 的过期字段](requestschedule.md)指示访问包分配应过期的时间。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|endDateTime|DateTimeOffset|使用 ISO 8601 格式的日期和时间信息的时间戳，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|duration|期限|请求者所需的访问持续时间以 ISO 8601 格式表示。 例如，PT3H 是指三个小时。  如果在请求中指定 **，endDateTime** 不应存在， **并且 type** 属性应设置为 `afterDuration` 。|
|type|expirationPatternType|请求者所需的过期模式类型。|

### <a name="expirationpatterntype-values"></a>expirationPatternType 值

| 成员 | 值| 说明 |
|:---------------|:--------|:----------|
|notSpecified|0|未指定过期计划。|
|noExpiration|1|请求者不希望访问过期。|
|afterDateTime|2|访问将在指定的日期和时间后过期。|
|afterDuration|3|访问将在相对于授予访问权限的指定持续时间后过期。 指定 **duration 属性** 时是必需的。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern"
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


