---
title: 更新 educationassignment
description: 更新 educationAssigment 对象。
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f754a8e4e79bd0043199924acbaf28eec8261716
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020040"
---
# <a name="update-educationassignment"></a>更新 educationassignment

命名空间：microsoft.graph

更新 educationAssigment 对象。 

只有教师才能执行此操作。 

或者，通过发布操作请求更改工作 [分配](../api/educationassignment-publish.md) 的状态。 请勿将 PATCH 操作用于此目的。

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
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
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
|allowLateSubmissions|Boolean| 学生是否可以在截止日期后发送提交。|
|allowStudentsToAddResourcesToSubmission|布尔值| 学生是否可以向提交中添加资源。 此外，指示提交中所有资源是否对应于工作分配资源列表。 |
|assignDateTime|DateTimeOffset| 指示向学生发布作业的日期。 |
|assignTo|educationAssignmentRecipient| 获得作业的学生。|
|closeDateTime|DateTimeOffset| 工作分配关闭提交的日期。 如果分配不允许LateSubmissions或 closeDateTime 与 dueDateTime 相同，则该字段可以是 null 的可选字段，但如果指定，它必须大于或等于 dueDateTime。|
|displayName|String| 工作分配的名称。 |
|dueDateTime|DateTimeOffset| 日期分配到期。 |
|一个|educationAssignmentGradeType| 如何对作业进行评分。|
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
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
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
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "closeDateTime": "2014-02-11T00:00:00Z",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
}
```

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


