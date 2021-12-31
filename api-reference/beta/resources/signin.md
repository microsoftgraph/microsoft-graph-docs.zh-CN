---
title: signIn 资源类型
doc_type: resourcePageType
description: 提供有关目录中用户或应用程序登录活动的详细信息。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
ms.openlocfilehash: 04f489275de117a4ad3ad603748035b07aebfacc
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61646929"
---
# <a name="signin-resource-type"></a>signIn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关目录中用户或应用程序登录活动的详细信息。 你必须拥有 Azure AD Premium P1 或 P2 许可证才能使用 Microsoft Graph API 下载登录日志。

登录日志的可用性受数据保留策略[Azure AD控制](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 signIn](../api/signin-list.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[获取 signIn](../api/signin-get.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appDisplayName|String|Azure 门户中显示的应用程序名称。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|appId|String|应用程序中的应用程序Azure Active Directory。 仅 `$filter` (`eq` 运算符) 。|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) 集合|由相应登录活动触发的条件访问策略列表。|
|authenticationDetails|[authenticationDetail](authenticationdetail.md) 集合|身份验证尝试的结果和有关身份验证方法的其他详细信息。|
|authenticationMethodsUsed|字符串集合|使用的身份验证方法。 可能的值 `SMS` `Authenticator App` `App Verification code` ：、、、、、、 `Password` `FIDO` `PTA` 或 `PHS` 。|
|authenticationProcessingDetails|[keyValue](keyvalue.md) 集合|其他身份验证处理详细信息，例如 PTA/PHS 中的代理名称或联合身份验证情况下的服务器/服务器场名称。|
|authenticationProtocol|protocolType|列出身份验证中使用的协议类型或授予类型。 可取值包括：`none`、`oAuth2`、`ropc`、`wsFederation`、`saml20`、`deviceCode`、`unknownFutureValue`。 对于使用未列出可能值的协议的身份验证，协议类型将列为 `none` 。 |
|authenticationRequirement | String | 这将保留所有登录步骤所需的最高级别的身份验证，以成功登录。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) 集合|身份验证要求的来源，例如条件访问、每用户 MFA、标识保护和安全默认值。|
|autonomousSystemNumber|Int32|自治系统 (ASN) 使用的网络的一部分。|
|clientAppUsed|String|用于登录活动的旧客户端。 例如 `Browser` `Exchange Active Sync` `Modern clients` ：、、、、、、 `IMAP` `MAPI` `SMTP` 或 `POP` 。 仅 `$filter` (`eq` 运算符) 。 |
|conditionalAccessStatus|conditionalAccessStatus| 触发的条件访问策略的状态。 可能的值 `success` `failure` ：、、 `notApplied` 或 `unknownFutureValue` 。 仅 `$filter` (`eq` 运算符) 。|
|correlationId|String|启动登录时从客户端发送的标识符。 这用于在调用支持时对相应的登录活动进行疑难解答。 仅 `$filter` (`eq` 运算符) 。|
|createdDateTime|DateTimeOffset|启动登录的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 仅 `$orderby` 支持 `$filter` (、 `eq` `le` 和 `ge` 运算符) 。|
|crossTenantAccessType|signInAccessType|描述参与者用于访问资源的跨租户访问的类型。 可取值为：`none`、`b2bCollaboration`、`b2bDirectConnect`、`microsoftSupport`、`serviceProvider`、`unknownFutureValue`。 如果登录未跨租户边界，则值为 `none` 。|
|deviceDetail|[deviceDetail](devicedetail.md)|登录发生位置的设备信息。 包括 deviceId、OS 和浏览器等信息。 仅 `$filter` (`eq` `startsWith` 浏览器和 **operatingSystem** 属性) **和** 运算符。|
|flaggedForReview|Boolean|在登录失败期间，用户可能会单击 Azure 门户中的按钮，为租户管理员标记失败事件。 如果用户单击该按钮来标记失败的登录，则此值为 `true` 。|
|homeTenantId|String|启动登录的用户的租户标识符。 在托管标识或服务主体登录中不适用。|
|homeTenantName|String|对于用户登录，用户是租户的标识符。 仅在主租户已同意允许用户Azure AD租户内容时填充。|
|id|String|表示登录活动的标识符。 继承自 [实体](entity.md)。 仅 `$filter` (`eq` 运算符) 。|
|incomingTokenType|incomingTokenType|指示向用户呈现的令牌Azure AD以验证登录中的参与者。 可能的值包括 `none`、`primaryRefreshToken`、`saml11`、`saml20`、`unknownFutureValue`。 <br><br> **注意** Azure AD还使用了未在此枚举类型中列出的令牌类型来验证参与者。 如果令牌不是列出的类型之一，则不要推断缺少令牌。 |
|ipAddress|String|发生登录的客户端的 IP 地址。 仅 `$filter` (`eq` `startsWith` 和运算符) 。|
|ipAddressFromResourceProvider|String|用户用于联系资源提供程序的 IP 地址，用于确定某些策略的条件访问合规性。 例如，当用户与用户Exchange Online时，可能会Exchange接收的 IP 地址。 此值通常是 `null` 。|
|isInteractive|Boolean|指示用户登录是否是交互式登录。 在交互式登录中，用户向用户提供身份验证Azure AD。 这些因素包括密码、MFA 挑战响应、生物识别因素或用户为应用或关联应用Azure AD QR 码。 在非交互式登录中，用户不提供身份验证因素。 相反，客户端应用使用令牌或代码来代表用户进行身份验证或访问资源。 非交互式登录通常用于客户端在对用户透明的进程中代表用户登录。|
|isTenantRestricted|Boolean|显示登录事件是否受租户Azure AD策略的限制。|
|location|[signInLocation](signinlocation.md)|发生登录的城市、省/市/县和 2 个字母的国家/地区代码。 仅 `$filter` (`eq` `startsWith` city、state 和 **countryOrRegion** 属性) 和运算符。|
|networkLocationDetails|[networkLocationDetail](networklocationdetail.md) 集合|网络位置详细信息，包括所使用的网络的类型及其名称。|
|originalRequestId|String|身份验证序列中第一个请求的请求标识符。 仅 `$filter` (`eq` 运算符) 。|
|privateLinkDetails|[privateLinkDetails](../resources/privatelinkdetails.md)|包含有关Azure AD登录事件关联的专用链接策略的信息。|
|processingTimeInMilliseconds|Int|AD STS 中的请求处理时间（以毫秒为单位）。|
|resourceDisplayName|String|用户登录的资源的名称。 仅 `$filter` (`eq` 运算符) 。|
|resourceId|String|用户登录到的资源的标识符。 仅 `$filter` (`eq` 运算符) 。|
|resourceTenantId|String|登录中引用的资源的租户标识符。|
|riskDetail|riskDetail|风险用户、登录或风险事件的特定状态背后的原因。 可能的值 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` ：、、、、、、、、 `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` 或 `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` 。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 仅 `$filter` (`eq` 运算符) 。<br> **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskEventTypes_v2|字符串集合|与登录关联的风险事件类型列表。 可能的值 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` ：、、、、、、、、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` 或 `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` 。 仅 `$filter` (`eq` `startsWith` 和运算符) 。|
|riskLevelAggregated|riskLevel|聚合的风险级别。 可能的值 `none` `low` `medium` ：、、、、 `high` `hidden` 或 `unknownFutureValue` 。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 仅 `$filter` (`eq` 运算符) 。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskLevelDuringSignIn|riskLevel|登录期间的风险级别。 可能的值 `none` `low` `medium` ：、、、、 `high` `hidden` 或 `unknownFutureValue` 。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 仅 `$filter` (`eq` 运算符) 。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskState|riskState|风险用户、登录或风险事件的风险状态。 可能的值 `none` `confirmedSafe` `remediated` ：、、、、、、 `dismissed` `atRisk` `confirmedCompromised` 或 `unknownFutureValue` 。 仅 `$filter` (`eq` 运算符) 。|
|servicePrincipalCredentialKeyId|String|服务主体用于进行身份验证的密钥凭据的唯一标识符。|
|servicePrincipalCredentialThumbprint|String|服务主体用于进行身份验证的证书的证书指纹。|
|servicePrincipalId|String|用于登录的应用程序标识符。 使用应用程序登录时将填充此字段。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|servicePrincipalName|String|用于登录的应用程序名称。 使用应用程序登录时将填充此字段。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|signInEventTypes|字符串集合|指示事件表示的登录类别。 对于用户登录，类别可以是 或 ，并且对应于登录资源上的 `interactiveUser` `nonInteractiveUser` **isInteractive** 属性的值。 对于托管标识登录，类别为 `managedIdentity` 。 对于服务主体登录，类别为 **servicePrincipal**。 可取值为：`interactiveUser`、`nonInteractiveUser`、`servicePrincipal`、`managedIdentity`、`unknownFutureValue`。 仅 `$filter` (`eq` 运算符) 。|
|signInIdentifier|String|用户提供的用于登录的标识。 它可能是 userPrincipalName，但在用户使用其他标识符登录时也会填充它。|
|signInIdentifierType|signInIdentifierType|登录标识符的类型。 可取值为：`userPrincipalName`、`phoneNumber`、`proxyAddress`、`qrCode`、`onPremisesUserPrincipalName`、`unknownFutureValue`。|
|status|[signInStatus](signinstatus.md)|登录状态。 包括登录失败时的错误代码 (错误描述) 。 仅 `$filter` (`eq` **errorCode**) 的运算符。|
|tokenIssuerName|String|标识提供程序的名称。 例如，`sts.microsoft.com`。 仅 `$filter` (`eq` 运算符) 。|
|tokenIssuerType|tokenIssuerType|标识提供程序的类型。 可能的值包括 `AzureAD`、`ADFederationServices`、`UnknownFutureValue`、`AzureADBackupAuth`。 请注意，必须使用此可变化枚举 (请求) 获取以下 `Prefer: include - unknown -enum-members` [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) `AzureADBackupAuth` ： 。|
|uniqueTokenIdentifier|String|唯一的 base64 编码请求标识符，用于在资源Azure AD兑换令牌时跟踪令牌。 |
|userAgent|String|与登录相关的用户代理信息。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|userDisplayName|String|用户的显示名称。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|userId|String|用户的标识符。 仅 `$filter` (`eq` 运算符) 。|
|userPrincipalName|String|用户的 UPN。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|userType|signInUserType|标识用户是租户中的成员还是来宾。 可取值为：`member`、`guest`、`unknownFutureValue`。|
|mfaDetail (弃) |String|此属性已弃用。|


## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.signIn",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.signIn",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "autonomousSystemNumber": "Integer",
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "crossTenantAccessType": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "flaggedForReview": "Boolean",
  "id": "String (identifier)",
  "homeTenantId": "String",
  "homeTenantName": "String",
  "isInteractive": "Boolean",
  "isTenantRestricted": "Boolean",
  "ipAddress": "String",
  "ipAddressFromResourceProvider": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "privateLinkDetails": {
    "@odata.type": "microsoft.graph.privateLinkDetails"
  },
  "processingTimeInMilliseconds": "Integer",
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "resourceTenantId": "String",
  "servicePrincipalCredentialKeyId": "String",
  "servicePrincipalCredentialThumbprint": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "signInEventTypes": [
    "String"
  ],
  "signInIdentifier": "String",
  "signInIdentifierType": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
