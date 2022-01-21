---
title: 教程：使用 Microsoft Graph API 识别和修正风险
description: 了解如何使用 Microsoft Graph API 识别和修正风险。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4402c6d2873f1405199a0c32701c5d48526bb4d5
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161744"
---
# <a name="tutorial-identify-and-remediate-risks-using-microsoft-graph-apis"></a>教程：使用 Microsoft Graph API 识别和修正风险

Azure AD Identity Protection 使组织能够深入了解基于标识的风险以及调查和自动修正风险的不同方法。 本教程中使用的 Identity Protection API 可以帮助您识别风险，并配置工作流以确认泄露或启用修正。 有关详细信息，请参阅 [什么是风险？](/azure/active-directory/identity-protection/concept-identity-protection-risks)

在本教程中，你将了解如何生成有风险的登录，以及使用要求多重身份验证和 MFA 身份验证的条件访问策略修正用户 (状态) 。 可选部分展示了如何阻止用户也使用条件访问策略登录，并消除用户风险。

>**注意：** 为了可读性，本教程中显示的响应对象可能会缩短。 

## <a name="prerequisites"></a>先决条件

若要成功完成本教程，请确保满足以下先决条件：

- 你必须拥有一个Azure AD Premium P1 P2 许可证才能使用风险检测 API。
- 本教程使用 Tor 浏览器匿名登录 Azure 门户。 可以使用任何匿名浏览器来完成该任务。 若要下载 Tor 浏览器，请参阅 [下载 Tor 浏览器](https://www.torproject.org/download/)。
- 本教程的前提是使用 Microsoft Graph Explorer，但是可以使用 Postman，也可以创建自己的客户端应用程序来调用 Microsoft Graph。 如果要在本教程中调用 Microsoft Graph API，需要使用具有全局管理员角色和适当权限的帐户。 完成以下步骤以在 Microsoft Graph Explorer 中设置权限：
    1. 启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。
    2. 选择“**使用 Microsoft 登录**”，然后使用 Azure AD 全局管理员账户登录。 成功登录后，可在左侧窗格中看到用户帐户详细信息。
    3. 选择用户帐户详细信息右侧的设置图标，然后选择“**权限**”。

        ![设置权限](./images/tutorial-riskdetection-api/set-permissions.png)
        
    4. 滚动浏览这些权限的权限列表：
        - **IdentityRiskEvents (2) ，** 展开，然后选择 `IdentityRiskEvent.Read.All`
        - **IdentityRiskyUser (2) ，** 展开并选择 `IdentityRiskyUser.ReadWrite.All`
        - **策略 (13) ，** 展开，然后选择 `Policy.Read.All``Policy.ReadWrite.ConditionalAccess`
        - **用户 (8) ，** 展开并选择 `User.ReadWrite.All`
        
        ![搜索权限](./images/tutorial-riskdetection-api/permissions-consent.png)
    
    5. 选择“**同意**”，然后选择“**接受**”，以接受同意权限。 你不需要代表组织同意这些权限。

        ![接受权限](./images/tutorial-riskdetection-api/accept-permissions.png)

## <a name="step-1-create-a-user-account"></a>步骤 1：创建用户帐户

对于本教程，你将创建用于测试风险检测的用户帐户。 在请求正文中， `contoso.com` 更改为租户的域名。 可在 Azure Active Directory 概述页面上找到租户信息。

### <a name="request"></a>请求

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

## <a name="step-2-trigger-a-risk-detection"></a>步骤 2：触发风险检测

### <a name="trigger-a-risk-detection"></a>触发风险检测

触发用户帐户风险检测的一种方式是匿名登录 Azure 门户。 在本教程中，Tor 浏览器用于匿名登录。 

1. 打开浏览器并输入 `portal.azure.com` 站点地址。
2. 使用之前创建的 **MyTestUser1** 帐户的凭据登录门户。 将要求您更改现有密码。

### <a name="list-risk-detections"></a>列出风险检测

使用匿名浏览器登录 Azure 门户时， `anonymizedIPAddress` 检测到风险事件。 查询参数可用于 `$filter` 仅获取与 **MyTestUser1** 用户帐户关联的风险检测。

#### <a name="request"></a>请求

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#riskDetections",
  "value": [
    {
      "id": "d52a631815aaa527bf642b196715da5cf0f35b6879204ea5b5c99b21bd4c16f4",
      "requestId": "06f7fd18-b8f1-407d-86a3-f6cbe3a4be00",
      "correlationId": "2a38abff-5701-4073-a81e-fd3aac09cba3",
      "riskType": "anonymizedIPAddress",
      "riskEventType": "anonymizedIPAddress",
      "riskState": "atRisk",
      "riskLevel": "medium",
      "riskDetail": "none",
      "source": "IdentityProtection",
      "detectionTimingType": "realtime",
      "activity": "signin",
      "tokenIssuerType": "AzureAD",
      "ipAddress": "178.17.170.23",
      "activityDateTime": "2020-11-03T20:51:34.6245276Z",
      "detectedDateTime": "2020-11-03T20:51:34.6245276Z",
      "lastUpdatedDateTime": "2020-11-03T20:53:12.1984203Z",
      "userId": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com",
      "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
      "location": {
        "city": "Chisinau",
        "state": "Chisinau",
        "countryOrRegion": "MD",
        "geoCoordinates": {
          "latitude": 47.0269,
          "longitude": 28.8416
        }
      }
    }
  ]
}
```

> **注意：** 可能需要几分钟时间才能返回事件。

## <a name="step-3-create-a-conditional-access-policy"></a>步骤 3：创建条件访问策略

可以在组织中利用条件访问策略，以允许用户在检测到风险时进行自我修正。 利用自修正功能，用户可以在完成策略提示后取消阻止自己安全地访问其资源。 在此步骤中，将创建一个条件访问策略，要求用户在出现中等或高风险检测时使用 MFA 登录。

### <a name="set-up-multi-factor-authentication"></a>设置多重身份验证

为 MFA 设置帐户时，可以从多种方法中选择用于验证用户的方法。 选择最适合你的情况来完成本教程的方法。 

1. 使用 **MyTestUser1** [帐户](https://aka.ms/MFASetup)登录 以确保帐户安全网站。
2. 使用适用于你的情况的方法完成 MFA 设置过程，例如向手机发送短信。

### <a name="create-the-conditional-access-policy"></a>创建条件访问策略

条件访问策略提供了设置策略条件以确定登录风险级别的能力。 风险级别可以是 `low` `medium` `high` 、、、。 `none` 在从列出 **MyTestUser1** 的风险检测返回的响应中，可以看到风险级别为 `medium` 。 此示例演示如何要求被标识为风险用户的 **MyTestUser1** 进行 MFA。

#### <a name="request"></a>请求 

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies 
Content-type: application/json
 
{ 
  "displayName": "Policy for risky sign-in", 
  "state": "enabled", 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "applications": { 
      "includeApplications": ["All"]
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ] 
  } 
} 
```

