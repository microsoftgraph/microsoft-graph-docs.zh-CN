---
title: 更新 educationassignment
description: 更新的 assignment 对象。 仅教师类中的可以执行此操作。 请注意，您无法使用 PATCH 请求更改的工作分配状态。 使用发布操作更改的工作分配状态。
localization_priority: Normal
ms.openlocfilehash: 78d5b526468fbdf35c3529084f878f8c35216c99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838288"
---
# <a name="update-educationassignment"></a>更新 educationassignment

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新的 assignment 对象。 仅教师类中的可以执行此操作。 请注意，您无法使用 PATCH 请求更改的工作分配状态。 使用[发布](../api/educationassignment-publish.md)操作更改的工作分配状态。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadWriteBasic EduAssignments.ReadWrite  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | 不支持。 | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|allowLateSubmissions|布尔| 是否可以在截止日期之后提交提交。|
|allowStudentsToAddResourcesToSubmission|布尔| 是否学生可以将资源添加到提交。 指示在提交的那些项目是否来自工作分配资源列表。 |
|assignDateTime|DateTimeOffset| 应将工作分配发布到学生的日期。 |
|assignTo|educationAssignmentRecipient| 获取工作分配的学生。|
|displayName|字符串| 工作分配的名称。 |
|dueDateTime|DateTimeOffset| 截止日期工作分配。 |
|分级|educationAssignmentGradeType| 如何将评分工作分配。|
|说明|itemBody| 要赋予以及工作分配学生的说明。 |

## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[educationAssignment](../resources/educationassignment.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
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
##### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 将从实际调用中返回所有属性。

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
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
