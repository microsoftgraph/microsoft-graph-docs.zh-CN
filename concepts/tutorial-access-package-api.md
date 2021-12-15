---
title: 教程：使用 Microsoft Graph API 管理对 Active Directory 授权管理中的资源的访问权限
description: 了解如何使用 Microsoft (Azure AD) API 管理对 Active Directory Graph的访问权限。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 461d3ed9bdbc7fa09f84514abe222cabf8519bcd
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526007"
---
# <a name="tutorial-manage-access-to-resources-in-active-directory-entitlement-management-using-microsoft-graph-apis"></a>教程：使用 Microsoft Graph API 管理对 Active Directory 授权管理中的资源的访问权限

管理对员工需要的所有资源（如组、应用程序和网站）的访问权限是组织的一项重要功能。 您希望向员工授予高效工作所需的正确级别的访问权限，并删除不再需要的访问权限。 [Azure Active Directory (Azure AD) Microsoft](/azure/active-directory/governance/entitlement-management-overview) Graph API 进行权利管理，可管理这种类型的访问。

本教程要求你开发代码，为内部用户可以自助请求的营销活动创建一个资源包。 请求不需要审批，用户的访问权限将在 30 天后过期。 对于本教程，市场营销活动资源只是单个组的成员身份，但它可能是组、应用程序或 SharePoint Online 网站的集合。

>**注意：** 为了可读性，本教程中显示的响应对象可能会缩短。 

## <a name="prerequisites"></a>先决条件

