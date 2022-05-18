---
title: 教程：使用 Privileged Identity Management (PIM) API 分配 Azure AD 角色
description: 了解如何在 Microsoft Graph中使用 Privileged Identity Management (PIM) API 来分配 Azure AD 特权角色。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 0f15636c80b72ba67f56a28d4352236fa4c0e19e
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461210"
---
# <a name="tutorial-use-the-privileged-identity-management-pim-api-to-assign-azure-ad-roles"></a>教程：使用 Privileged Identity Management (PIM) API 分配 Azure AD 角色

Microsoft Graph PIM API 使组织能够管理对 Azure Active Directory (Azure AD) 中的资源的特权访问。 它还通过限制访问处于活动状态、管理访问范围以及提供可审核的特权访问日志来帮助管理特权访问的风险。

在本教程中，一家名为 Contoso Limited 的虚构公司希望其 IT 支持人员管理员工访问的生命周期。 公司已将 Azure AD 用户管理员角色确定为 IT 支持人员所需的适当特权角色，并将使用 PIM API 分配该角色。

你将为 IT 支持人员创建一个可分配角色的安全组，并使用 PIM API 将安全组资格分配给用户管理员角色。 通过将符合条件的角色分配给安全组，Contoso 可以更高效地管理管理员对 Azure AD 角色等资源的访问权限。 例如：

+ 删除现有或添加更多组成员也会删除管理员。
+ 向组成员添加更多角色，而不是将角色分配给单个用户。

分配资格而非永久活动用户管理员权限允许公司强制实施 **实时访问**，从而授予执行特权任务的临时权限。 定义角色资格后，符合条件的组成员将激活其分配的临时期限。 所有角色激活记录将由公司审核。

