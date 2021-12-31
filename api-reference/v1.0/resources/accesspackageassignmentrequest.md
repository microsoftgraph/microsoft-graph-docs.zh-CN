---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由想要获取访问包分配的用户创建。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ca963bd2a538cad8efe8692e82c6e1da678c0a21
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651447"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>accessPackageAssignmentRequest 资源类型

命名空间：microsoft.graph


在[Azure AD中](entitlementmanagement-overview.md)，访问包分配请求由希望获取访问包分配的用户或代表该用户创建。 如果请求成功，并且经过任何必要的审批，用户将收到访问包分配，并且是生成的访问包分配的主题。  Azure AD还自动创建访问包分配请求，以跟踪访问删除。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合|检索 **accesspackageassignmentrequest 对象** 的列表。 |
| [创建 accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 **accessPackageAssignmentRequest** 对象。 |
|[获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md)|[accessPackageAssignmentRequest](accesspackageassignmentrequest.md)|读取 **accessPackageAssignmentRequest** 对象的属性和关系。 |
|[删除 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md)|无|删除 **accessPackageAssignmentRequest**。 |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|检索已登录 **用户筛选的 accessPackageAssignmentRequest** 对象列表。|
|[取消](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|取消 **处于可取消状态中的 accessPackageAssignmentRequest** 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|completedDate|DateTimeOffset|请求处理终止的日期（成功或失败）。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|id|String|只读。|
|requestType|accessPackageRequestType|请求的类型。 可能的值是 `notSpecified` `userAdd` `userUpdate` `userRemove` `adminAdd` `adminUpdate` ：、、、、、、、。 `adminRemove` `systemAdd` `systemUpdate` `systemRemove` `onBehalfAdd` `unknownFutureValue` 来自用户本身的请求的 requestType 为 `UserAdd` 或 `UserRemove` 。 一旦设置此属性，就无法更改。|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|要分配给请求者的日期范围。 一旦设置此属性，就无法更改。|
|state|accessPackageRequestState|请求的状态。 可取值包括：`submitted`、`pendingApproval`、`delivering`、`delivered`、`deliveryFailed`、`denied`、`scheduled`、`canceled`、`partiallyDelivered`、`unknownFutureValue`。 只读。|
|状态|String|有关请求处理状态详细信息。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessPackage|[accessPackage](../resources/accesspackage.md)|与 accessPackageAssignmentRequest 关联的访问包。 访问包定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。 只读。 可为 NULL。 <br/><br/> 支持 `$expand`。|
|工作分配|[accessPackageAssignment](../resources/accesspackageassignment.md)|对于 **或** 的 `UserAdd` `AdminAdd` requestType，这是请求创建的访问包分配。  对于 、 或 的 **requestType，** 此属性具有要删除的现有 `UserRemove` `AdminRemove` `SystemRemove` `id` 工作分配的 属性。  <br/><br/> 支持 `$expand`。|
|requestor|[accessPackageSubject](../resources/accesspackagesubject.md)|请求或分配了直接分配（如果为直接分配）的主题。 只读。 可为 NULL。 支持 `$expand`。|

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
  "completedDate": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