若要成功完成本教程，请确保满足以下先决条件：
- Azure AD权限管理需要特定许可证。 有关详细信息，请参阅许可证 [要求](/azure/active-directory/governance/entitlement-management-overview#license-requirements)。 租户中需要以下许可证：
    - Azure AD Premium P2
    - 企业移动性 + 安全性 (EMS) E5 许可证
- 本教程的前提是使用 Microsoft Graph Explorer，但是可以使用 Postman，也可以创建自己的客户端应用程序来调用 Microsoft Graph。 如果要在本教程中调用 Microsoft Graph API，需要使用具有全局管理员角色和适当权限的帐户。 对于本教程，需要 、 和 `User.ReadWrite.All` `Group.ReadWrite.All` `EntitlementManagement.ReadWrite.All` 委派权限。 完成以下步骤以在 Microsoft Graph Explorer 中设置权限：
    1. 启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。
    2. 选择“**使用 Microsoft 登录**”，然后使用 Azure AD 全局管理员账户登录。 成功登录后，可在左侧窗格中看到用户帐户详细信息。
    3. 选择用户帐户详细信息右侧的设置图标，然后选择“**权限**”。

        ![选择 Microsoft Graph 权限](./images/tutorial-access-package-api/set-permissions.png)
        
    4. 滚动浏览权限列表，展开组 (`Group` **2) ，** 选择 **Group.ReadWrite.All** 权限。 进一步向下滚动权限列表，展开"用户 (8) "，然后选择 `User` **User.ReadWrite.All** 权限。 ****

        ![搜索用户、组和权利管理权限](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. 选择“**同意**”，然后选择“**接受**”，以接受同意权限。 你不需要代表组织同意这些权限。
    6. 搜索权限，展开 `EntitlementManagement` **EntitlementManagement (2) ，** 选择 **Entitlement.ReadWrite.All** 权限，然后选择同意 。  由于此权限需要管理员同意，并且你需要在本教程创建的用户帐户使用，因此你必须选择"代表 **你的组织同意"。**

        ![组织同意](./images/tutorial-access-package-api/consent-for-organization.png)

    7. 选择 **"** 接受"接受权限的同意。

## <a name="step-1-create-a-user-account-and-a-group"></a>步骤 1：创建用户帐户和组

在此步骤中，您将在目录中创建一个名为 **"** 市场营销资源"的组，该组是权利管理的目标资源。 您还可以创建一个设置为内部请求者的帐户。

### <a name="create-a-user-account"></a>创建用户账户

对于本教程，你将创建一个用户帐户，该帐户用于请求访问访问包中的资源。 进行这些调用时，请 `contoso.onmicrosoft.com` 更改为租户的域名。 可在 Azure Active Directory 概述页面上找到租户信息。 记录返回的 **id** 属性的值，以在本教程的稍后部分使用。

#### <a name="request"></a>请求

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"Requestor1",
  "mailNickname":"Requestor1",
  "userPrincipalName":"Requestor1@contoso.onmicrosoft.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
  "deletedDateTime": null,
  "accountEnabled": true,
  "ageGroup": null,
  "businessPhones": [],
  "city": null,
  "createdDateTime": null,
  "creationType": null,
  "companyName": null,
  "consentProvidedForMinor": null,
  "country": null,
  "department": null,
  "displayName": "Requestor1",
  "employeeId": null,
  "faxNumber": null,
  "givenName": null,
  "imAddresses": [],
  "infoCatalogs": [],
  "isResourceAccount": null,
  "jobTitle": null,
  "legalAgeGroupClassification": null,
  "mail": null,
  "mailNickname": "Requestor1",
}
```

### <a name="create-a-group"></a>创建群组

在本教程中，你将创建一个名为 **"市场营销** 资源"的组，该组是权利管理的目标资源。 如果已有一个组，可以使用现有组。 记录返回的 **id** 属性的值，以在本教程的稍后部分使用。 

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
  "description":"Marketing group",
  "displayName":"Marketing resources",
  "mailEnabled":false,
  "mailNickname":"markres",
  "securityEnabled":true
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
  "id": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2020-06-24T16:47:37Z",
  "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
  "description": "Marketing group",
  "displayName": "Marketing resources",
  "expirationDateTime": null,
  "groupTypes": [],
  "infoCatalogs": [],
  "isAssignableToRole": null,
  "mail": null,
  "mailEnabled": false,
  "mailNickname": "markres"
}
```

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a>步骤 2：向目录添加资源并创建访问包

访问 *包* 是团队或项目需要且受策略管理的资源捆绑包。 访问包在名为目录的容器中定义。 目录可以引用访问包中使用的资源，如组、应用程序和网站。 在此步骤中， **你将在常规** 目录中创建市场营销活动访问包。 如果您有不同的目录，请使用下一节中的名称。

### <a name="get-the-catalog-identifier"></a>获取目录标识符

若要向目录添加资源，必须先获取其标识符。 如果使用的是常规目录，请运行以下请求获取其标识符。 如果使用的是其他 calalog，将请求中的筛选器值更改为目录名称。 记录返回的 **id** 属性的值，以在本教程的稍后部分使用。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageCatalogs",
  "value": [ 
    {
      "id": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "displayName": "General",
      "description": "Built-in catalog.",
      "catalogType": "ServiceDefault",
      "catalogStatus": "Published",
      "isExternallyVisible": true,
      "createdBy": "Azure AD",
      "createdDateTime": "2020-05-30T10:58:05.363Z",
      "modifiedBy": "Azure AD",
      "modifiedDateTime": "2020-05-30T10:58:05.363Z"
    }
  ]
}
```

响应应仅包含请求中提供其名称的目录。 如果没有返回任何值，请在继续之前检查目录的名称是否正确。

### <a name="add-the-group-to-the-catalog"></a>将组添加到目录

若要将创建的组添加到目录，请提供以下属性值：
- **catalogId** -你使用的目录的 ID
- **displayName** - 组的名称
- **description** - 组的说明
- **originId** - **你创建的** 组的 ID

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
    "displayName": "Marketing resources",
    "description": "Marketing group",
    "resourceType": "AadGroup",
    "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "originSystem": "AadGroup"
  }
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "executeImmediately": false,
  "id": "44e521e0-fb6b-4d5e-a282-e7e68dc59493",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": ""
}
```

### <a name="get-catalog-resources"></a>获取目录资源

在本教程的稍后步骤中，你需要分配给目录中的组资源的 ID。 此标识符（表示作为目录中的资源的组）与 Microsoft Graph 中的组本身Graph。 这是因为目录具有的资源不会在 Microsoft Graph。

在请求中， **提供** 你使用的目录的 ID。 记录组目录资源的 **id** 属性的值。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResources",
  "value": [
    {
      "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
      "displayName": "Marketing resources",
      "description": "Marketing group",
      "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "resourceType": "Security Group",
      "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "originSystem": "AadGroup",
      "isPendingOnboarding": false,
      "addedBy": "admin@contoso.onmicrosoft.com",
      "addedOn": "2020-08-21T19:27:29.967Z"
    }
  ]
}
```

### <a name="get-resources-roles"></a>获取资源角色

访问包将用户分配给资源的角色。 组的典型角色是成员角色。 其他资源（如 SharePoint Online 网站和应用程序）可能有许多角色。 访问包中使用的组的典型角色是成员角色。 在本教程稍后将资源角色添加到访问包时，将需要成员角色。 

在请求中，使用目录 **的 ID** 和您记录的目录中组资源的 **ID** 获取 Member 资源角色的 **originId。** 记录 **originId 属性的值** ，以在本教程的稍后部分使用。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('ede67938-cda7-4127-a9ca-7c7bf86a19b7')/accessPackageResourceRoles(accessPackageResource())",
  "value": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "displayName": "Member",
      "description": null,
      "originSystem": "AadGroup",
      "originId": "Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "accessPackageResource@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/$entity",
      "accessPackageResource": {
        "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
        "displayName": "Marketing resources",
        "description": "Marketing group",
        "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "resourceType": "Security Group",
        "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "originSystem": "AadGroup",
        "isPendingOnboarding": false,
        "addedBy": "admin@contoso.onmicrosoft.com",
        "addedOn": "2020-06-26T17:13:23.723Z",
        "accessPackageResourceScopes@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/accessPackageResourceScopes",
        "accessPackageResourceScopes": []
      }
    }
  ]
}
```

