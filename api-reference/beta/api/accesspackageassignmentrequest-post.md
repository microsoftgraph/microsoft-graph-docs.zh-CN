---
title: 创建 accessPackageAssignmentRequest
description: 创建新的 accessPackageAssignmentRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 128c4c84879ec11c6ac0b54991247b84125285f2
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108404"
---
# <a name="create-accesspackageassignmentrequest"></a>创建 accessPackageAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，创建一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。  此操作用于将用户分配给访问包，或删除访问包分配。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 \{token\}。 必填。 |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的 JSON 表示形式。

若要为用户创建分配， **requestType** `AdminAdd`属性的值是， **accessPackageAssignment**属性包含`targetId`被分配的用户、 **assignmentPolicyId**属性（标识[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)）和标识[accessPackage](../resources/accesspackage.md)的**accessPackageId**属性。

若要删除分配， **requestType**属性`AdminRemove`的值是， **accessPackageAssignment**属性包含标识要删除的[accessPackageAssignment](../resources/accesspackageassignment.md)的**id**属性。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是一个直接分配请求的示例。  **TargetID**的值是要分配的用户的对象 ID， **accessPackageId**的值是所需的访问包，而**assignmentPolicyId**的值是该访问包中的直接分配策略。
 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
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
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
