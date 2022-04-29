---
title: 列出 roleManagementPolicyAssignments
description: 获取所有角色管理策略分配的详细信息。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 459f5ae00317e521d3d3643a7f4347eb5ce69dac
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134074"
---
# <a name="list-rolemanagementpolicyassignments"></a>列出 roleManagementPolicyAssignments
命名空间：microsoft.graph

获取所有角色管理策略分配的详细信息。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleManagementPolicy.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagementPolicy.ReadWrite.Directory、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|RoleManagement.Read.All、RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments?$filter=scopeId eq 'scopeId' and scopeType eq 'scopeType'
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法要求 `$filter` (`eq`) 查询参数将请求的范围限定到 **scopeId** 和 **scopeType**。 还可以按 **roleDefinitionId** 进行筛选，或使用 `$select` OData `$expand` 查询参数帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="example-1-retrieve-the-role-management-policy-assignments"></a>示例 1：检索角色管理策略分配

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyassignment"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicyAssignments?$filter=scopeId eq '/' and scopeType eq 'Directory'
```


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicyAssignments",
    "value": [
        {
            "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10",
            "policyId": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "scopeId": "/",
            "scopeType": "Directory",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_23b16f1a-1f8d-4891-93b1-21244cdf6115_2af84b1e-32c8-42b7-82bc-daa82404023b",
            "policyId": "Directory_cab01047-8ad9-4792-8e42-569340767f1b_23b16f1a-1f8d-4891-93b1-21244cdf6115",
            "scopeId": "/",
            "scopeType": "Directory",
            "roleDefinitionId": "2af84b1e-32c8-42b7-82bc-daa82404023b"
        }
    ]
}
```


### <a name="example-2-retrieve-the-role-management-policy-assignments-for-an-azure-ad-role-and-expand-the-policy-and-its-associated-rules"></a>示例 2：检索Azure AD角色的角色管理策略分配，并展开策略及其关联的规则

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyassignment_expand_all_relationships"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicyAssignments?$filter=scopeId eq '/' and scopeType eq 'DirectoryRole' and roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=policy($expand=rules)
```


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicyAssignments(policy(rules()))",
    "value": [
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10",
            "policyId": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "policy": {
                "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
                "displayName": "DirectoryRole",
                "description": "DirectoryRole",
                "isOrganizationDefault": false,
                "scopeId": "/",
                "scopeType": "DirectoryRole",
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
    ]
}
```