如果成功，则返回一个值，该值代表该组的 Member 角色。 如果未返回任何角色，请检查 **目录和** 访问包资源的 id 值。

### <a name="create-the-access-package"></a>创建访问包

此时，您具有一个包含组资源的目录，并且知道您将使用访问包中组的成员的资源角色。 下一步是创建访问包。 获取访问包后，你可以向它添加资源角色，并创建一个策略，用于说明用户如何请求访问该资源角色。 使用之前记录的目录的 **ID** 创建访问包。 记录访问包的 **ID，** 以在本教程的稍后部分使用。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign"
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages/$entity",
  "id": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign",
  "isHidden": false,
  "isRoleScopesVisible": false,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:45:33.2042281Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:45:33.2042281Z"
}
```

### <a name="add-a-resource-role-to-the-access-package"></a>将资源角色添加到访问包

将组资源的 Member 角色添加到访问包。 在请求中，提供访问包的 **ID。** 在请求正文中，提供 accessPackageResource 的组目录资源的 **ID，** 并提供之前记录的 Member 角色的 **originId。**

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/88203d16-0e31-41d4-87b2-dd402f1435e9/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole": {
    "originId":"Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource": {
      "id":"4a1e21c5-8a76-4578-acb1-641160e076e8","resourceType":"Security Group",  
      "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
    }
  },
  "accessPackageResourceScope": {
    "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
  }
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages('88203d16-0e31-41d4-87b2-dd402f1435e9')/accessPackageResourceRoleScopes/$entity",
  "id": "e081321b-2802-4834-a6ca-6f598ce3cdf7_6dbd2209-9d14-4c76-b92b-fcb00e835fe1",
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:56:00.6320729Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:56:00.6320729Z"
}
```

访问包现在具有一个资源角色，即组成员身份。 角色分配给具有访问包的任何用户。

### <a name="create-an-access-package-policy"></a>创建访问包策略

现在，你已创建访问包并添加了资源和角色，你可以决定谁可以通过创建访问包策略来访问它。 在本教程中，你将启用你创建的 **Requestor1** 帐户，以请求访问访问包中的资源。 对于此任务，需要以下值：
- **accessPackageId** 属性值的访问包的 **id**
- **allowedRequestors** 中 **id** 属性值的 **Requestor1** **用户帐户的** id
 
**durationInDays** 属性的值使 **Requestor1** 帐户能够在最多 30 天内访问访问包中的资源。 记录返回的 **id** 属性的值，以在本教程的稍后部分使用。 

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "accessReviewSettings": null,
  "durationInDays": 30,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.singleUser",
         "isBackup": false,
         "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
         "description": "Requestor1"
       }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentPolicies/$entity",
  "id": "db440482-1210-4a60-9b55-3ac7a72f63ba",
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "canExtend": false,
  "durationInDays": 30,
  "expirationDateTime": null,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-06-29T19:47:44.7399675Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-06-29T19:47:44.7555489Z",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
      {
        "@odata.type": "#microsoft.graph.singleUser",
        "isBackup": false,
        "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
        "description": "Requestor1"
      }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

## <a name="step-3-request-access"></a>步骤 3：请求访问

在此步骤中 **，Requestor1** 用户帐户请求访问访问包中的资源。

若要请求访问包中的资源，需要提供以下值：
- **为** **targetId** 属性的值创建的 **Requestor1** 用户帐户的 id
-  **assignmentPolicyId** 属性值的分配策略 id
-  **accessPackageId** 属性值的访问包 ID

在响应中，你可以看到"已接受 **"** 状态和"已提交 **"状态**。 记录返回的 **id** 属性的值，以稍后获取请求的状态。