>[!NOTE]
>本教程中显示的响应对象可能会缩短以实现可读性。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ 已启用Azure AD Premium P2或 EMS E5 许可证的工作 Azure AD 租户。
+ 以全局管理员角色的用户身份登录[到Graph资源管理器](https://developer.microsoft.com/graph/graph-explorer)。
  + [可选]"开始"菜单新的隐身或 InPrivate 浏览器会话，或在匿名浏览器中启动会话。 本教程稍后将登录。
+ 以下委派权限：`User.ReadWrite.All`、`Group.ReadWrite.All`、`Directory.Read.All`、`RoleEligibilitySchedule.ReadWrite.Directory`和 `RoleAssignmentSchedule.ReadWrite.Directory``RoleManagement.ReadWrite.Directory`。
+ Authenticator安装在手机上的应用，以注册用户进行多重身份验证 (MFA) 。

若要在Graph资源管理器中同意所需的权限，请执行以下操作：
1. 选择用户帐户详细信息右侧的水平省略号图标，然后选择 **“选择权限**”。
  
      :::image type="content" source="/graph/images/GE-Permissions/selectpermissions.png" alt-text="选择 Microsoft Graph权限。" border="true":::

2. 滚动浏览这些权限的权限列表：
    + 组 (2) ，展开，然后选择 **Group.ReadWrite.All**。
    + 目录 (4) ，展开，然后选择 **Directory.Read.All**。
    + RoleAssignmentSchedule (2) ，展开并选择 **RoleAssignmentSchedule.ReadWrite.Directory**。
    + RoleEligibilitySchedule (2) ，展开并选择 **RoleEligibilitySchedule.ReadWrite.Directory**。
    + RoleManagement (3) ，展开并选择 **RoleManagement.ReadWrite.Directory**。
    + 用户 (8) ，展开并选择 **User.ReadWrite.All**。
   
   选择“**同意**”，然后选择“**接受**”，以接受同意权限。 对于权 `RoleEligibilitySchedule.ReadWrite.Directory` 限和 `RoleAssignmentSchedule.ReadWrite.All` 权限，请代表你的组织同意。

      :::image type="content" source="/graph/images/GE-Permissions/User.ReadWrite.All-consent.png" alt-text="同意 Microsoft Graph权限。" border="true":::

## <a name="step-1-create-a-test-user"></a>步骤 1：创建测试用户

创建必须在第一次登录时重置其密码的用户。 在此步骤中，记录要在下一步中使用的新用户 **ID** 的值。 创建用户后，请访问Azure 门户并为用户启用多重身份验证 (MFA) 。 有关启用 MFA 的详细信息，请 [参阅“另请参阅](#see-also) ”部分。


### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-createUser"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@Contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/29a4f813-9274-4e1b-858d-0afa98ae66d4/directoryObjects/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2/Microsoft.DirectoryServices.User",
    "id": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@Contoso.com"
}
```

## <a name="step-2-create-a-security-group-that-can-be-assigned-an-azure-ad-role"></a>步骤 2：创建可分配 Azure AD 角色的安全组

创建可分配给 Azure AD 角色的组。 将自己分配为组所有者，你和 Aline (在步骤 1 中创建的用户) 作为成员。

### <a name="request-create-a-role-assignable-group"></a>请求：创建可分配角色的组

替换 `1ed8ac56-4827-4733-8f80-86adc2e67db5` 为 ID 和 `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` Aline ID 的值。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-createSecurityGroup"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
    "description": "IT Helpdesk to support Contoso employees",
    "displayName": "IT Helpdesk (User)",
    "mailEnabled": false,
    "mailNickname": "userHelpdesk",
    "securityEnabled": true,
    "isAssignableToRole": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5",
        "https://graph.microsoft.com/v1.0/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2"
    ]
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/29a4f813-9274-4e1b-858d-0afa98ae66d4/directoryObjects/e77cbb23-0ff2-4e18-819c-690f58269752/Microsoft.DirectoryServices.Group",
    "id": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "description": "IT Helpdesk to support Contoso employees",
    "displayName": "IT Helpdesk (User)",
    "groupTypes": [],
    "isAssignableToRole": true,
    "mailEnabled": false,
    "mailNickname": "userHelpdesk",
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-3883711267-1310199794-258579585-1385637464",
    "visibility": "Private",
    "onPremisesProvisioningErrors": []
}
```

## <a name="step-3-create-a-unifiedroleeligibilityschedulerequest"></a>步骤 3：创建 unifiedRoleEligibilityScheduleRequest

现在你有一个安全组，将其分配为符合用户管理员角色的条件。 在此步骤中：

+ 创建一个 unifiedRoleEligibilityScheduleRequest 对象，该对象将组 **IT 支持人员 (用户)** 标识为符合用户管理员角色一年的条件。 Azure AD 将此符合条件的分配扩展到组成员，即你和 Aline。
+ 将符合条件的分配范围限定到整个租户。 这允许用户管理员对租户中的所有用户使用其特权，但更高特权用户（如全局管理员）除外。

### <a name="request"></a>请求

替换`e77cbb23-0ff2-4e18-819c-690f58269752`为 **IT 支持人员 (用户)** 安全组的 **ID** 值。 此 **principalId** 标识用户管理员角色的资格分配者。 roleDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` 是 Azure AD 中用户管理员角色的全局模板标识符。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-unifiedRoleEligibilityScheduleRequest_create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
Content-type: application/json

{
    "action": "AdminAssign",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "scheduleInfo": {
        "startDateTime": "2021-07-01T00:00:00Z",
        "expiration": {
            "endDateTime": "2022-06-30T00:00:00Z",
            "type": "AfterDateTime"
        }
    }
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleRequests"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "64a8bd54-4591-4f6a-9c77-3e9cb1fdd29b",
    "status": "Provisioned",
    "createdDateTime": "2021-09-03T20:45:28.3848182Z",
    "completedDateTime": "2021-09-03T20:45:39.1194292Z",
    "action": "AdminAssign",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "isValidationOnly": false,
    "targetScheduleId": "64a8bd54-4591-4f6a-9c77-3e9cb1fdd29b",
    "justification": "Assign User Admin eligibility to IT Helpdesk (User) group",
    "createdBy": {
        "user": {
            "id": "1ed8ac56-4827-4733-8f80-86adc2e67db5"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-09-03T20:45:39.1194292Z",
        "expiration": {
            "type": "afterDateTime",
            "endDateTime": "2022-06-30T00:00:00Z"
        }
    },
    "ticketInfo": {}
}
```

## <a name="step-4-confirm-the-users-current-role-assignments"></a>步骤 4：确认用户当前的角色分配

虽然组成员现在有资格担任用户管理员角色，但仍无法使用该角色。 这是因为他们尚未激活其资格。 可以通过检查用户当前的角色分配来确认。


### <a name="request"></a>请求

在以下请求中，替换 `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` 为 Aline **ID 的** 值。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignments_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignments?$filter=principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignments"
} -->
```
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignments",
    "value": []
}
```

空响应对象显示 Aline 在 Contoso 中没有现有的 Azure AD 角色。 Aline 现在会在有限的时间内激活其符合条件的用户管理员角色。

## <a name="step-5-user-self-activates-their-eligible-assignment"></a>步骤 5：用户自行激活其符合条件的分配

ConTOSO 事件票证：Contoso 的事件管理系统中已提高安全性-012345，公司要求所有员工的刷新令牌都失效。 作为 IT 支持人员的成员，Aline 负责完成此任务。

首先，在手机上启动Authenticator应用并打开 Aline Dupuy 的帐户。

