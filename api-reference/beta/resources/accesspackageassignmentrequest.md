---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由想要获取访问包分配的用户创建。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b12d512b34c1b42751cae22c6a387ff9c2e69e8d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337521"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>accessPackageAssignmentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](entitlementmanagement-overview.md)，访问包分配请求由希望获取访问包分配的用户或代表该用户创建。 如果请求成功，并且经过任何必要的审批，用户将收到访问包分配，并且是生成的访问包分配的主题。  Azure AD还自动创建访问包分配请求，以跟踪访问删除。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignmentRequests](../api/entitlementmanagement-list-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合 | 检索 **accesspackageassignmentrequest 对象** 的列表。 |
| [创建 accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 **accessPackageAssignmentRequest**。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 **accessPackageAssignmentRequest** 对象的属性和关系。 |
| [删除 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |无 | 删除 **accessPackageAssignmentRequest**。 |
|[filterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|检索已登录 **用户筛选的 accessPackageAssignmentRequest** 对象列表。|
|[取消](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|取消 **处于可取消状态中的 accessPackageAssignmentRequest** 对象。|
| [重新处理](../api/accesspackageassignmentrequest-reprocess.md) | 无 | 自动重试用户对访问包的访问请求。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|请求处理终止的日期（成功或失败）。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|customExtensionHandlerInstances|[customExtensionHandlerInstance](../resources/customextensionhandlerinstance.md) 集合| 对分配 [请求运行的](customaccesspackageworkflowextension.md) 自定义工作流扩展实例的集合。 只读。 |
|id|字符串| 只读。|
|isValidationOnly|Boolean|如此 如果不处理工作分配的请求。|
|justification|String|请求者提供的理由。|
|requestState|String|、 、 `Denied`、 `Delivering`、 `Delivered`、 `PartiallyDelivered`、 `DeliveryFailed`或 `Submitted` 之一`Scheduled`。`PendingApproval``Canceled` 只读。|
|requestStatus|字符串|有关请求处理状态详细信息。 只读。|
|requestType|String|`UserAdd`、 、 `UserRemove``AdminAdd`或 `AdminRemove` 之一`SystemRemove`。 来自用户本身的请求的 requestType 为 `UserAdd` 或 `UserRemove`。 只读。|
|schedule|[requestSchedule](requestschedule.md)| 要分配给请求者的日期范围。 只读。|
|answers|[accessPackageAnswer](accesspackageanswer.md) 集合|请求者提供的 [accessPackageQuestions](accesspackagequestion.md) 在请求时询问他们的答案。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](../resources/accesspackage.md)|与 accessPackageAssignmentRequest 关联的访问包。 访问包定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。 只读。 可为 NULL。 支持 `$expand`。|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| 对于 **或 的 requestType** `UserAdd` `AdminAdd`，这是请求创建的访问包分配。  对于 、 或 `SystemRemove`的 **requestType**`UserRemove``AdminRemove`，此属性`id`具有要删除的现有工作分配的 属性。  支持 `$expand`。|
|requestor|[accessPackageSubject](accesspackagesubject.md)| 请求或分配了直接分配（如果为直接分配）的主题。 只读。 可为 NULL。 支持 `$expand`。|


## <a name="json-representation"></a>JSON 表示形式


下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequest",
  "id": "String (identifier)",
  "requestType": "String",
  "requestState": "String",
  "requestStatus": "String",
  "isValidationOnly": "Boolean",
  "createdDateTime": "String (timestamp)",
  "completedDate": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "justification": "String",
  "schedule": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "answers": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerString"
    }
  ],
  "customExtensionHandlerInstances": [
    {
      "@odata.type": "microsoft.graph.customExtensionHandlerInstance"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
