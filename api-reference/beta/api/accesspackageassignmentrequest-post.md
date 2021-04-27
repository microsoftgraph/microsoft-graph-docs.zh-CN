---
title: 创建 accessPackageAssignmentRequest
description: 创建新的 accessPackageAssignmentRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ff0f60841fe852d67e5c76268fe4e00ce277af11
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048594"
---
# <a name="create-accesspackageassignmentrequest"></a>创建 accessPackageAssignmentRequest

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，创建新的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。  此操作用于将用户分配给访问包或删除访问包分配。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 \{token\}。必需。 |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象的 JSON 表示形式。

对于请求为用户创建工作分配的管理员 **，requestType** 属性的值为 ，accessPackageAssignment 属性包含要分配的用户的 、标识 `AdminAdd`  `targetId` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)的 **assignmentPolicyId** 属性和标识 accessPackage 的 **accessPackageId**[](../resources/accesspackage.md)属性。

对于请求删除分配的管理员 **，requestType** 属性的值为 `AdminRemove` **，accessPackageAssignment** 属性包含标识要删除的 [accessPackageAssignment](../resources/accesspackageassignment.md)的 **id** 属性。

对于需要自行创建工作分配的非管理员用户 **，requestType** 属性的值为 ，accessPackageAssignment 属性包含具有用户本身 ID 的 、 `UserAdd`  `targetId` 标识 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)的 **assignmentPolicyId** 属性和标识 accessPackage 的 **accessPackageId**[](../resources/accesspackage.md)属性。  提出请求的用户必须已存在于 目录中。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 200 系列响应代码和新 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。  

如果这是请求，则随后会 `AdminAdd` [创建 accessPackageAssignment，](../resources/accesspackageassignment.md)如果需要，还会创建[accessPackageSubject。](../resources/accesspackagesubject.md) 在列出 [accessPackageAssignments](accesspackageassignment-list.md)时，可以使用查询参数查找这些参数。

## <a name="examples"></a>示例
### <a name="example-1-admin-requests-a-direct-assignment-for-a-user"></a>示例 1：管理员请求直接分配用户
#### <a name="request"></a>请求

下面是直接分配请求的一个示例，其中管理员请求为用户创建工作分配。 由于 [accessPackageSubject](../resources/accesspackagesubject.md) 可能尚不存在 **，targetID** 的值是分配的用户的对象 **ID，accessPackageId** 的值是该用户所需的访问包 **，assignmentPolicyId** 的值是该访问包中的直接分配策略。
 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

### <a name="example-2-user-requests-a-package-and-answers-questions-for-approval"></a>示例 2：用户请求程序包并回答需要审批的问题
#### <a name="request"></a>请求

下面是请求的一个示例，请求者向审批者提供了答案以帮助他们做出决策。
 



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "targetId": "46184453-e63b-4f20-86c2-c557ed5d5df9",
        "assignmentPolicyId": "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
        }
    }]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


#### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e382d02-4454-436b-b700-59c7dd77f466",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF",
            "isRequired": false,
            "text": {
                "defaultText": "what state are you from?",
                "localizedTexts": [{
                    "text": "¿De qué estado eres?",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
            "choices": [{
                "actualValue": "AZ",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Arizona",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "CA",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "California",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "OH",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Ohio",
                        "languageCode": "es"
                    }]
                }
            }],
            "allowsMultipleSelection": false
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA",
            "isRequired": false,
            "text": {
                "defaultText": "Who is your manager?",
                "localizedTexts": [{
                    "text": "por qué necesita acceso a este paquete",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": false
        }
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


