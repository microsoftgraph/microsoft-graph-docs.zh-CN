---
title: educationSubmission：未提交
description: '一种操作，指示学生想要在作业提交后进行作业提交。 此操作仅能由学生执行。 '
author: dipakboyed
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e7d06aabec1a13888309c90d44e2f32a89bb58fb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981853"
---
# <a name="educationsubmission-unsubmit"></a>educationSubmission：未提交

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指示学生想要在作业提交后处理作业提交。 此操作仅能由学生执行。 这会将提交状态从"已提交"更改为"正在工作"。 在提交过程中，所有资源都将从 submittedResources 复制到 workingResources 存储桶。 教师将查看工作资源列表进行评分。

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
POST /education/classes/{class-id}/assignments/{assignment-id}/submissions/{submission-id}/unsubmit
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在 `200 Ok` 响应正文中返回 响应代码和 [educationSubmission](../resources/educationsubmission.md) 对象。

## <a name="example"></a>示例
以下示例演示如何调用此 API。
### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/7192332b-e904-4891-81e2-356242ab1858/submissions/02bb5de1-7205-2a25-fe33-f99cf53de1c4/unsubmit
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationsubmission-unsubmit-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->

```http
HTTP/1.1 200 Ok

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationSubmission",
    "@odata.type": "#microsoft.graph.educationSubmission",
    "status": "returned",
    "submittedDateTime": null,
    "unsubmittedDateTime": "2021-09-07T14:41:18.9512645Z",
    "returnedDateTime": null,
    "resourcesFolderUrl": null,
    "id": "02bb5de1-7205-2a25-fe33-f99cf53de1c4",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "80cefd93-8d88-40e2-b5d3-67898383e226"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "80cefd93-8d88-40e2-b5d3-67898383e226",
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


