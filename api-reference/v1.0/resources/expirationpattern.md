---
title: expirationPattern 资源类型
description: 请求计划中的过期模式可包含在访问包分配请求中，并且存在于访问包分配中。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 413fde6006f8a7fdf9aa5175adbb2d57c957c817
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242316"
---
# <a name="expirationpattern-resource-type"></a>expirationPattern 资源类型

命名空间：microsoft.graph

在[Azure AD中](entitlementmanagement-root.md)，访问包分配请求由想要获取访问包分配的用户创建。 此请求可包括用户希望何时进行工作分配的计划。  由此类请求导致的访问包分配也具有计划。  [entitlementManagementSchedule 的](entitlementmanagementschedule.md)过期字段指示访问包分配应过期的时间。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|duration|期限|请求者所需的访问持续时间以 ISO 8601 格式表示。 例如，PT3H 是指三个小时。  如果在请求中指定 **，endDateTime** 不应存在， **并且 type** 属性应设置为 `afterDuration` 。|
|endDateTime|DateTimeOffset|使用 ISO 8601 格式的日期和时间信息的时间戳，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|type|[expirationPatternType](#expirationpatterntype-values)|请求者所需的过期模式类型。 可能的值包括 `notSpecified`、`noExpiration`、`afterDateTime`、`afterDuration`。 |

### <a name="expirationpatterntype-values"></a>expirationPatternType 值

| 成员 | 说明 |
|:---------------|:--------|
|notSpecified|未指定过期计划。|
|noExpiration|请求者不希望访问过期。|
|afterDateTime|访问将在指定的日期和时间后过期。|
|afterDuration|访问将在相对于授予访问权限的指定持续时间后过期。 指定 **duration 属性** 时是必需的。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expirationPattern"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expirationPattern",
  "endDateTime": "String (timestamp)",
  "duration": "String (duration)",
  "type": "String"
}
```


