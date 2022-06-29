---
title: 获取 unifiedRoleManagementPolicyAssignment
description: 获取角色管理策略分配的详细信息，包括与 Azure AD 角色关联的策略和规则。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 67c68443b5db9124b81e13187c9aa990c2681e77
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441286"
---
# <a name="get-unifiedrolemanagementpolicyassignment"></a>获取 unifiedRoleManagementPolicyAssignment
命名空间：microsoft.graph

获取角色管理策略分配的详细信息，包括与 Azure AD 角色关联的策略和规则。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleManagementPolicy.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagementPolicy.ReadWrite.Directory、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|Application|RoleManagement.Read.All、RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments/{unifiedRoleManagementPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` OData 查询参数， `$expand` 以帮助自定义响应。 还可以指定通配符值 `*` 以展开所有受支持的关系，即 `?$expand=*`。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-retrieve-a-role-management-policy-assignment"></a>示例 1：检索角色管理策略分配

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyassignment"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicyAssignments/Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicyassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicyassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicyassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicyassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedrolemanagementpolicyassignment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-unifiedrolemanagementpolicyassignment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicyAssignments/$entity",
    "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10",
    "policyId": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
    "scopeId": "/",
    "scopeType": "Directory",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
}
```


### <a name="example-2-retrieve-a-role-management-policy-assignment-and-expand-the-policy-and-its-associated-rules"></a>示例 2：检索角色管理策略分配并展开策略及其关联的规则

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyassignment_expand_all_relationships"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicyAssignments/Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10?$expand=policy($expand=rules)
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicyassignment-expand-all-relationships-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicyassignment-expand-all-relationships-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicyassignment-expand-all-relationships-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicyassignment-expand-all-relationships-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-unifiedrolemanagementpolicyassignment-expand-all-relationships-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-unifiedrolemanagementpolicyassignment-expand-all-relationships-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicyAssignments(policy(rules()))/$entity",
    "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10",
    "policyId": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
    "scopeId": "/",
    "scopeType": "Directory",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "policy": {
        "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
        "displayName": "Directory",
        "description": "Directory",
        "isOrganizationDefault": false,
        "scopeId": "/",
        "scopeType": "Directory",
        "lastModifiedDateTime": null,
        "lastModifiedBy": {
            "displayName": null,
            "id": null
        },
        "rules": [
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                "id": "Expiration_Admin_Eligibility",
                "isExpirationRequired": false,
                "maximumDuration": "P365D",
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Eligibility",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                "id": "Enablement_Admin_Eligibility",
                "enabledRules": [],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Eligibility",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Admin_Admin_Eligibility",
                "notificationType": "Email",
                "recipientType": "Admin",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Eligibility",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Requestor_Admin_Eligibility",
                "notificationType": "Email",
                "recipientType": "Requestor",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Eligibility",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Approver_Admin_Eligibility",
                "notificationType": "Email",
                "recipientType": "Approver",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Eligibility",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                "id": "Expiration_Admin_Assignment",
                "isExpirationRequired": false,
                "maximumDuration": "P180D",
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                "id": "Enablement_Admin_Assignment",
                "enabledRules": [
                    "Justification"
                ],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Admin_Admin_Assignment",
                "notificationType": "Email",
                "recipientType": "Admin",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Requestor_Admin_Assignment",
                "notificationType": "Email",
                "recipientType": "Requestor",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Approver_Admin_Assignment",
                "notificationType": "Email",
                "recipientType": "Approver",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "Admin",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
                "id": "Expiration_EndUser_Assignment",
                "isExpirationRequired": true,
                "maximumDuration": "PT8H",
                "target": {
                    "caller": "EndUser",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
                "id": "Enablement_EndUser_Assignment",
                "enabledRules": [
                    "MultiFactorAuthentication",
                    "Justification"
                ],
                "target": {
                    "caller": "EndUser",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
                "id": "Approval_EndUser_Assignment",
                "target": {
                    "caller": "EndUser",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                },
                "setting": {
                    "isApprovalRequired": false,
                    "isApprovalRequiredForExtension": false,
                    "isRequestorJustificationRequired": true,
                    "approvalMode": "SingleStage",
                    "approvalStages": [
                        {
                            "approvalStageTimeOutInDays": 1,
                            "isApproverJustificationRequired": true,
                            "escalationTimeInMinutes": 0,
                            "isEscalationEnabled": false,
                            "primaryApprovers": [],
                            "escalationApprovers": []
                        }
                    ]
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
                "id": "AuthenticationContext_EndUser_Assignment",
                "isEnabled": false,
                "claimValue": null,
                "target": {
                    "caller": "EndUser",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Admin_EndUser_Assignment",
                "notificationType": "Email",
                "recipientType": "Admin",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "EndUser",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Requestor_EndUser_Assignment",
                "notificationType": "Email",
                "recipientType": "Requestor",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "EndUser",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            },
            {
                "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
                "id": "Notification_Approver_EndUser_Assignment",
                "notificationType": "Email",
                "recipientType": "Approver",
                "notificationLevel": "All",
                "isDefaultRecipientsEnabled": true,
                "notificationRecipients": [],
                "target": {
                    "caller": "EndUser",
                    "operations": [
                        "all"
                    ],
                    "level": "Assignment",
                    "inheritableSettings": [],
                    "enforcedSettings": []
                }
            }
        ]
    }
}
```