#### <a name="response"></a>响应 

```
{ 
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity", 
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8", 
  "displayName": "Policy for risky sign-in", 
  "createdDateTime": "2020-11-03T20:56:38.6210843Z", 
  "modifiedDateTime": null, 
  "state": "enabled", 
  "sessionControls": null, 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "clientAppTypes": [  
      "all"  
    ], 
    "platforms": null, 
    "locations": null, 
    "applications": { 
      "includeApplications": [ 
        "All" 
      ], 
      "excludeApplications": [], 
      "includeUserActions": [] 
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ], 
      "excludeUsers": [], 
      "includeGroups": [], 
      "excludeGroups": [], 
      "includeRoles": [], 
      "excludeRoles": [] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ], 
    "customAuthenticationFactors": [], 
    "termsOfUse": [] 
  } 
} 
```

在设置此条件访问策略后，现在需要 **MyTestUser1** 帐户在登录时使用 MFA，因为登录风险级别为中或   高。 

### <a name="sign-in-and-complete-multi-factor-authentication"></a>登录并完成多重身份验证 

通过登录匿名浏览器，将检测到风险，但会通过完成 MFA 进行修正。 

1. 打开浏览器并输入  `portal.azure.com`   站点地址。 
2. 使用 **MyTestUser1** 帐户的凭据登录门户并   完成 MFA 过程。 

### <a name="list-risk-detections"></a>列出风险检测

因为 MFA 已完成。 现在，当你列出风险检测时 **，riskState** 将事件显示为 `remediated` 。

#### <a name="request"></a>请求

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>响应

