---
title: accessPackageAssignment 资源类型
description: 访问包分配是在一段时间内将访问包分配给特定主题。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7a4f603ee7f3f1553d97c4d04b0b695e3c0c2c0e
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698042"
---
# <a name="accesspackageassignment-resource-type"></a>accessPackageAssignment 资源类型

命名空间：microsoft.graph

在 [Azure AD 权利管理](entitlementmanagement-overview.md)中，访问包分配是在一段时间内分配给特定主题的访问包。  例如，访问包分配可以说明在 2019 年 1 月至 2019 年 7 月期间，用户 Alice 已通过访问包 Sales 分配访问权限。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackageAssignments](../api/entitlementmanagement-list-assignments.md)|[accessPackageAssignment](accesspackageassignment.md) 集合|检索 **accessPackageAssignment 对象的** 列表。 |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索已登录用户上筛选的 **accessPackageAssignment** 对象的列表。|
|[重新处理](../api/accesspackageassignment-reprocess.md) | 无 | 自动重新评估并强制执行特定访问包的用户分配。|

> [!NOTE]
> 若要为用户创建或删除访问包分配，请使用 [创建 accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) 方法。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|expiredDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|id|字符串|只读。|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|当访问分配到位时。 只读。|
|state|accessPackageAssignmentState|访问包分配的状态。 可能的值包括 `delivering`、`partiallyDelivered`、`delivered`、`expired`、`deliveryFailed`、`unknownFutureValue`。 只读。 支持 `$filter`（`eq`）。|
|status|String|有关分配生命周期的详细信息。  可能的值包括`Delivering`、`Delivered`或 `NearExpiry1DayNotificationTriggered``ExpiredNotificationTriggered`。  只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessPackage|[accessPackage](accesspackage.md)|只读。 可为 NULL。 支持 `$filter` 对 `eq` **id** 属性和 `$expand` 查询参数 () 。|
|target|[accessPackageSubject](accesspackagesubject.md)|访问包分配的主题。 只读。 可为 NULL。 支持 `$expand`。 支持 `$filter` **objectId** 上的 (`eq`) 。|
|assignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)|只读。 支持 `$filter` 对 `eq` **id** 属性和 `$expand` 查询参数 () 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "String (identifier)",
  "state": "String",
  "status": "String",
  "expiredDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


