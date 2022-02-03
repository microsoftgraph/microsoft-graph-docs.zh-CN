---
title: educationSubmission：重新分配
description: 将提交重新分配给学生并反馈评价。
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5621a0682a35f06acc41e198375845ea8f87027a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343581"
---
# <a name="educationsubmission-reassign"></a>educationSubmission：重新分配

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将 [提交重新](../resources/educationsubmission.md) 分配给学生并反馈评价。

只有教师才能执行此操作。 

`Prefer: include-unknown-enum-members`调用此方法时包含 标头;否则，重新分配的提交将被视为返回的提交。 这意味着状态将`reassigned``returned`映射到状态，**reassignedDateTime** 和 **reassignedBy** 属性将分别映射到 **returnedDateTime** 和 **returnedBy**。

如果提供了标头 `Prefer: include-unknown-enum-members` ，则重新分配的提交将保留状态 `reassigned` 。 有关详细信息，请参阅示例部分。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite   |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | 不支持。 | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Prefer  | `include-unknown-enum-members`. 可选。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmission](../resources/educationsubmission.md) 对象。

## <a name="examples"></a>示例
### <a name="example-1-request-without-optional-prefer-header"></a>示例 1：没有可选首选标头的请求

#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_reassign"
}-->

```http
POST /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/7192332b-e904-4891-81e2-356242ab1858/submissions/02bb5de1-7205-2a25-fe33-f99cf53de1c4/reassign
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-reassign-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-reassign-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-reassign-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-reassign-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationsubmission-reassign-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/educationsubmission-reassign-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面是请求标头 `Prefer: include-unknown-enum-members` 中未提供且之前未返回提交时的响应示例。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationSubmission",
    "@odata.type": "#microsoft.graph.educationSubmission",
    "status": "returned",
    "submittedDateTime": "2021-09-07T14:54:46.1606962Z",
    "unsubmittedDateTime": "2021-09-07T14:41:18.9512645Z",
    "returnedDateTime": "2021-09-07T21:38:40.5254847Z",
    "reassignedDateTime": "2021-09-07T21:38:40.5254847Z",
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
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    },
    "reassignedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f3a5344e-dbde-48b0-be24-b5b62a243836",
            "displayName": null
        }
    }
}
```

### <a name="example-2-request-with-prefer-header"></a>示例 2：具有 Prefer 标头的请求
以下示例演示如何调用此方法。

#### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_prefer_reassign"
}-->

```http
POST /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/7192332b-e904-4891-81e2-356242ab1858/submissions/02bb5de1-7205-2a25-fe33-f99cf53de1c4/reassign
Prefer: include-unknown-enum-members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-prefer-reassign-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-prefer-reassign-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-prefer-reassign-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-prefer-reassign-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationsubmission-prefer-reassign-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/educationsubmission-prefer-reassign-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面是请求标头中提供 `Prefer: include-unknown-enum-members` 且之前未返回提交时的响应示例。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#educationSubmission",
    "@odata.type": "#microsoft.graph.educationSubmission",
    "status": "reassigned",
    "submittedDateTime": "2021-09-07T21:44:41.8377109Z",
    "unsubmittedDateTime": "2021-09-07T14:41:18.9512645Z",
    "returnedDateTime": null,
    "reassignedDateTime": "2021-09-07T21:45:42.9027726Z",
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
    },
    "reassignedBy": {
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
  "description": "educationSubmission: reassign",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


