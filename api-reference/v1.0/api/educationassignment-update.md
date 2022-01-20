---
title: 更新 educationassignment
description: 更新 educationAssigment 对象。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: faca28843e5e9b6c6f4eadea6f9be265ff56bd9e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092358"
---
# <a name="update-educationassignment"></a>更新 educationassignment

命名空间：microsoft.graph

更新 [educationAssignment](../resources/educationassignment.md) 对象。 

只有教师才能执行此操作。 

或者，通过发布操作 **请求更改** 工作 [分配](../api/educationassignment-publish.md) 的状态。 请勿将 PATCH 操作用于此目的。

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
PATCH /education/classes/{class-id}/assignments/{assignment-id}
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，仅提供要更新的字段的值。 

请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|addedStudentAction|String| 描述是否应当将作业分发给在作业发布日期之后添加的学生。|
|addToCalendarAction|educationAddToCalendarOptions|可选字段，用于控制 **发布** 作业时将作业添加到学生和教师日历 **的作业** 行为。 可能的值包括 `none`、`studentsAndPublisher`、`studentsAndTeamOwners`、`unknownFutureValue`、`studentsOnly`。 请注意，必须使用此可变化枚举 (请求) 获取以下 `Prefer: include - unknown -enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `studentsOnly` ： 。 可选。|
|allowLateSubmissions|布尔| 学生是否可以在截止日期后发送提交。|
|allowStudentsToAddResourcesToSubmission|布尔| 学生是否可以向提交中添加资源。 此外，指示提交中所有资源是否对应于工作分配资源列表。 |
|assignDateTime|DateTimeOffset| 指示向学生发布作业的日期。 工作分配发布后无法编辑。|
|assignTo|[educationAssignmentRecipient](../resources/educationassignmentrecipient.md)| 获得作业的学生。|
|closeDateTime|DateTimeOffset| 工作分配关闭提交的日期。 如果分配不允许LateSubmissions或 closeDateTime 与 dueDateTime 相同，则该字段可以是 null 的可选字段，但如果指定，它必须大于或等于 dueDateTime。|
|displayName|String| 工作分配的名称。 |
|dueDateTime|DateTimeOffset| 日期分配到期。 |
|一个|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)| 如何对作业进行评分。|
|instructions|itemBody| 要与作业一起向学生提供的说明。 |
|notificationChannelUrl|String| 与分配相关的通知通信的通道。 若要更改 URL，将值设置为 `assignTo` [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md)。 频道 URL 在工作分配发布后不能更改。|

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationAssignment](../resources/educationassignment.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["72a7baec-c3e9-4213-a850-f62de0adad5f","4679bc1b-90c5-45af-ae1a-d5357672ed39"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39
Content-type: application/json

{
    "displayName": "Reading and review test 09.03 #5",
    "instructions": {
        "contentType": "text",
        "content": "Read chapter 5 and write your review"
    },
    "dueDateTime": "2021-09-10T00:00:00Z",
    "addedStudentAction": "none"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-educationassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-educationassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('72a7baec-c3e9-4213-a850-f62de0adad5f')/assignments/$entity",
    "classId": "72a7baec-c3e9-4213-a850-f62de0adad5f",
    "displayName": "Reading and review test 09.03 #5",
    "closeDateTime": null,
    "dueDateTime": "2021-09-10T00:00:00Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "createdDateTime": "2021-09-03T23:57:14.6088791Z",
    "lastModifiedDateTime": "2021-09-04T15:01:35.3361649Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%2272a7baec-c3e9-4213-a850-f62de0adad5f%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%224679bc1b-90c5-45af-ae1a-d5357672ed39%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addedStudentAction": "none",
    "id": "4679bc1b-90c5-45af-ae1a-d5357672ed39",
    "instructions": {
        "content": "Read chapter 5 and write your review",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 50
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
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
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
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


