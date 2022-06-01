---
title: signIn 资源类型
doc_type: resourcePageType
description: 提供有关目录中用户或应用程序登录活动的详细信息。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
ms.openlocfilehash: ba1100b738c2904c6661e52df62171a11aa4dda3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819347"
---
# <a name="signin-resource-type"></a>signIn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关目录中用户或应用程序登录活动的详细信息。 必须具有Azure AD Premium P1或 P2 许可证才能使用 Microsoft 图形 API 下载登录日志。

登录日志的可用性受 [Azure AD 数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的约束。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 signIn](../api/signin-list.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[获取 signIn](../api/signin-get.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[确认已被盗用](../api/signin-confirmcompromised.md)|无|将 Azure AD 登录日志中的事件标记为有风险。|
|[确认安全](../api/signin-confirmsafe.md)|无|将 Azure AD 登录日志中的事件标记为安全。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appDisplayName|String|Azure 门户中显示的应用程序名称。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|appId|String|Azure Active Directory中的应用程序标识符。 仅支持 `$filter` (运算 `eq` 符) 。|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) 集合|由相应登录活动触发的条件访问策略列表。|
|authenticationContextClassReferences|[authenticationContext](authenticationcontext.md) 集合|包含一个值集合，这些值表示应用于登录的条件访问身份验证上下文。|
|authenticationDetails|[authenticationDetail](authenticationdetail.md) 集合|身份验证尝试的结果以及有关身份验证方法的其他详细信息。|
|authenticationMethodsUsed|String collection|使用的身份验证方法。 可能的值：`SMS`、`Authenticator App`、`App Verification code`、`Password`、`FIDO`或 `PTA``PHS`。|
|authenticationProcessingDetails|[keyValue](keyvalue.md) 集合|其他身份验证处理详细信息，例如，在联合身份验证的情况下，使用 PTA/PHS 或服务器/场名称的代理名称。|
|authenticationProtocol|protocolType|列出身份验证中使用的协议类型或授权类型。 可取值包括：`none`、`oAuth2`、`ropc`、`wsFederation`、`saml20`、`deviceCode`、`unknownFutureValue`。 对于使用列出的可能值以外的协议的身份验证，将协议类型列为 `none`。 |
|authenticationRequirement | String | 这保存所有登录步骤所需的最高级别的身份验证，以便登录成功。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) 集合|身份验证要求的源，例如条件访问、每用户 MFA、标识保护和安全默认值。|
|autonomousSystemNumber|Int32|执行组件使用的网络的自治系统编号 (ASN) 。|
|azureResourceId|String|包含在登录期间访问的 Azure 资源的完全限定 Azure 资源管理器 ID。|
|clientAppUsed|String|用于登录活动的旧客户端。 例如：、、、、`IMAP``MAPI`或 `POP``SMTP`。 `Modern clients``Exchange ActiveSync``Browser` 仅支持 `$filter` (运算 `eq` 符) 。 |
|clientCredentialType|clientCredentialType|描述用户客户端或服务主体提供给 Azure AD 进行自身身份验证的凭据类型。 你可能希望查看 clientCredentialType 以跟踪和消除不太安全的凭据类型，或者使用异常凭据类型监视客户端和服务主体。 可取值包括：`none`、`clientSecret`、`clientAssertion`、`federatedIdentityCredential`、`managedIdentity`、`certificate`、`unknownFutureValue`。|
|conditionalAccessStatus|conditionalAccessStatus| 触发的条件访问策略的状态。 可能的值：`success`、`failure`或 `notApplied``unknownFutureValue`。 仅支持 `$filter` (运算 `eq` 符) 。|
|correlationId|String|启动登录时从客户端发送的标识符。 这用于在调用支持时对相应的登录活动进行故障排除。 仅支持 `$filter` (运算 `eq` 符) 。|
|createdDateTime|DateTimeOffset|登录的启动日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$orderby` 和 `$filter` (`eq`， `le`运 `ge` 算符仅) 。|
|crossTenantAccessType|signInAccessType|描述执行组件用于访问资源的跨租户访问类型。 可取值为：`none`、`b2bCollaboration`、`b2bDirectConnect`、`microsoftSupport`、`serviceProvider`、`unknownFutureValue`。 如果登录未跨越租户边界，则值为 `none`。|
|deviceDetail|[deviceDetail](devicedetail.md)|登录发生位置的设备信息。 包括 deviceId、OS 和浏览器等信息。 仅支持`$filter`在`eq`**浏览器** 和 `startsWith` **operatingSystem** 属性上)  (和运算符。|
|federatedCredentialId|String|如果使用联合标识凭据登录，则包含应用程序的联合标识凭据的标识符。|
|flaggedForReview|布尔|在登录失败期间，用户可以单击Azure 门户中的按钮，为租户管理员标记失败的事件。 如果用户单击按钮标记失败的登录，则此值为 `true`。|
|homeTenantId|String|发起登录的用户的租户标识符。 不适用于托管标识或服务主体登录。|
|homeTenantName|String|对于用户登录，用户所属的租户的标识符。 仅在家庭租户向 Azure AD 提供肯定同意以显示租户内容的情况下填充。|
|id|String|表示登录活动的标识符。 继承自 [entity](entity.md)。 仅支持 `$filter` (运算 `eq` 符) 。|
|incomingTokenType|incomingTokenType|指示显示给 Azure AD 的令牌类型，以便对登录中的执行组件进行身份验证。 可能的值包括 `none`、`primaryRefreshToken`、`saml11`、`saml20`、`unknownFutureValue`、`remoteDesktopToken`。 <br><br> **注意** Azure AD 可能还使用此枚举类型中未列出的令牌类型对执行组件进行身份验证。 如果令牌不是列出的类型之一，请勿推断令牌的缺失。 此外，请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中 () 的以下值： `remoteDesktopToken`|
|ipAddress|String|发生登录的客户端的 IP 地址。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|ipAddressFromResourceProvider|String|用于访问资源提供程序的用户的 IP 地址，用于确定某些策略的条件访问符合性。 例如，当用户与Exchange Online交互时，可能会在此处记录Exchange从用户接收的 IP 地址。 此值通常是 `null`。|
|isInteractive|Boolean|指示用户登录是否为交互式。 在交互式登录中，用户向 Azure AD 提供身份验证因子。 这些因素包括密码、对 MFA 挑战的响应、生物识别因素或用户提供给 Azure AD 或关联应用的 QR 代码。 在非交互式登录中，用户不提供身份验证因子。 相反，客户端应用使用令牌或代码代表用户对资源进行身份验证或访问。 非交互式登录通常用于客户端在用户透明的进程中代表用户登录。|
|isTenantRestricted|布尔|显示登录事件是否受 Azure AD 租户限制策略的限制。|
|location|[signInLocation](signinlocation.md)|登录发生地的城市、州和 2 个字母国家/地区代码。 仅支持`$filter`对`eq`**城市**、**州** 和 `startsWith` **countryOrRegion** 属性)  (和运算符。|
|networkLocationDetails|[networkLocationDetail](networklocationdetail.md) 集合|网络位置详细信息，包括使用的网络类型及其名称。|
|originalRequestId|String|身份验证序列中第一个请求的请求标识符。 仅支持 `$filter` (运算 `eq` 符) 。|
|privateLinkDetails|[privateLinkDetails](../resources/privatelinkdetails.md)|包含有关与登录事件关联的 Azure AD 专用链接策略的信息。|
|processingTimeInMilliseconds|Int|AD STS 中的请求处理时间（以毫秒为单位）。|
|resourceDisplayName|String|用户登录到的资源的名称。 仅支持 `$filter` (运算 `eq` 符) 。|
|resourceId|String|用户登录到的资源的标识符。 仅支持 `$filter` (运算 `eq` 符) 。|
|resourceServicePrincipalId|String|在登录事件中代表目标资源的服务主体标识符。|
|resourceTenantId|String|登录中引用的资源的租户标识符。|
|riskDetail|riskDetail|风险用户、登录或风险事件的特定状态背后的原因。 可能的值：`none`、、`userPerformedSecuredPasswordChange``adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminConfirmedSigninCompromised``adminDismissedAllRiskForUser`或 `unknownFutureValue`。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 仅支持 `$filter` (运算 `eq` 符) 。<br> **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 返回所有其他客户 `hidden`。|
|riskEventTypes_v2|String collection|与登录关联的风险事件类型的列表。 可能的值：`unlikelyTravel`、、`maliciousIPAddress``anonymizedIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`generic``investigationsThreatIntelligence`或 `unknownFutureValue`。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|riskLevelAggregated|riskLevel|聚合风险级别。 可能的值：`none`、`low`、`medium`、`high`或 `hidden``unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 仅支持 `$filter` (运算 `eq` 符) 。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 返回所有其他客户 `hidden`。|
|riskLevelDuringSignIn|riskLevel|登录期间的风险级别。 可能的值：`none`、`low`、`medium`、`high`或 `hidden``unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 仅支持 `$filter` (运算 `eq` 符) 。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 返回所有其他客户 `hidden`。|
|riskState|riskState|风险用户、登录或风险事件的风险状态。 可能的值：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`或 `confirmedCompromised``unknownFutureValue`。 仅支持 `$filter` (运算 `eq` 符) 。|
|servicePrincipalCredentialKeyId|String|服务主体用来进行身份验证的密钥凭据的唯一标识符。|
|servicePrincipalCredentialThumbprint|String|服务主体用来进行身份验证的证书的证书指纹。|
|servicePrincipalId|String|用于登录的应用程序标识符。 使用应用程序登录时，将填充此字段。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|servicePrincipalName|String|用于登录的应用程序名称。 使用应用程序登录时，将填充此字段。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|sessionLifetimePolicies|[sessionLifetimePolicy](sessionlifetimepolicy.md) 集合|在登录事件中应用的任何条件访问会话管理策略。|
|signInEventTypes|String collection|指示事件表示的登录类别。 对于用户登录，类别可以是 `interactiveUser` 或 `nonInteractiveUser` 对应于登录资源上的 **isInteractive** 属性的值。 对于托管标识登录，类别为 `managedIdentity`。 对于服务主体登录，类别为 **servicePrincipal**。 可取值为：`interactiveUser`、`nonInteractiveUser`、`servicePrincipal`、`managedIdentity`、`unknownFutureValue`。 支持 `$filter`（`eq`、`ne`）。|
|signInIdentifier|String|用户提供的登录标识。 它可能是 userPrincipalName，但在用户使用其他标识符登录时也会填充它。|
|signInIdentifierType|signInIdentifierType|登录标识符的类型。 可取值为：`userPrincipalName`、`phoneNumber`、`proxyAddress`、`qrCode`、`onPremisesUserPrincipalName`、`unknownFutureValue`。|
|status|[signInStatus](signinstatus.md)|登录状态。 包括登录失败) 时 (的错误代码和说明。 仅支持 `$filter` errorCode 属性上的 (`eq` 运 **算符**) 。|
|tokenIssuerName|String|标识提供者的名称。 例如，`sts.microsoft.com`。 仅支持 `$filter` (运算 `eq` 符) 。|
|tokenIssuerType|tokenIssuerType|标识提供者的类型。 可能的值包括 `AzureAD`、`ADFederationServices`、`UnknownFutureValue`、`AzureADBackupAuth`、`ADFederationServicesMFAAdapter`、`NPSExtension`。 请注意，必须使用`Prefer: include-unknown-enum-members`请求标头获取此[可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)中的以下值： `AzureADBackupAuth` ， ， `ADFederationServicesMFAAdapter` 。 `NPSExtension`|
|uniqueTokenIdentifier|String|唯一的 base64 编码请求标识符，用于跟踪 Azure AD 颁发的令牌，因为它们是在资源提供程序中兑换的。 |
|userAgent|String|与登录相关的用户代理信息。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|userDisplayName|String|用户的显示名称。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|userId|String|用户的标识符。 仅支持 `$filter` (运算 `eq` 符) 。|
|userPrincipalName|String|用户的 UPN。 仅支持 `$filter` (`eq` 和 `startsWith` 运算符) 。|
|userType|signInUserType|标识用户是租户中的成员还是来宾。 可取值为：`member`、`guest`、`unknownFutureValue`。|
|mfaDetail (已弃用) |String|此属性已弃用。|


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
  "authenticationContextClassReferences": [{"@odata.type": "microsoft.graph.authenticationContext"}],
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
  "azureResourceId": "String",
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "crossTenantAccessType": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "federatedCredentialId": "String",
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
  "sessionLifetimePolicies": [{"@odata.type": "microsoft.graph.sessionLifetimePolicy"}],
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
