---
title: 创建 assignmentPolicies
description: 创建新的 accessPackageAssignmentPolicy 对象。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c4337a07e9667ac23d3d0c386964fc1f9f44a275
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209600"
---
# <a name="create-assignmentpolicies"></a>创建 assignmentPolicies
命名空间：microsoft.graph

在[Azure AD权利管理](../resources/entitlementmanagement-overview.md)中，创建新的 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。  请求将包含对将包含此策略的 [accessPackage](../resources/accesspackage.md) 的引用，该策略必须已经存在。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.ReadWrite.All  |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | EntitlementManagement.ReadWrite.All |


## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/assignmentPolicies
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的 JSON 表示形式。

创建 **accessPackageAssignmentPolicy** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|说明|String|策略的说明。|
|displayName|字符串|策略的显示名称。|
|allowedTargetScope|allowedTargetScope|允许通过此策略为Who分配访问包。 可取值包括：`notSpecified`、`specificDirectoryUsers`、`specificConnectedOrganizationUsers`、`specificDirectoryServicePrincipals`、`allMemberUsers`、`allDirectoryUsers`、`allDirectoryServicePrincipals`、`allConfiguredConnectedOrganizationUsers`、`allExternalUsers`、`unknownFutureValue`。 可选。|
|到期|[expirationPattern](../resources/expirationpattern.md)|在此策略中创建的分配的到期日期。|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|指定通过此策略批准访问包分配请求的设置。 例如，如果新请求需要审批。|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|提供其他设置，以选择谁可以通过此策略创建访问包分配请求，以及它们可以包含在请求中的内容。|
|specificAllowedTargets|[subjectSet](../resources/subjectset.md) 集合|从此策略的访问包分配访问权限的目标。|
|accessPackage|[accessPackage](../resources/accesspackage.md)| 对将包含必须已存在的策略的访问包的引用。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-create-a-direct-assignment-policy"></a>示例 1：创建直接分配策略

当访问包分配请求仅由管理员而不是用户自己创建时，直接分配策略非常有用。

#### <a name="request"></a>请求

以下示例演示创建访问包分配策略的请求。 在此策略中，没有用户可以请求，也不需要审批，也没有访问评审。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
Content-Type: application/json

{
  "displayName": "New Policy",
  "description": "policy for assignment",
  "allowedTargetScope": "notSpecified",
  "specificAllowedTargets": [],
  "expiration": {
      "endDateTime": null,
      "duration": null,
      "type": "noExpiration"
  },
  "requestorSettings": {
      "enableTargetsToSelfAddAccess": false,
      "enableTargetsToSelfUpdateAccess": false,
      "enableTargetsToSelfRemoveAccess": false,
      "allowCustomAssignmentSchedule": true,
      "enableOnBehalfRequestorsToAddAccess": false,
      "enableOnBehalfRequestorsToUpdateAccess": false,
      "enableOnBehalfRequestorsToRemoveAccess": false,
      "onBehalfRequestors": []
  },
  "requestApprovalSettings": {
      "isApprovalRequiredForAdd": false,
      "isApprovalRequiredForUpdate": false,
      "stages": []
  },
  "accessPackage": {
      "id": "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accesspackageassignmentpolicy-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-accesspackageassignmentpolicy-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "New policy",
  "description": "policy for assignment"
}
```

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a>示例 2：为其他组织的用户创建要请求的策略

下面的示例演示了一个更复杂的策略，其中有两个阶段的审批。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_2"
}
-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
Content-Type: application/json

{
    "displayName": "policy for external access requests",
    "description": "policy for users from connected organizations to request access, with two stages of approval.",
    "allowedTargetScope": "allConfiguredConnectedOrganizationUsers",
    "specificAllowedTargets": [],
    "expiration": {
        "type": "noExpiration"
    },
    "requestorSettings": {
        "enableTargetsToSelfAddAccess": true,
        "enableTargetsToSelfUpdateAccess": true,
        "enableTargetsToSelfRemoveAccess": true,
        "allowCustomAssignmentSchedule": false,
        "enableOnBehalfRequestorsToAddAccess": false,
        "enableOnBehalfRequestorsToUpdateAccess": false,
        "enableOnBehalfRequestorsToRemoveAccess": false,
        "onBehalfRequestors": []
    },
    "requestApprovalSettings": {
        "isApprovalRequiredForAdd": true,
        "isApprovalRequiredForUpdate": false,
        "stages": [
            {
                "durationBeforeAutomaticDenial": "P14D",
                "isApproverJustificationRequired": false,
                "isEscalationEnabled": false,
                "durationBeforeEscalation": "PT0S",
                "primaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.internalSponsors"
                    }
                ],
                "fallbackPrimaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "userId": "7deff43e-1f17-44ef-9e5f-d516b0ba11d4"
                    },
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "groupId": "1623f912-5e86-41c2-af47-39dd67582b66"
                    }
                ],
                "escalationApprovers": [],
                "fallbackEscalationApprovers": []
            },
            {
                "durationBeforeAutomaticDenial": "P14D",
                "isApproverJustificationRequired": false,
                "isEscalationEnabled": false,
                "durationBeforeEscalation": "PT0S",
                "primaryApprovers": [],
                "fallbackPrimaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "userId": "46184453-e63b-4f20-86c2-c557ed5d5df9"
                    },
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "groupId": "1623f912-5e86-41c2-af47-39dd67582b66"
                    }
                ],
                "escalationApprovers": [],
                "fallbackEscalationApprovers": []
            }
        ]
    },
    "accessPackage": {
        "id": "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-accesspackageassignmentpolicy-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "9d8f2361-39be-482e-b267-34ad6baef4d3",
    "displayName": "policy for external access requests",
    "description": "policy for users from connected organizations to request access, with two stages of approval."
}
```

