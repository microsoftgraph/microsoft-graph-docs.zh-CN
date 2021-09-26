---
title: 教程：使用 Privileged Identity Management (PIM) API 分配 Azure AD 角色
description: 了解如何使用 Microsoft Privileged Identity Management (PIM) API Graph Azure AD 特权角色。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 9f706b6c8a39548fb65dcb46e83845b51fd9af21
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777295"
---
# <a name="tutorial-use-the-privileged-identity-management-pim-api-to-assign-azure-ad-roles"></a>教程：使用 Privileged Identity Management (PIM) API 分配 Azure AD 角色

Microsoft Graph PIM API 使组织能够管理 Azure AD Azure Active Directory (中的资源的特权) 。 它还通过限制访问处于活动状态、管理访问范围和提供特权访问的可审核日志来帮助管理特权访问的风险。

在本教程中，名为 Contoso Limited 的虚构公司希望其 IT 支持人员管理员工访问的生命周期。 该公司将 Azure AD 用户管理员角色标识为 IT 支持人员所需的相应特权角色，并将使用 PIM API 分配角色。

你将为 IT 支持人员创建可分配角色的安全组，然后使用 PIM API 将安全组资格分配给用户管理员角色。 通过向安全组分配符合条件的角色，Contoso 可以更高效地管理管理员对 Azure AD 角色等资源的访问。 例如: 

+ 删除现有或添加更多的组成员也会删除管理员。
+ 向组的成员添加更多角色，而不是向单个用户分配角色。

分配资格（而不是持久有效的用户管理员权限）允许公司强制执行实时访问，这将授予执行特权任务的临时权限。 定义角色资格后，符合条件的组成员会暂时激活其分配。 公司将审核所有角色激活记录。

