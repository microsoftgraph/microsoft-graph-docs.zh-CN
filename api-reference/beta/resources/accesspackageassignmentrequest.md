---
title: accessPackageAssignmentRequest 资源类型
description: 访问包分配请求由想要获取访问包分配的用户创建。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ce7d47ccb4e911689e9398c2514cb8311b3ae0a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155606"
---
# <a name="accesspackageassignmentrequest-resource-type"></a>accessPackageAssignmentRequest 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包分配请求由想要获取访问包分配的用户创建或代表用户创建。 如果请求成功，则用户会收到访问包分配，并经过任何必要的审批，并作为生成的访问包分配的主题。  Azure AD 还会自动创建访问包分配请求，以跟踪访问删除。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合 | 检索 accesspackageassignmentrequest 对象的列表。 |
| [创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 accessPackageAssignmentRequest。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 accessPackageAssignmentRequest 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|completedDate|DateTimeOffset|请求处理结束的日期（成功或失败）。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 只读。|
|id|String| 只读。|
|isValidationOnly|布尔|如此 如果不处理工作分配的请求。|
|justification|String|请求者提供的理由。|
|requestState|String|`PendingApproval` `Canceled` `Denied` 、、、、或 之 `Delivering` `Delivered` `PartiallyDelivered` `Submitted` 一 `Scheduled` 。 只读。|
|requestStatus|String|有关请求处理状态的信息。 只读。|
|requestType|String|之 `UserAdd` 一 `UserRemove` ， ， 或 `AdminAdd` `AdminRemove` `SystemRemove` 。 来自用户本身的请求将具有的 requestType `UserAdd` 或 `UserRemove` 。 只读。|
|schedule|[requestSchedule](requestschedule.md)| 要分配给请求者的日期范围。 只读。|
|accessPackageAssignment|[accessPackageAssignment](accesspackageassignment.md)| 对于 or 的 `UserAdd` `AdminAdd` requestType，这是请求创建的访问包分配。  对于或 的 `UserRemove` `AdminRemove` `SystemRemove` requestType，此属性具有要删除 `id` 的现有工作分配的属性。|
|answers|[accessPackageAnswer](accesspackageanswer.md) 集合|请求者提供的对 [accessPackageQuestions](accesspackagequestion.md) 的回答在请求时询问他们。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|requestor|[accessPackageSubject](accesspackagesubject.md)| 请求或分配了直接分配的主题。 只读。 可为 Null。|

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
    "createdDateTime": "string",
    "completedDate": "string",
    "id": "string",
    "requestType": "string",
    "requestState": "string",
    "requestStatus": "string",
    "isValidationOnly": false,
    "justification": "string",
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "string",
        "answeredQuestion": {
            "id": "string",
            "text": {
                "defaultText": "string",
                "localizedTexts": [{
                    "text": "string",
                    "languageCode": "string"
                }]
            },
            "isRequired": true,
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": true
        }
    }]
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