如果尚未这样做，请注销在 Microsoft Graph 资源管理器中使用的管理员帐户。 登录到您创建的 **Requestor1** 用户帐户。 如果密码是首次登录，将要求您更改密码。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "UserAdd",
  "accessPackageAssignment":{
     "targetId":"007d1c7e-7fa8-4e33-b678-5e437acdcddc",
     "assignmentPolicyId":"db440482-1210-4a60-9b55-3ac7a72f63ba",
     "accessPackageId":"88203d16-0e31-41d4-87b2-dd402f1435e9"
  }
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

## <a name="step-4-validate-that-access-has-been-assigned"></a>步骤 4：验证是否分配了访问权限

在此步骤中，确认 **为 Requestor1** 用户帐户分配了访问包，并且他们现在是 Marketing 资源 **组** 的成员。

注销 Requestor1 帐户，然后重新登录到管理员帐户以查看请求的状态。

### <a name="get-the-status-of-the-request"></a>获取请求的状态

使用请求 **的 id** 属性的值获取它的当前状态。 在响应中，你可以看到状态更改为"已实现 **"，** 状态更改为"已 **送达"。**

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
  "createdDateTime": "2020-06-29T20:24:24.683Z",
  "completedDate": "2020-06-29T20:24:47.937Z",
  "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": null
}
```

### <a name="get-access-package-assignments"></a>获取访问包分配

您还可以使用所创建的访问包策略的 **ID，** 以查看资源已分配给 **Requestor1** 用户帐户。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'&$expand=target,accessPackageAssignmentResourceRoles
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignments",
  "value": [
    {
      "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
      "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
      "assignmentPolicyId": "db440482-1210-4a60-9b55-3ac7a72f63ba",
      "targetId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0",
      "assignmentStatus": "Delivered",
      "assignmentState": "Delivered",
      "isExtended": false,
      "expiredDateTime": null,
      "target": {
         "id": "8586ddc8-0ff7-4c24-9c79-f192bc3566e3",
         "objectId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0"
      },
      "accessPackageAssignmentResourceRoles": [
         {
            "id": "bdb7e0a0-a927-42ab-bf30-c5b5533dc54a",
            "originSystem": "AadGroup",
            "status": "Fulfilled"
         }
      ]
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a>获取组的成员

授予请求后，可以使用为 **Marketing** 资源组记录的 **ID** 查看 **Requestor1** 用户帐户已添加到该 ID。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/groups/e93e24d1-2b65-4a6c-a1dd-654a12225487/members
```

#### <a name="response"></a>响应：

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "businessPhones": [],
      "city": null,
      "createdDateTime": "2020-06-23T18:43:24Z",
      "creationType": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "department": null,
      "displayName": "Requestor1",
      "employeeId": null,
      "faxNumber": null,
      "givenName": null,
      "imAddresses": [],
      "infoCatalogs": [],
      "isResourceAccount": null,
      "jobTitle": null,
      "legalAgeGroupClassification": null,
      "mail": null,
      "mailNickname": "Requestor1"
    }
  ]
}
```

## <a name="step-5-clean-up-resources"></a>步骤 5：清理资源

在此步骤中，将删除所做的更改并删除 **市场营销活动** 访问包。

### <a name="remove-an-access-package-assignment"></a>删除访问包分配

必须先删除对访问包的任何分配，然后才能将其删除。 使用 **之前** 记录的分配请求的 ID 将其删除。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminRemove",
  "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
  }
}
```

#### <a name="response"></a>响应

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="delete-the-access-package-assignment-policy"></a>删除访问包分配策略

使用 **之前** 记录的分配策略的 ID 将其删除。 确保首先删除所有工作分配。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a>响应

```http
No Content - 204
```

### <a name="delete-the-access-package"></a>删除访问包

使用 **之前** 录制的访问包的 ID 将其删除。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a>响应

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>删除用户账户

删除 **Requestor1** 用户帐户。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a>响应

```http
No Content - 204
```

### <a name="delete-the-group"></a>添加或删除组成员

删除 **"市场营销资源"** 组。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a>响应

```http
No Content - 204
```

## <a name="see-also"></a>另请参阅

在本教程中，你使用了许多 API 来完成任务。 浏览这些 API 的 API 参考，详细了解 API 可以执行哪些操作。


- [使用 Azure AD权限管理 API](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true)
- [accessPackageCatalog](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true)
- [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true)
- [accessPackage](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true)
- [accessPackageResourceRoleScope](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta&preserve-view=true)
- [accessPackageAssignmentPolicy](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true)
- [accessPackageAssignmentRequest](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta&preserve-view=true)
- [组](/graph/api/resources/group)
- [用户](/graph/api/resources/user?)
