---
title: signIn 资源类型
doc_type: resourcePageType
description: 提供有关目录中用户或应用程序登录活动的详细信息。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
ms.openlocfilehash: d3b077823872842e23ea38b1383636809f7e408e
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2021
ms.locfileid: "61402886"
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
|alternateSignInName|String|每次使用电话号码登录时，备用登录标识。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|appDisplayName|String|Azure 门户中显示的应用程序名称。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|appId|String|应用程序中的应用程序Azure Active Directory。 仅 `$filter` (`eq` 运算符) 。|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) 集合|由相应登录活动触发的条件访问策略列表。|
|authenticationDetails|[authenticationDetail](authenticationdetail.md) 集合|身份验证尝试的结果和有关身份验证方法的其他详细信息。|
|authenticationMethodsUsed|字符串集合|使用的身份验证方法。 可能的值 `SMS` `Authenticator App` `App Verification code` ：、、、、、、 `Password` `FIDO` `PTA` 或 `PHS` 。|
|authenticationProcessingDetails|[keyValue](keyvalue.md) 集合|其他身份验证处理详细信息，例如 PTA/PHS 中的代理名称或联合身份验证情况下的服务器/服务器场名称。|
|authenticationRequirement | 字符串 | 这将保留所有登录步骤所需的最高级别的身份验证，以成功登录。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|clientAppUsed|String| 标识用于登录活动的客户端。 新式验证客户端包括 `Browser` `modern clients` 和 。 旧版身份验证客户端包括 `Exchange Active Sync` `IMAP` `MAPI` 、、、、 `SMTP` 和 `POP` `other clients` 。 仅 `$filter` (`eq` 运算符) 。 |
|conditionalAccessStatus|conditionalAccessStatus| 触发的条件访问策略的状态。 可能的值 `success` `failure` ：、、 `notApplied` 或 `unknownFutureValue` 。 仅 `$filter` (`eq` 运算符) 。|
|correlationId|String|启动登录时从客户端发送的标识符。 这用于在调用支持时对相应的登录活动进行疑难解答。 仅 `$filter` (`eq` 运算符) 。|
|createdDateTime|DateTimeOffset|启动登录的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 仅 `$orderby` 支持 `$filter` (`eq` `le` 、、 `ge` 和 运算符) 。|
|deviceDetail|[deviceDetail](devicedetail.md)|登录发生位置的设备信息。 包括 deviceId、OS 和浏览器等信息。 仅 `$filter` (`eq` `startsWith` 浏览器和 **operatingSytem**) **和** 运算符。|
|id|String|表示登录活动的标识符。 仅 `$filter` (`eq` 运算符) 。|
|ipAddress|String|发生登录的客户端的 IP 地址。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|isInteractive|Boolean|指示登录是否交互。|
|location|[signInLocation](signinlocation.md)|发生登录的城市、省/市/县和 2 个字母的国家/地区代码。 仅 `$filter` (`eq` `startsWith` city、state 和 **countryOrRegion** 属性) 和运算符。|
|networkLocationDetails|[networkLocationDetail](networklocationdetail.md) 集合|网络位置详细信息，包括所使用的网络的类型及其名称。|
|originalRequestId|String|身份验证序列中第一个请求的请求标识符。 仅 `$filter` (`eq` 运算符) 。|
|processingTimeInMilliseconds|Int|AD STS 中的请求处理时间（以毫秒为单位）。|
|resourceDisplayName|String|用户登录的资源的名称。 仅 `$filter` (`eq` 运算符) 。|
|resourceId|String|用户登录到的资源的标识符。 仅 `$filter` (`eq` 运算符) 。|
|riskDetail|riskDetail|风险用户、登录或风险事件的特定状态背后的原因。 可能的值 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` ：、、、、、、、、 `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` 或 `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `unknownFutureValue` 。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 仅 `$filter` (`eq` 运算符) 。<br> **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskEventTypes|riskEventType 集合|与登录关联的风险事件类型列表。 可能的值 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` ：、、、、、、、、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` 或 `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` 。 仅 `$filter` (`eq` 运算符) 。|
|riskEventTypes_v2|字符串集合|与登录关联的风险事件类型列表。 可能的值 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` ：、、、、、、、、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` 或 `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` 。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|riskLevelAggregated|riskLevel|聚合的风险级别。 可能的值 `none` `low` `medium` ：、、、、 `high` `hidden` 或 `unknownFutureValue` 。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 仅 `$filter` (`eq` 运算符) 。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskLevelDuringSignIn|riskLevel|登录期间的风险级别。 可能的值 `none` `low` `medium` ：、、、、 `high` `hidden` 或 `unknownFutureValue` 。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 仅 `$filter` (`eq` 运算符) 。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskState|riskState|风险用户、登录或风险事件的风险状态。 可能的值 `none` `confirmedSafe` `remediated` ：、、、、、、 `dismissed` `atRisk` `confirmedCompromised` 或 `unknownFutureValue` 。 仅 `$filter` (`eq` 运算符) 。|
|servicePrincipalId|字符串|用于登录的应用程序标识符。 使用应用程序登录时将填充此字段。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|servicePrincipalName|String|用于登录的应用程序名称。 使用应用程序登录时将填充此字段。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|status|[signInStatus](signinstatus.md)|登录状态。 包括错误代码和错误描述 (登录失败时的错误) 。 仅 `$filter` (`eq` **errorCode**) 属性的运算符。|
|tokenIssuerName|String|标识提供程序的名称。 例如，`sts.microsoft.com`。 仅 `$filter` (`eq` 运算符) 。|
|tokenIssuerType|tokenIssuerType|标识提供程序的类型。 可能的值 `AzureAD` ：、 `ADFederationServices` 或 `UnknownFutureValue` 。|
|userAgent|String|与登录相关的用户代理信息。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|userDisplayName|String|用户的显示名称。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|
|userId|String|用户的标识符。 仅 `$filter` (`eq` 运算符) 。|
|userPrincipalName|String|用户的 UPN。 仅 `$filter` (`eq` `startsWith` 运算符和) 。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signIn"
}-->

```json
{
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "authenticationDetails": [{"@odata.type": "microsoft.graph.authenticationDetail"}],
  "authenticationMethodsUsed": ["String"],
  "authenticationProcessingDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "string",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "id": "String (identifier)",
  "ipAddress": "String",
  "isInteractive": true,
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": 1024,
  "resourceDisplayName": "String",
  "resourceId": "String",
  "riskDetail": "string",
  "riskEventTypes": ["string"],
  "riskEventTypes_v2": ["String"],
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "tokenIssuerName": "String",
  "tokenIssuerType": "string",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String"
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


