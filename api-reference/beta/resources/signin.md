---
title: signIn 资源类型
doc_type: resourcePageType
description: 描述 Microsoft Graph API (REST) 的 signIn 资源，这有利于审核用户和应用程序登录活动（beta 版本）。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a0f3977c14ce8e0e53cdbd296ea28c4b79f5762
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396742"
---
# <a name="signin-resource-type"></a>signIn 资源类型

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
|appDisplayName|String|表示 Azure 门户中显示的应用程序名称。|
|appId|String|表示唯一 GUID（表示 Azure Active Directory 中的应用程序 ID）。|
|clientAppUsed|String|提供用于登录活动的旧版客户端。例如， 包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI SMTP、POP。|
|appliedConditionalAccessPolicies|[conditionalAccessPolicy](conditionalaccesspolicy.md) 集合|提供由相应登录活动触发的条件访问策略列表。|
|conditionalAccessStatus|string| 提供触发的条件访问策略的状态。 可取值为：`success`、`failure`、`notApplied`、`unknownFutureValue`。|
|originalRequestId|String|身份验证序列中第一个请求的请求 ID。|
|isInteractive|Boolean|指示登录是否为交互式。|
|tokenIssuerName|String|标识提供者（例如 sts.microsoft.com）的名称|
|tokenIssuerType|String|提供标识提供者的类型。 可取值为 `AzureAD`、`ADFederationServices`、`UnknownFutureValue`。|
|correlationId|String|表示登录启动时从客户端发送的 ID。 此属性用于在调用帮助台或支持时对相应的登录活动进行故障诊断。|
|createdDateTime|DateTimeOffset|提供登录启动的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|提供发生登录的设备的信息。 包括设备 ID、操作系统、浏览器等信息。 |
|id|String|表示登录活动的唯一 ID。|
|ipAddress|String|提供发生登录的客户端的 IP 地址。|
|location|[signInLocation](signinlocation.md)|提供发生登录的城市、省/市/自治区和 2 个字母的国家/地区代码。|
|processingTimeInMilliseconds|Int|提供 AD STS 中的请求处理时间（以毫秒为单位）|
|riskDetail|`riskDetail`|提供风险用户、登录或风险事件的特定状态背后的“原因”。 可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 对于所有其他客户，将返回 `hidden`。|
|riskLevelAggregated|`riskLevel`|提供聚合的风险级别。 可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 对于所有其他客户，将返回 `hidden`。|
|riskLevelDuringSignIn|`riskLevel`|提供登录期间的风险级别。 可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 对于所有其他客户，将返回 `hidden`。|
|riskEventTypes|`riskEventType` 集合|提供与登录关联的风险事件类型列表。 可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。|
|riskState|`riskState`|提供风险用户、登录或风险事件的“风险状态”。 可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|mfaDetail|[mfaDetail](mfadetail.md)|提供相应登录的 MFA 相关信息，例如“需要 MFA”、“MFA 状态”。|
|networkLocationDetails|[networkLocationDetail](networklocationdetail.md) 集合|提供有关网络位置的详细信息。|
|status|[signInStatus](signinstatus.md)|提供登录状态。 可取值包括 `Success` 和 `Failure`。|
|userDisplayName|String|指示用户的显示名称。|
|userId|String|指示用户的用户 ID。|
|userPrincipalName|String|指示用户的 UPN。|
|resourceDisplayName|String|指示用户登录的资源的名称|
|resourceId|String|指示用户登录的资源的 ID。|
|authenticationMethodsUsed|String|指示使用的身份验证方法列表|

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
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "mfaDetail": {"@odata.type": "microsoft.graph.mfaDetail"},
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicies": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "originalRequestId": "String",
  "isInteractive": "String",
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "processingTimeInMilliseconds": 12356,
  "networkLocationDetails": [{"@odata.type": "microsoft.graph.networkLocationDetail"}]
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
