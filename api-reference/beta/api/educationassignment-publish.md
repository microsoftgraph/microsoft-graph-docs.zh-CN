---
title: educationAssignment： publish
description: 将 educationAssignment 的状态从原始草稿状态更改为已发布状态。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fd3daac7d17b4b88c5f17d3d2a1dca676cfa602b
ms.sourcegitcommit: 7a0f9f1a535795c6f77c80e02fd97581c36f1273
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/27/2021
ms.locfileid: "61608981"
---
# <a name="educationassignment-publish"></a>educationAssignment： publish

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 [educationAssignment 的状态](../resources/educationassignment.md) 从原始 `draft` 状态更改为 `published` 状态。 

如果工作分配计划在将来的日期 `draft` ，您可以将状态 `scheduled` 从 更改为 。  

只有课堂中的教师才能进行此呼叫。 当 **作业** 为草稿状态时，学生将看不到作业，也不会看到任何提交对象。 调用此 API 时， [将创建 educationSubmission](../resources/educationsubmission.md) 对象，作业将显示在学生列表中。

如果发布 **过程中出现** 任何后端故障，则分配 `draft` 的状态将返回。

若要更新已发布的工作分配 **的属性，** 请参阅 [更新工作分配](../api/educationassignment-update.md)。

若要更新已发布的工作分配的属性，请参阅 [更新工作分配](../api/educationassignment-update.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | 不支持。 | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 Ok` 正文中返回 响应代码和 [educationAssignment](../resources/educationassignment.md) 对象。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","1b6df208-ea5a-475c-8dd2-b92f693c928a"],
  "name": "educationassignment_publish_2"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1b6df208-ea5a-475c-8dd2-b92f693c928a/publish
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationassignment-publish-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
响应示例如下所示。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->

```http
HTTP/1.1 200 Ok

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationAssignment",
    "@odata.type": "#microsoft.graph.educationAssignment",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Reading Test 09.03 3",
    "closeDateTime": null,
    "dueDateTime": "2021-09-05T06:59:00Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "createdDateTime": "2021-09-03T23:26:35.4182773Z",
    "lastModifiedDateTime": "2021-09-03T23:28:05.0704312Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "published",
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%221b6df208-ea5a-475c-8dd2-b92f693c928a%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addToCalendarAction": "none",
    "addedStudentAction": "none",
    "id": "1b6df208-ea5a-475c-8dd2-b92f693c928a",
    "grading": null,
    "instructions": {
        "content": "",
        "contentType": "text"
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
    },
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "AAAAAAAA-0123-4567-89AB-1B4BB48C3119",
            "displayName": null
        }
    }
}
```

## <a name="see-also"></a>另请参阅

* [分配和提交状态、转换和限制](/graph/assignments-submissions-states-transition)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