>[!NOTE]
>为了可读性，本教程中显示的响应对象可能会缩短。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ Azure AD 租户（已启用Azure AD Premium P2 EMS E5 许可证）。
+ 以全局[Graph](https://developer.microsoft.com/graph/graph-explorer)用户登录资源管理器。
  + [可选]启动新的隐身或 InPrivate 浏览器会话，或在匿名浏览器中启动会话。 你将在本教程的稍后部分登录。
+ 以下委派权限 `User.ReadWrite.All` `Group.ReadWrite.All` ：、、、、 `Directory.Read.All` `RoleEligibilitySchedule.ReadWrite.Directory` `RoleAssignmentSchedule.ReadWrite.Directory` 和 `RoleManagement.ReadWrite.Directory` 。
+ Authenticator安装在手机上的应用，以注册用户以使用 MFA (多重) 。

若要同意在浏览器浏览器中Graph权限：
1. 选择用户帐户详细信息右边的水平省略号图标，然后选择选择 **权限**。
  
      :::image type="content" source="/graph/images/GE-Permissions/selectpermissions.png" alt-text="选择&quot;Microsoft Graph权限&quot;。" border="true":::

2. 滚动浏览这些权限的权限列表：
    + 将 (2) ，展开，然后选择 **Group.ReadWrite.All。**
    + Directory (4) ，展开，然后选择 **Directory.Read.All。**
    + RoleAssignmentSchedule (2) ，展开，然后选择 **RoleAssignmentSchedule.ReadWrite.Directory**。
    + RoleEligibilitySchedule (2) ，展开，然后选择 **RoleEligibilitySchedule.ReadWrite.Directory**。
    + RoleManagement (3) ，展开，然后选择 **RoleManagement.ReadWrite.Directory**。
    + 用户 (8) ，展开，然后选择 **User.ReadWrite.All。**
   
   选择“**同意**”，然后选择“**接受**”，以接受同意权限。 对于 `RoleEligibilitySchedule.ReadWrite.Directory` 和 `RoleAssignmentSchedule.ReadWrite.All` 权限，请代表你的组织同意。

      :::image type="content" source="/graph/images/GE-Permissions/User.ReadWrite.All-consent.png" alt-text="同意 Microsoft Graph权限。" border="true":::

## <a name="step-1-create-a-test-user"></a>步骤 1：创建测试用户

创建一个用户，该用户必须在首次登录时重置其密码。 在此步骤中，记录新用户 **ID** 的值，以用于下一步。 创建用户后，访问 Azure 门户，然后为用户 (MFA) 多重身份验证。 有关启用 MFA 的信息，请参阅另 [请参阅部分](#see-also) 。


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

创建可分配给 Azure AD 角色的组。 将自己分配为组所有者，同时将你和 Aline (步骤 1 中创建的用户分配为) 成员。

### <a name="request-create-a-role-assignable-group"></a>请求：创建可分配角色的组

将 `1ed8ac56-4827-4733-8f80-86adc2e67db5` 替换为 **你的 id**。

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

### <a name="request"></a>请求

将自己和 Aline 分配为安全组的两个成员。 在下面的请求中，替换：
+ `e77cbb23-0ff2-4e18-819c-690f58269752` 在 URL 中，组 ID 的值 **为**。
+ `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` 使用 Aline 的 **id 的值**。
+ `1ed8ac56-4827-4733-8f80-86adc2e67db5` 使用 id **的值**。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-addGroupMembers"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/groups/e77cbb23-0ff2-4e18-819c-690f58269752
Content-type: application/json

{
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
HTTP/1.1 204 No Content
```

## <a name="step-3-create-a-unifiedroleeligibilityschedulerequest"></a>步骤 3：创建 unifiedRoleEligibilityScheduleRequest

现在你已拥有一个安全组，请将其分配为符合用户管理员角色条件。 在此步骤中：

+ 创建 unifiedRoleEligibilityScheduleRequest 对象，该对象将 **组 IT** (User) 标识为有资格担任用户管理员角色一年。 Azure AD 可将此符合条件的分配扩展到组的成员，即你和 Aline。
+ 将符合条件的分配范围确定到整个租户。 这允许用户管理员针对租户中的所有用户使用其权限，但具有更高权限的用户（如全局管理员）除外。

### <a name="request"></a>请求

将 `e77cbb23-0ff2-4e18-819c-690f58269752` 替换为"用户安全组" **的** IT (**id)** 的值。 此 **principalId** 标识具有用户管理员角色资格的接受者。 roleDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` 是 Azure AD 中用户管理员角色的全局模板标识符。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-unifiedRoleEligibilityScheduleRequest_create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
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

## <a name="step-4-confirm-the-users-current-role-assignments"></a>步骤 4：确认用户的当前角色分配

虽然这些组的成员现在有资格担任用户管理员角色，但他们仍然无法使用该角色。 这是因为他们尚未激活其资格。 您可以通过检查用户的当前角色分配来确认。


### <a name="request"></a>请求

在下面的请求中， `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` 将 替换为 Aline 的 **id 的值**。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignments_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=principalId eq '7146daa8-1b4b-4a66-b2f7-cf593d03c8d2'
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": []
}
```

空响应对象显示 Aline 在 Contoso 中没有现有的 Azure AD 角色。 现在，Aline 将在有限时间内激活其符合条件的用户管理员角色。

## <a name="step-5-user-self-activates-their-eligible-assignment"></a>步骤 5：用户自行激活其符合条件的分配

事件票证 CONTOSO：Contoso 的事件管理系统中引发了 Security-012345，公司要求使员工的刷新令牌失效。 作为 IT 支持人员的成员，Aline 负责完成此任务。

首先，在Authenticator启动应用，然后打开 Aline Dupuy 的帐户。

Sign in to Graph Explorer as Aline. 对于此步骤，可以使用隐身会话或匿名浏览器。 这样，你就不会以全局管理员角色的用户角色中断当前会话。 或者，你可以中断当前会话，Graph资源管理器并作为 Aline 重新登录。

以 Aline 登录后，你将首先更改密码，因为这是在帐户创建期间指定的。 然后，由于管理员为 MFA 配置了您的帐户，系统将提示你在 Authenticator 应用中设置帐户，并提示你进行 MFA 登录。 这是因为 PIM 要求所有活动角色分配都使用 MFA。

登录后，激活用户管理员角色五个小时。

### <a name="request"></a>请求

若要激活角色，请调用 `roleAssignmentScheduleRequests` 终结点。 在此请求中 `UserActivate` ，此操作允许您激活符合条件的工作分配（本例中为 5 小时）。

+ 对于 **principalId**，提供 Aline (id 的) **值**。
+ **roleDefinitionId** 是有资格使用的角色的 **ID，** 在这种情况下，是用户管理员角色。
+ 输入提供激活请求的可审核理由的票证系统的详细信息。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleAssignmentScheduleRequests_selfActivate"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignmentScheduleRequests/$entity",
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

你可以运行 来确认分配 `GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentScheduleRequests/filterByCurrentUser(on='principal')` 。 响应对象返回新激活角色分配，其状态设置为 `Granted` 。 使用新权限，在工作分配活动五小时内执行任何允许的操作。 这包括使所有员工的刷新令牌失效。 五小时后，活动分配将过期，但通过 IT (**Users)** 组的成员身份，您仍有资格担任用户管理员角色。

返回到全局管理员会话，你已收到符合条件的分配和角色激活的通知。 这使全局管理员能够了解整个组织对管理员权限的所有提升。

## <a name="step-6-clean-up-resources"></a>步骤 6：清理资源

以全局管理员登录并删除为本教程创建的以下资源：角色资格请求、IT 支持 (Users) 组和测试用户 (Aline Dupuy) 。

### <a name="revoke-the-role-eligibility-request"></a>撤销角色资格请求

#### <a name="request"></a>请求

将 `e77cbb23-0ff2-4e18-819c-690f58269752` 替换为 **"用户** "组 (IT) ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-roleEligibilityScheduleRequests_revoke"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleEligibilityScheduleRequests/$entity",
    "id": "dcd11a1c-300f-4d17-8c7a-523830400ec8",
    "status": "Revoked",
    "action": "AdminRemove",
    "principalId": "e77cbb23-0ff2-4e18-819c-690f58269752",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "directoryScopeId": "/"
}
```

### <a name="delete-the-it-support-users-group"></a>Delete the IT Support (Users) group

#### <a name="request"></a>请求

将 `e77cbb23-0ff2-4e18-819c-690f58269752` 替换为 **"用户** "组 (IT) ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-group_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/groups/e77cbb23-0ff2-4e18-819c-690f58269752
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

将 `7146daa8-1b4b-4a66-b2f7-cf593d03c8d2` 替换为 Aline 的 **id 的值**。

<!-- {
  "blockType": "request",
  "name": "tutorial-assignaadroles-user_delete"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2
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

+ [开始使用Privileged Identity Management](/azure/active-directory/privileged-identity-management/pim-getting-started)
+ [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference#all-roles)
+ [启用每用户 Azure AD 多重身份验证，以确保登录事件的安全](/azure/active-directory/authentication/howto-mfa-userstates)
+ [unifiedRoleEligibilityScheduleRequest 资源类型](/graph/api/resources/unifiedroleeligibilityschedulerequest?view=graph-rest-beta&preserve-view=true)