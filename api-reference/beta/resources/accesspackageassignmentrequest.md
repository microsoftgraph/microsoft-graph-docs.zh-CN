---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7d7fcf663abf15478b0c2745e9c60e1021d1ee7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508546"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>accessPackageAssignmentRequest 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包分配请求由要获取访问包分配的用户创建。 如果请求成功，并且具有必要的审批，则用户将收到访问包分配，并且是最终的访问包分配的主题。  Azure AD 还会自动创建访问包分配请求，以用于跟踪访问删除。


## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)集合 | 检索 accesspackageassignmentrequest 对象的列表。 |
| [创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 accessPackageAssignmentRequest。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 accessPackageAssignmentRequest 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|请求的处理结束日期（成功或失败）。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|id|String| 只读。|
|isValidationOnly|布尔|如果请求不处理工作分配，则为 True。|
|合理化|String|请求者提供的理由。|
|requestState|String|、 `Denied` `Delivered` `Submitted` 、或`Scheduled`的其中`PartiallyDelivered`一个。 只读。|
|requestStatus|String|有关请求处理状态的详细信息。 只读。|
|requestType|String|、 `UserAdd` `UserRemove` `AdminRemove` 、或`SystemRemove`的其中`AdminAdd`一个。 只读。|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| 请求创建的访问包分配。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|请求程序|[accessPackageSubject](accesspackagesubject.md)| 分配了请求的主题或分配了直接分配的主题。 此为只读属性。 可为 Null。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "2020-02-12T22:06:58.303Z",
  "completedDate": "2020-02-12T22:14:28.19Z",
  "id": "1244d439-5baa-4b9a-be5f-e8fdef5a998b",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "justification": ""
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
