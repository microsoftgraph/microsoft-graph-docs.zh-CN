---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由想要获取访问包分配的用户创建。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cdf2e4111daeea48babd57aac912006bd2418187
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698357"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>accessPackageAssignmentRequest 资源类型

命名空间：microsoft.graph


在 [Azure AD 权利管理](entitlementmanagement-overview.md)中，访问包分配请求是由想要获取访问包分配的用户或代表用户创建的。 如果请求成功，并且需要任何必要的批准，则用户将收到访问包分配，并且是生成的访问包分配的主题。  Azure AD 还会自动创建用于跟踪访问删除的访问包分配请求。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合|检索 **accesspackageassignmentrequest 对象的** 列表。 |
| [创建 accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 **accessPackageAssignmentRequest** 对象。 |
|[获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|读取 **accessPackageAssignmentRequest** 对象的属性和关系。 |
|[删除 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|无|删除 **accessPackageAssignmentRequest**。 |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|检索已登录用户上筛选的 **accessPackageAssignmentRequest** 对象的列表。|
|[取消](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|取消处于可取消状态 **的 accessPackageAssignmentRequest** 对象。|
|[重新处理](../api/accesspackageassignmentrequest-reprocess.md) | 无 | 自动重试用户对访问包的访问请求。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|请求的处理结束日期（成功或失败）。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|id|String|只读。|
|requestType|accessPackageRequestType|请求的类型。 可能的值为：`notSpecified`、、`userAdd`、`userUpdate`、`userRemove`、`adminUpdate``adminAdd`、`adminRemove`、`systemAdd``systemUpdate`、`systemRemove`、`onBehalfAdd`。 `unknownFutureValue` 来自用户本身的请求的 requestType 为 `UserAdd` 或 `UserRemove`. 设置后，无法更改此属性。|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|要将访问权限分配给请求方的日期范围。 设置后，无法更改此属性。|
|state|accessPackageRequestState|请求的状态。 可取值包括：`submitted`、`pendingApproval`、`delivering`、`delivered`、`deliveryFailed`、`denied`、`scheduled`、`canceled`、`partiallyDelivered`、`unknownFutureValue`。 只读。|
|status|String|有关请求处理状态的详细信息。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|与 accessPackageAssignmentRequest 关联的访问包。 访问包定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。 只读。 可为 NULL。 <br/><br/> 支持 `$expand`。|
|分配|[accessPackageAssignment](../resources/accesspackageassignment.md)|对于 **requestType** 或`UserAdd``AdminAdd`，这是请求创建的访问包分配。  对于 **requestType**，`UserRemove``AdminRemove`或者`SystemRemove`，这具有`id`要删除的现有分配的属性。  <br/><br/> 支持 `$expand`。|
|请求|[accessPackageSubject](../resources/accesspackagesubject.md)|请求的主题，或者分配了直接分配。 只读。 可为 NULL。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "state": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


