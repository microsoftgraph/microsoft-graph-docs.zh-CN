---
title: expirationPattern 资源类型
description: 过期模式定义请求或分配何时过期。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a42454acfb8c6dc50077fdd85fc7fcf9fa8086e5
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461329"
---
# <a name="expirationpattern-resource-type"></a>expirationPattern 资源类型

命名空间：microsoft.graph

在 [Azure AD 权利管理](entitlementmanagement-overview.md)中，访问包分配请求由想要获取访问包分配的用户创建。 此请求可以包含用户想要分配时间的计划。 来自此类请求的访问包分配也有计划。 [entitlementManagementSchedule](entitlementmanagementschedule.md) 的过期字段指示访问包分配何时到期。

在 PIM 中，使用此资源定义 [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) 或 [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) 对象何时过期。 此对象允许的设置取决于 [Azure AD 角色的设置](../api/unifiedrolemanagementpolicy-list-rules.md)。 例如，如果 Azure AD 角色的设置指定不允许永久符合条件的分配，则为 **type** 属性指定`noExpiration`将返回错误。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|duration|期限|请求者所需的访问持续时间（以 ISO 8601 格式表示）持续时间。 例如，PT3H 是指 3 小时。  如果在请求中指定， **则不应存在 endDateTime** ，并且应将 **type** 属性设置为 `afterDuration`。|
|endDateTime|DateTimeOffset|使用 ISO 8601 格式的时间戳日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|type|[expirationPatternType](#expirationpatterntype-values)|请求者的所需过期模式类型。 可能的值包括 `notSpecified`、`noExpiration`、`afterDateTime`、`afterDuration`。 |

### <a name="expirationpatterntype-values"></a>expirationPatternType 值

| 成员 | 说明 |
|:---------------|:--------|
|notSpecified|未指定过期计划。|
|noExpiration|请求者不希望访问过期。|
|afterDateTime|访问将在指定的日期和时间后过期。|
|afterDuration|相对于授予访问权限的指定持续时间后，访问权限将过期。 指定 **duration** 属性时是必需的。|

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