```http
{
  "id": "ba9d45f16d8f87f6ae974efda7336b2120962a398cb362dfd9e5bdc8e9d149d0",
  "requestId": "156c01fb-31cf-4a10-b9a9-beee93e6a400",
  "correlationId": "a8aaac45-fe22-46df-babf-10a8dba85d62",
  "riskType": "anonymizedIPAddress",
  "riskEventType": "anonymizedIPAddress",
  "riskState": "remediated",
  "riskLevel": "medium",
  "riskDetail": "userPassedMFADrivenByRiskBasedPolicy",
  "source": "IdentityProtection",
  "detectionTimingType": "realtime",
  "activity": "signin",
  "tokenIssuerType": "AzureAD",
  "ipAddress": "185.220.101.213",
  "activityDateTime": "2020-11-12T23:45:22.4092789Z",
  "detectedDateTime": "2020-11-12T23:45:22.4092789Z",
  "lastUpdatedDateTime": "2020-11-12T23:47:57.7831423Z",
  "userId": "4b608561-9258-44ba-8cdb-3286dcbf0e3b",
  "userDisplayName": "MyTestUser1",
  "userPrincipalName": "MyTestUser1@contoso.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
  "location": {
    "city": "Schoenwalde-Glien",
    "state": "Brandenburg",
    "countryOrRegion": "DE",
    "geoCoordinates": {
      "latitude": 52.61983,
      "longitude": 13.12743
    }
  }
}
```

## <a name="step-4-optional-block-the-user-from-signing-in"></a>步骤 4 (可选) 阻止用户登录

你可以阻止用户登录，而不是为用户提供自行修正的机会。 在此步骤中，您将创建一个新的条件访问策略，在出现中等或高风险检测时阻止用户登录。 策略中的区别在于 **，builtInControls** 设置为 `block` 。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
  "displayName": "Policy for risky sign-in block access",
  "state": "enabled",
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "applications": {
      "includeApplications": ["All"]
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ]
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ]
  }
}
```

### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity",
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8",
  "displayName": "Policy for risky sign-in block access",
  "createdDateTime": "2020-11-03T20:56:38.6210843Z",
  "modifiedDateTime": null,
  "state": "enabled",
  "sessionControls": null,
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "clientAppTypes": [ 
      "all" 
    ],
    "platforms": null,
    "locations": null,
    "applications": {
      "includeApplications": [
        "All"
      ],
      "excludeApplications": [],
      "includeUserActions": []
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ],
      "excludeUsers": [],
      "includeGroups": [],
      "excludeGroups": [],
      "includeRoles": [],
      "excludeRoles": []
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ],
    "customAuthenticationFactors": [],
    "termsOfUse": []
  }
}
```

在设置此条件访问策略后 **，MyTestUser1** 帐户现在被阻止登录，因为登录风险级别是 `medium` 或 `high` 。

![阻止登录](./images/tutorial-riskdetection-api/conditionalaccess-policy.png)

## <a name="step-5-dismiss-risky-users"></a>步骤 5：消除有风险的用户

如果您认为用户没有风险，并且不希望强制执行条件访问策略，您可以手动消除存在风险的用户。

### <a name="dismiss-the-risky-user"></a>消除有风险的用户

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "4628e7df-dff3-407c-a08f-75f08c0806dc"
  ]
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204 No Content
```        

### <a name="list-risky-users"></a>列出有风险的用户

消除风险用户后，在列出存在风险的用户时，可以在响应中看到 **MyTestUser1** 用户帐户现在的风险级别为 `none` ，riskState 为 `dismissed` 。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "isDeleted": false,
      "isProcessing": false,
      "riskLevel": "none",
      "riskState": "dismissed",
      "riskDetail": "adminDismissedAllRiskForUser",
      "riskLastUpdatedDateTime": "2020-11-03T21:48:53.4298425Z",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com"
    }
  ]
}
```

## <a name="step-6-clean-up-resources"></a>步骤 6：清理资源

在此步骤中，将删除创建的资源。

### <a name="delete-the-user-account"></a>删除用户账户

删除 **MyTestUser1** 用户帐户。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/users/4628e7df-dff3-407c-a08f-75f08c0806dc
```

#### <a name="response"></a>响应

```http
No Content - 204
```

### <a name="delete-the-conditional-access-policy"></a>删除条件访问策略

删除创建的条件访问策略。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/groups/9ad78153-b1f8-4714-adc1-1445727678a8
```

#### <a name="response"></a>响应

```http
No Content - 204
```

## <a name="see-also"></a>另请参阅

在本教程中，你使用了许多 API 来完成任务。 浏览这些 API 的 API 参考，详细了解 API 可以执行哪些操作。

- [什么是标识保护？](/azure/active-directory/identity-protection/overview-identity-protection)
- [什么是条件访问？](/azure/active-directory/conditional-access/overview)
- [工作原理：Azure 多重身份验证](/azure/active-directory/authentication/concept-mfa-howitworks)
- [在 Identity Protection 中模拟风险检测](/azure/active-directory/identity-protection/howto-identity-protection-simulate-risk)
- [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy)
- [riskDetection](/graph/api/resources/riskdetection)
- [riskyUser](/graph/api/resources/riskyuser)
- [用户](/graph/api/resources/user)