以 Aline 身份登录到Graph资源管理器。 可以为此步骤使用隐身会话或匿名浏览器。 这样，你就不会中断当前会话作为全局管理员角色中的用户。 或者，可以通过注销Graph资源管理器并以 Aline 身份重新登录来中断当前会话。

以 Aline 身份登录时，将首先更改密码，因为这是在创建帐户期间指定的。 然后，由于管理员为 MFA 配置了帐户，系统会提示你在Authenticator应用中设置帐户，并针对 MFA 登录提出质询。 这是因为 PIM 需要所有活动角色分配的 MFA。

登录后，激活用户管理员角色 5 小时。

### <a name="request"></a>请求

若要激活角色，请调用 `roleAssignmentScheduleRequests` 终结点。 在此请求中 `UserActivate` ，此操作允许你激活符合条件的分配（在此示例中为 5 小时）。

+ 对于 **principalId**，请提供 (Aline) **ID** 的值。
+ **roleDefinitionId** 是你有资格在本例中使用用户管理员角色的角色的 **ID**。
+ 输入票证系统的详细信息，该系统提供激活请求的可审核理由。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignmentScheduleRequests_selfActivate"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests
Content-type: application/json

{
    "action": "SelfActivate",
    "principalId": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "justification": "Need to invalidate all app refresh tokens for Contoso users.",
    "scheduleInfo": {
        "startDateTime": "2021-09-04T15:13:00.000Z",
        "expiration": {
            "type": "AfterDuration",
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Security-012345",
        "ticketSystem": "Contoso ICM"
    }
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleEligibilityScheduleRequests"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
    "id": "295edd40-4646-40ca-89b8-ab0b46b6f60e",
    "status": "Granted",
    "createdDateTime": "2021-09-03T21:10:49.6670479Z",
    "completedDateTime": "2021-09-04T15:13:00Z",
    "action": "SelfActivate",
    "principalId": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/",
    "isValidationOnly": false,
    "targetScheduleId": "295edd40-4646-40ca-89b8-ab0b46b6f60e",
    "justification": "Need to invalidate all app refresh tokens for Contoso users.",
    "createdBy": {
        "user": {
            "id": "7146daa8-1b4b-4a66-b2f7-cf593d03c8d2"
        }
    },
    "scheduleInfo": {
        "startDateTime": "2021-09-04T15:13:00Z",
        "expiration": {
            "type": "afterDuration",
            "endDateTime": null,
            "duration": "PT5H"
        }
    },
    "ticketInfo": {
        "ticketNumber": "CONTOSO:Security-012345",
        "ticketSystem": "Contoso ICM"
    }
}
```

可以通过运行 `GET https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='principal')`来确认分配。 响应对象返回新激活的角色分配，其状态设置为 `Granted`。 使用新权限，在工作分配处于活动状态的五小时内执行任何允许的操作。 这包括使所有员工的刷新令牌失效。 五小时后，活动分配将过期，但通过 **IT 支持 (用户)** 组的成员身份，你仍有资格担任用户管理员角色。

回到全局管理员会话中，你已收到符合条件的分配和角色激活的通知。 这样，全局管理员便可以了解组织中管理员权限的所有提升。

## <a name="step-6-clean-up-resources"></a>步骤 6：清理资源

以全局管理员身份登录并删除为本教程创建的以下资源：角色资格请求、IT 支持 (用户) 组，以及测试用户 (Aline Dupuy) 。

### <a name="revoke-the-role-eligibility-request"></a>撤销角色资格请求

#### <a name="request"></a>请求

替换 `e77cbb23-0ff2-4e18-819c-690f58269752` 为 IT 支持 (用户) 组的 **ID** 。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleEligibilityScheduleRequests_revoke"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/roleManagement/directory/roleEligibilityScheduleRequests
Content-type: application/json

{
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}

```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roleEligibilityScheduleRequests"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "dcd11a1c-300f-4d17-8c7a-523830400ec8",
    "status": "Revoked",
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}
```

### <a name="delete-the-it-support-users-group"></a>删除 IT 支持 (用户) 组

#### <a name="request"></a>请求

替换 `e77cbb23-0ff2-4e18-819c-690f58269752` 为 IT 支持 (用户) 组的 **ID** 。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-group_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/groups/e77cbb23-0ff2-4e18-819c-690f58269752
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-test-user"></a>删除测试用户

#### <a name="request"></a>请求

替换 `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` 为 Aline **ID 的值**。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-user_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>另请参阅

+ [教程：使用 Microsoft Graph PowerShell 在Privileged Identity Management中分配 Azure AD 角色](/powershell/microsoftgraph/tutorial-pim)
+ [通过 PIM 管理角色的概述](/graph/api/resources/privilegedidentitymanagementv3-overview)