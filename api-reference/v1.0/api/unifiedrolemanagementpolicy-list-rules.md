---
title: '列出角色管理策略 (规则) '
description: 获取为角色管理策略定义的规则。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1084a5b889fcec98c74f9211705d6d6ec261c509
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204580"
---
# <a name="list-rules-for-a-role-management-policy"></a>列出角色管理策略 (规则) 
命名空间：microsoft.graph

获取为角色管理策略定义的规则。 规则是派生自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象的以下类型的集合：
+ [unifiedRoleManagementPolicyApprovalRule](../resources/unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](../resources/unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](../resources/unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](../resources/unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](../resources/unifiedrolemanagementpolicynotificationrule.md)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|RoleManagementPolicy.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagementPolicy.ReadWrite.Directory、RoleManagement.ReadWrite.Directory|
|委派（个人 Microsoft 帐户）|不支持|
|Application|RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` OData 查询参数， `$filter` 以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicies/DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448/rules
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicyrule-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyRule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies('DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448')/rules",
    "value": [
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
```

