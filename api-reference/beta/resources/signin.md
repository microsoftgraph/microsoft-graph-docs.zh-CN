---
title: signIn 资源类型
doc_type: resourcePageType
description: 提供有关目录中用户或应用程序登录活动的详细信息。
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
ms.openlocfilehash: 84cad7fd567918712f53ac90ba757f09627cf2f7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721969"
---
# <a name="signin-resource-type"></a>signIn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关目录中用户或应用程序登录活动的详细信息。 必须具有 Azure AD Premium P1 或 P2 许可证才能使用 Microsoft Graph API 下载登录日志。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 signIn](../api/signin-list.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[获取 signIn](../api/signin-get.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|alternateSignInName|String|使用电话号码登录时备用登录标识。|
|appDisplayName|String|Azure 门户中显示的应用程序名称。|
|appId|String|Azure Active Directory 中的应用程序标识符。|
|appliedConditionalAccessPolicies|[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合|由相应登录活动触发的条件访问策略列表。|
|authenticationDetails|[authenticationDetail](authenticationdetail.md) 集合|身份验证尝试的结果和有关身份验证方法的其他详细信息。|
|authenticationMethodsUsed|字符串集合|使用的身份验证方法。 可能的值 `SMS` `Authenticator App` `App Verification code` ：、、、、、 `Password` `FIDO` `PTA` 或 `PHS` 。|
|authenticationProcessingDetails|[keyValue](keyvalue.md) 集合|其他身份验证处理详细信息，例如，对于 PTA/PHS 或服务器/服务器场名称（如果为联合身份验证）的代理名称。|
|authenticationRequirement | string | 这将保留所有登录步骤所需的最高级别的身份验证，以成功登录。|
|clientAppUsed|String|用于登录活动的旧客户端。 例如，浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 或 POP。|
|conditionalAccessStatus|string| 触发的条件访问策略的状态。 可能的值 `success` `failure` ：、、 `notApplied` 或 `unknownFutureValue` 。|
|correlationId|String|启动登录时从客户端发送的标识符。 这用于在调用支持时对相应的登录活动进行疑难解答。|
|createdDateTime|DateTimeOffset|启动登录的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|deviceDetail|[deviceDetail](devicedetail.md)|登录发生位置的设备信息。 包括 deviceId、OS 和浏览器等信息。 |
|id|String|表示登录活动的标识符。|
|ipAddress|String|发生登录的客户端的 IP 地址。|
|isInteractive|Boolean|指示登录是否交互。|
|location|[signInLocation](signinlocation.md)|发生登录的城市、省/市/县和 2 个字母的国家/地区代码。|
|networkLocationDetails|[networkLocationDetail](networklocationdetail.md) 集合|网络位置详细信息，如 IP 地址、登录位置、使用的网络类型及其名称。 可能的值 `Named Netowrk` `Extranet` ：、、 `Intranet` 或 `Trusted Network` 。|
|originalRequestId|String|身份验证序列中第一个请求的请求标识符。|
|processingTimeInMilliseconds|Int|AD STS 中的请求处理时间（以毫秒为单位）。|
|resourceDisplayName|String|用户登录的资源的名称。|
|resourceId|String|用户登录的资源的标识符。|
|riskDetail|riskDetail|风险用户、登录或风险事件的特定状态背后的原因。 可能的值 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` ：、、、、、、 `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` 或 `unknownFutureValue` 。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskEventTypes|riskEventType 集合|与登录关联的风险事件类型列表。 可能的值 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` ：、、、、、、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` 或 `unknownFutureValue` 。|
|riskEventTypes_v2|字符串集合|与登录关联的风险事件类型列表。 可能的值 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` ：、、、、、、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`  `generic` 或 `unknownFutureValue` 。|
|riskLevelAggregated|riskLevel|聚合风险级别。 可能的值 `none` `low` `medium` ：、、、、 `high` `hidden` 或 `unknownFutureValue` 。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskLevelDuringSignIn|riskLevel|登录期间的风险级别。 可能的值 `none` `low` `medium` ：、、、、 `high` `hidden` 或 `unknownFutureValue` 。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回所有其他客户 `hidden` 。|
|riskState|riskState|风险用户、登录或风险事件的风险状态。 可能的值 `none` `confirmedSafe` `remediated` ：、、、、、 `dismissed` `atRisk` `confirmedCompromised` 或 `unknownFutureValue` 。|
|servicePrincipalId|String|用于登录的应用程序标识符。 使用应用程序登录时将填充此字段。|
|servicePrincipalName|String|用于登录的应用程序名称。 使用应用程序登录时将填充此字段。|
|status|[signInStatus](signinstatus.md)|登录状态。 包括错误代码和错误说明 (登录失败时) 。|
|tokenIssuerName|String|标识提供程序的名称。 例如，`sts.microsoft.com`。|
|tokenIssuerType|String|标识提供程序的类型。 可能的值 `AzureAD` ：、 `ADFederationServices` 或 `UnknownFutureValue` 。|
|userAgent|String|与登录相关的用户代理信息。|
|userDisplayName|String|用户的显示名称。|
|userId|String|用户的标识符。|
|userPrincipalName|String|用户的 UPN。|

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


