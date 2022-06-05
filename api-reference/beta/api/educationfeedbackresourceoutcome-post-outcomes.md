---
title: 创建 educationFeedbackResourceOutcome
description: 为提交创建新的反馈资源。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d6d5a92ee8d4121b1e945ce8f94c041bc2f6a7d9
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900566"
---
# <a name="create-educationfeedbackresourceoutcome"></a>创建 educationFeedbackResourceOutcome

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为提交创建新的 [反馈资源](../resources/educationfeedbackresourceoutcome.md) 。

只有教师才能执行此操作。

若要创建新的基于文件的资源，请将文件上传到与分配关联的反馈资源文件夹。 如果文件不存在或不在该文件夹中，则 `POST` 请求将失败。

> [!IMPORTANT]
> 在上传作业反馈资源之前，必须为 [educationAssignment](../resources/educationassignment.md) [设置反馈资源文件夹](../api/educationassignment-setupfeedbackresourcesfolder.md)才能将文件上传到。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|Application | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{classId}/assignments/{assignmentId}/submissions/{submissionId}/outcomes
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json           |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [educationFeedbackResourceOutcome](../resources/educationfeedbackresourceoutcome.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [educationFeedbackResourceOutcome](../resources/educationfeedbackresourceoutcome.md) 对象。

此方法返回 `400 Bad Request` 提交超出五个以上反馈资源的情况。

## <a name="example"></a>示例
### <a name="request"></a>请求
请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "create_educationFeedbackResourceOutcome"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/37d99af7-cfc5-4e3b-8566-f7d40e4a2070/assignments/a3cce0ba-2008-4c4d-bf62-079408562d96/submissions/2185e6d7-2924-4ed1-dde1-269f89e29184/outcomes
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.educationFeedbackResourceOutcome",
    "feedbackResource": {
         "@odata.type": "#microsoft.graph.educationWordResource",
         "displayName": "Document1.docx"
     }
}
```

### <a name="response"></a>响应
下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFeedbackResourceOutcome"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/education/classes('37d99af7-cfc5-4e3b-8566-f7d40e4a2070')/assignments('a3cce0ba-2008-4c4d-bf62-079408562d96')/submissions('2185e6d7-2924-4ed1-dde1-269f89e29184')/outcomes/$entity",
    "@odata.type": "#microsoft.graph.educationFeedbackResourceOutcome",
    "lastModifiedDateTime": "2022-05-06T00:50:30.0772434Z",
    "id": "ba12f282-2190-4958-80b3-42b8afb9626a",
    "resourceStatus": "notPublished",
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
            "displayName": null
        }
    },
    "feedbackResource": {
        "@odata.type": "#microsoft.graph.educationWordResource",
        "displayName": "Document1.docx",
        "createdDateTime": "2022-05-06T00:50:30.0772177Z",
        "lastModifiedDateTime": "2022-05-06T00:50:30.0772434Z",
        "fileUrl": "https://graph.microsoft.com/beta/drives/b!-Ik2sRPLDEWy_bR8l75jfeDcpXQcRKVOmcml10NQLQ1F8CNZWU38SarWxPyWM7jx/items/01VANVJQZQ33I4AJBSURHZJDDQKEJ5TEMJ",
        "createdBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                "displayName": null
            }
        },
        "lastModifiedBy": {
            "application": null,
            "device": null,
            "user": {
                "id": "cb1a4af3-0aba-4679-aa12-9f99bab0b61a",
                "displayName": null
            }
        }
    }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2022-05-06 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationFeedbackResourceOutcome",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
