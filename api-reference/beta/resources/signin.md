---
title: 登录资源类型
description: '此资源详细介绍用户或应用程序登录活动目录中。 '
ms.openlocfilehash: e1975b7f690e340931cb2a4f00c29cc95b805a2e
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241074"
---
# <a name="signin-resource-type"></a>登录资源类型
此资源详细介绍用户或应用程序登录活动目录中。 

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表登录](../api/signin-list.md) | [登录](signin.md) |读取属性和登录对象之间的关系。|
|[获取登录](../api/signin-get.md) | [登录](signin.md) |读取属性和登录对象的关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appDisplayName|字符串|指 Azure 门户中显示的应用程序名称。|
|appId|String|引用代表 Azure Active Directory 中的应用程序 Id 的唯一 guid。|
|clientAppUsed|字符串|提供用于登录 activty.E.g 旧客户端。 包括浏览器、 Exchange Active Sync、 IMAP、 MAPI、 SMTP、 POP 现代客户端。|
|appliedConditionalAccessPolicy|[conditionalAccessPolicy](conditionalaccesspolicy.md)集合|提供由相应的登录活动触发的条件的访问策略的列表。|
|conditionalAccessStatus|string| 提供的触发条件访问策略的状态。 可取值为：`success`、`failure`、`notApplied`、`unknownFutureValue`。|
|originalRequestId|字符串|身份验证序列中的第一个请求的请求 id。|
|isInteractive|Boolean|指示是否是交互式登录。|
|tokenIssuerName|字符串|标识提供程序 (例如 sts.microsoft.com) 的名称|
|tokenIssuerType|字符串|提供了 identityProvider 的类型。 可能的值为`AzureAD`， `ADFederationServices`， `UnknownFutureValue`。|
|correlationId|String|指启动登录时，从客户端发送的 ID。 这用于解决对应的登录活动，调用支持人员或支持时。|
|createdDateTime|DateTimeOffset|提供的日期和时间启动登录。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|deviceDetail|[deviceDetail](devicedetail.md)|提供从登录出现的设备信息。 它 inclules 像 deviceId，操作系统、 浏览器的信息。 |
|id|字符串|指示表示登录活动的唯一 ID。|
|ipAddress|String|提供客户端登录出现的 IP 地址。|
|location|[signInLocation](signinlocation.md)|提供市/县、 状态和 2 个字母国家/地区代码从登录出现的位置。|
|processingTimeInMilliseconds|Int|提供处理时间 （毫秒） AD STS 中请求|
|riskDetail|`riskDetail`|提供原因后面的 risky 用户、 登录或风险事件特定状态。 可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。 值`none`是指的任何操作已执行上的用户或登录到目前为止。 **注意：** 仅为 Azure AD Premium P2 客户提供了此属性的详细信息。 将返回所有其他客户`hidden`。|
|riskLevelAggregated|`riskLevel`|提供聚合的风险级别。 可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。 值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。 **注意：** 仅为 Azure AD Premium P2 客户提供了此属性的详细信息。 将返回所有其他客户`hidden`。|
|riskLevelDuringSignIn|`riskLevel`|登录过程中提供的风险级别。 可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。 值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。 **注意：** 仅为 Azure AD Premium P2 客户提供了此属性的详细信息。 将返回所有其他客户`hidden`。|
|riskEventTypes|`riskEventTypes`|提供与登录相关联的风险事件类型的列表。 可能的值为： `unlikelyTravel`， `anonymizedIPAddress`， `maliciousIPAddress`， `unfamiliarFeatures`， `malwareInfectedIPAddress`， `suspiciousIPAddress`， `leakedCredentials`， `investigationsThreatIntelligence`， `generic`，和`unknownFutureValue`。|
|riskState|`riskState`|提供 risky 用户、 登录或风险事件的风险状态。 可能的值为： `none`， `confirmedSafe`， `remediated`， `dismissed`， `atRisk`， `confirmedCompromised`， `unknownFutureValue`。|
|mfaDetail|[mfaDetail](mfadetail.md)|提供相关 MFA 像 MFA 需要，MFA 相应登录状态的信息。|
|networkLocationDetail|[networkLocationDetail](networklocationdetail.md)|提供有关的网络位置的详细信息。|
|riskLevel|string| 提供与登录相关联的风险级别。可能的值为： `low`， `medium`， `high`。|
|status|[signInStatus](signinstatus.md)|提供的登录状态。 可能值包括`Success`和`Failure`。|
|userDisplayName|String|指示显示用户的名称。|
|userId|String|指示用户的用户 Id。|
|userPrincipalName|字符串|指示用户的 UPN。|
|resourceDisplayName|字符串|指示用户登录到的资源的名称|
|resourceId|String|指示用户登录到的资源的 Id。|
|authenticationMethodsUsed|字符串|指示使用的身份验证方法的列表|

## <a name="relationships"></a>Relationships
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
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
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
  "riskEventTypes": "string",
  "resourceDisplayName": "string",
  "resourceId": "string",
  "authenticationMethodsUsed": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
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
