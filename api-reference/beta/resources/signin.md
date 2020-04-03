---
title: signIn 资源类型
doc_type: resourcePageType
description: 提供有关目录中用户或应用程序登录活动的详细信息。
author: kholtz
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5aa7659c9ab53ac4879a7ab2f1a13f62c729df63
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125314"
---
# <a name="signin-resource-type"></a>signIn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供有关目录中用户或应用程序登录活动的详细信息。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 signIn](../api/signin-list.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[获取 signIn](../api/signin-get.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|alternateSignInName|String|备用登录标识（无论您何时使用电话号码登录）。|
|appDisplayName|String|Azure 门户中显示的应用程序名称。|
|appId|String|Azure Active Directory 中的应用程序标识符。|
|appliedConditionalAccessPolicies|[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合|由相应的登录活动触发的条件访问策略的列表。|
|authenticationDetails|[authenticationDetail](authenticationdetail.md)集合|身份验证尝试的结果和身份验证方法的其他详细信息。|
|authenticationMethodsUsed|String collection|使用的身份验证方法。 可能的值`SMS`： `Authenticator App`、 `App Verification code`、 `Password` `FIDO` `PTA`、、、或`PHS`。|
|authenticationProcessingDetails|[keyValue](keyvalue.md) 集合|其他身份验证处理详细信息，例如在联合身份验证时 PTA/PHS 或服务器/服务器场名称的代理名称。|
|authenticationRequirement | string | 这将在所有登录步骤中保留所需的最高级别的身份验证，以便登录成功。|
|clientAppUsed|String|用于登录活动的旧客户端。 例如，浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 或 POP。|
|conditionalAccessStatus|string| 触发的条件访问策略的状态。 可能的值`success`： `failure`、 `notApplied`、或`unknownFutureValue`。|
|correlationId|String|启动登录时从客户端发送的标识符。 这用于在调用支持时对相应的登录活动进行故障排除。|
|createdDateTime|DateTimeOffset|启动登录的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|deviceDetail|[deviceDetail](devicedetail.md)|发生登录的设备信息。 包括 deviceId、OS 和浏览器等信息。 |
|id|字符串|表示登录活动的标识符。|
|ipAddress|String|发生登录的客户端的 IP 地址。|
|isInteractive|Boolean|指示登录是否为交互式登录。|
|location|[signInLocation](signinlocation.md)|出现登录位置的城市、省/2 号国家/地区代码。|
|networkLocationDetails|[networkLocationDetail](networklocationdetail.md) 集合|网络位置详细信息，如 IP 地址、登录的位置、所使用的网络类型及其名称。 可能的值`Named Netowrk`： `Extranet`、 `Intranet`、或`Trusted Network`。|
|originalRequestId|String|身份验证序列中的第一个请求的请求标识符。|
|processingTimeInMilliseconds|Int|AD STS 中的请求处理时间（以毫秒为单位）。|
|resourceDisplayName|String|用户登录到的资源的名称。|
|resourceId|String|用户登录到的资源的标识符。|
|riskDetail|riskDetail|风险用户的特定状态、登录或风险事件背后的原因。 可能的值`none`： `adminGeneratedTemporaryPassword`、 `userPerformedSecuredPasswordChange`、 `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser`、、、、、、、 `unknownFutureValue` `adminConfirmedSigninCompromised`或。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 返回`hidden`所有其他客户。|
|riskEventTypes|riskEventType 集合|与登录相关联的风险事件类型的列表。 可能的值`unlikelyTravel`： `anonymizedIPAddress`、 `maliciousIPAddress`、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`、、、、、、、 `unknownFutureValue` `generic`或。|
|riskEventTypes_v2|String collection|与登录相关联的风险事件类型的列表。 可能的值`unlikelyTravel`： `anonymizedIPAddress`、 `maliciousIPAddress`、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence`、、、、、、、 `unknownFutureValue` `generic`或。|
|riskLevelAggregated|riskLevel|聚合风险级别。 可能的值`none`： `low`、 `medium`、 `high` `hidden`、、或`unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 返回`hidden`所有其他客户。|
|riskLevelDuringSignIn|riskLevel|登录过程中的风险级别。 可能的值`none`： `low`、 `medium`、 `high` `hidden`、、或`unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 返回`hidden`所有其他客户。|
|riskState|riskState|有风险的用户、登录或风险事件的风险状态。 可能的值`none`： `confirmedSafe`、 `remediated`、 `dismissed` `atRisk` `confirmedCompromised`、、、或`unknownFutureValue`。|
|servicePrincipalId|String|用于登录的应用程序标识符。 使用应用程序登录时，将填充此字段。|
|servicePrincipalName|String|用于登录的应用程序名称。 使用应用程序登录时，将填充此字段。|
|status|[signInStatus](signinstatus.md)|登录状态。 可能的值`Success` ： `Failure`或。|
|tokenIssuerName|String|标识提供程序的名称。 例如，`sts.microsoft.com`。|
|tokenIssuerType|String|标识提供程序的类型。 可能的值`AzureAD`： `ADFederationServices`、或`UnknownFutureValue`。|
|userAgent|String|与登录相关的用户代理信息。|
|userDisplayName|String|用户的显示名称。|
|userId|String|用户的标识符。|
|userPrincipalName|字符串|用户的 UPN。|

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
