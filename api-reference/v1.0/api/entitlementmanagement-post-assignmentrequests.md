---
title: 创建 accessPackageAssignmentRequest
description: 创建新的 accessPackageAssignmentRequest。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 827020fd3da1c4b52dd95f67bb0550fbfcb9253a
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607895"
---
# <a name="create-accesspackageassignmentrequest"></a>创建 accessPackageAssignmentRequest

命名空间：microsoft.graph


在[Azure AD管理](../resources/entitlementmanagement-overview.md)中，创建新的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。  此操作用于将用户分配给访问包或删除访问包分配。


## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/assignmentRequests
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 \{token\}。必需。 |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象的 JSON 表示形式。

对于要请求为用户创建工作分配的管理员，**requestType** `AdminAdd`属性的值为 ，`targetId`分配属性包含要分配的用户的 、标识 accessPackageAssignmentPolicy 的 **assignmentPolicyId** 属性和标识 [accessPackage](../resources/accesspackage.md) 的 **accessPackageId** 属性。

对于请求删除工作分配的管理员，**requestType** `AdminRemove`属性的值为 ，分配属性包含标识要删除的 [accessPackageAssignment](../resources/accesspackageassignment.md) 的 **id** 属性。

对于非管理员用户请求为第一个分配或续订分配创建自己的工作分配， **requestType** 属性的值为 `UserAdd`。 **赋值** 属性包含具有 的用户 `targetId` `id` 的对象。 **assignmentPolicyId** 属性标识 accessPackageAssignmentPolicy。 **accessPackageId** 属性标识 [accessPackage](../resources/accesspackage.md)。 提出请求的用户必须已存在于 目录中。

对于非管理员用户请求扩展其自己的分配， **requestType** 属性的值为 `UserExtend`。 **assignment** 属性包含与`targetId``id`用户的 的 。 **assignmentPolicyId** 属性标识 accessPackageAssignmentPolicy。 **accessPackageId** 属性标识 [accessPackage](../resources/accesspackage.md)。 提出请求的用户必须已存在于 目录中。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 200 系列响应代码和新 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。

如果这是请求， `AdminAdd` 则随后会 [创建 accessPackageAssignment](../resources/accesspackageassignment.md) ，如果需要，还会创建 [accessPackageSubject](../resources/accesspackagesubject.md) 。 在列出 [accessPackageAssignments 时，可以使用查询参数查找这些参数](entitlementmanagement-list-assignments.md)。

## <a name="examples"></a>示例

### <a name="example-1-admin-requests-a-direct-assignment-for-a-user-already-in-the-directory"></a>示例 1：管理员为目录中已有的用户请求直接分配
#### <a name="request"></a>请求

下面是直接分配请求的一个示例，其中管理员请求为用户创建工作分配。 由于 [accessPackageSubject](../resources/accesspackagesubject.md) 可能尚不存在， **targetID** 的值是所分配用户的对象 ID， **accessPackageId** 的值是该用户所需的访问包， **assignmentPolicyId** 的值是该访问包中的直接分配策略。


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "assignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```

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
  "requestStatus": "Accepted"
}
```

### <a name="example-2-remove-an-assignment"></a>示例 2：删除工作分配

若要删除分配，请创建具有以下设置的新 accessPackageAssignmentRequest 对象：

+ **requestType** 属性的值设置为 `AdminRemove`。
+ 在 assignment 属性中，包括具有要删除的 accessPackageAssignment 对象的标识符的对象。

#### <a name="request"></a>请求

以下示例演示如何删除工作分配。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentRequests
Content-type: application/json

{
    "requestType": "AdminRemove",
    "assignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#accessPackageAssignmentRequests/$entity",

    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted"
}
```

