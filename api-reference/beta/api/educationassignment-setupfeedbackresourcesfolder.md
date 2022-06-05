---
title: educationAssignment： setUpFeedbackResourcesFolder
description: 创建 SharePoint 文件夹以上传给定 educationSubmission 的反馈文件。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ed6381c3b5c7a9f6cdc0013d1c520a05374f6910
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900547"
---
# <a name="educationassignment-setupfeedbackresourcesfolder"></a>educationAssignment： setUpFeedbackResourcesFolder

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建 SharePoint 文件夹以上传给定 [educationSubmission](../resources/educationsubmission.md) 的反馈文件。

教师确定要在提交的反馈资源文件夹中上传的资源。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadBasic、EduAssignments.Read  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|Application | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /classes/{classId}/assignments/{assignmentId}/setUpFeedbackResourcesFolder
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json           |

## <a name="request-body"></a>请求正文
在请求正文中，提供此方法的空 JSON 对象 `{}` 。

## <a name="response"></a>响应
如果成功，此方法在请求正文中返回 `200 OK` 响应代码和 [educationAssignment](../resources/educationassignment.md) 对象。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

### <a name="request"></a>请求
请求示例如下所示。

<!-- {
  "blockType": "request",
  "sampleKeys": ["37d99af7-cfc5-4e3b-8566-f7d40e4a2070","a3cce0ba-2008-4c4d-bf62-079408562d96"],  
  "name": "educationassignment_setupfeedbackresourcesfolder"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/37d99af7-cfc5-4e3b-8566-f7d40e4a2070/assignments/a3cce0ba-2008-4c4d-bf62-079408562d96/setUpFeedbackResourcesFolder
Content-type: application/json

{
}
```

### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationAssignment",
    "@odata.type": "#microsoft.graph.educationAssignment",
    "classId": "155c5142-1716-4c24-b2ac-cd1bcd8ad7ac",
    "displayName": "2022-02-25T18_57_26_443Z",
    "closeDateTime": null,
    "dueDateTime": "2022-02-25T18:57:26.443Z",
    "assignDateTime": null,
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "resourcesFolderUrl": null,
    "feedbackResourcesFolderUrl": "https://graph.microsoft.com/beta/drives/b!9i0vapy4v02vPa13nXvmLuPofkLptz5InpCzu0fn0IRzOBm8o5mJQbXuPddtkYG7/items/01PREZ76FARBTP25X74JFISOFAN7QAHOYW",
    "createdDateTime": "2022-02-24T18:57:27.8611453Z",
    "lastModifiedDateTime": "2022-02-24T18:57:40.5319603Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": null,
    "webUrl": "https://teams.microsoft.com/l/entity/66aeee93-507d-479a-a3ef-8f494af43945/classroom?context=%7B%22subEntityId%22%3A%22%7B%5C%22version%5C%22%3A%5C%221.0%5C%22,%5C%22config%5C%22%3A%7B%5C%22classes%5C%22%3A%5B%7B%5C%22id%5C%22%3A%5C%22155c5142-1716-4c24-b2ac-cd1bcd8ad7ac%5C%22,%5C%22displayName%5C%22%3Anull,%5C%22assignmentIds%5C%22%3A%5B%5C%22d10f56f7-ba7e-4dfc-b5a2-ae9f10b0d1ad%5C%22%5D%7D%5D%7D,%5C%22action%5C%22%3A%5C%22navigate%5C%22,%5C%22view%5C%22%3A%5C%22assignment-viewer%5C%22%7D%22,%22channelId%22%3Anull%7D",
    "addToCalendarAction": "none",
    "addedStudentAction": "none",
    "id": "d10f56f7-ba7e-4dfc-b5a2-ae9f10b0d1ad",
    "instructions": {
        "content": "2022-02-25T18_57_26_443Z",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient"
    },
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "fadaae59-b18c-44d1-993f-fe8a281bd69c",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2022-05-05 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: setUpFeedbackResourcesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
