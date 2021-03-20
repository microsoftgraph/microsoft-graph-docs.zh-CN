---
title: signIn 资源类型
description: 详细介绍租户和目录租户的用户 (登录) 。
author: besiler
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a4f3a16defa48f1f57072f3c009d4f8c223f47d8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961935"
---
# <a name="signin-resource-type"></a>signIn 资源类型

命名空间：microsoft.graph

详细介绍租户和目录租户的用户 (登录) 。 必须具有 Azure AD Premium P1 或 P2 许可证才能使用 Microsoft Graph API 下载登录日志。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 signIn](../api/signin-list.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[获取 signIn](../api/signin-get.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appDisplayName|String|Azure 门户中显示的应用名称。|
|appId|String|表示 Azure Active Directory 中的应用 ID 的唯一 GUID。|
|appliedConditionalAccessPolicy|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) 集合|提供由相应登录活动触发的条件访问策略列表。|
|clientAppUsed|String|标识用于登录活动的旧客户端。  包括 `Browser` `Exchange Active Sync` `modern clients` `IMAP` 、、、、、 `MAPI` `SMTP` 和 `POP` 。|
|conditionalAccessStatus|conditionalAccessStatus| 报告已激活的条件访问策略的状态。 可能的值是 `success` `failure` ：、、 `notApplied` 和 `unknownFutureValue` 。|
|correlationId|String|启动登录时从客户端发送的请求 ID;用于解决登录活动问题。|
|createdDateTime|DateTimeOffset|启动登录 (UTC) 日期和时间。 示例：2014 年 1 月 1 日午夜报告为 `2014-01-01T00:00:00Z` 。|
|deviceDetail|[deviceDetail](devicedetail.md)|发生登录的设备信息;包括设备 ID、操作系统和浏览器。 |
|id|String|表示登录活动的唯一 ID。|
|ipAddress|String|用于登录的客户端的 IP 地址。|
|isInteractive|Boolean|指示登录是否交互。|
|location|[signInLocation](signinlocation.md)|提供登录源自的城市、州和国家/地区代码。|
|resourceDisplayName|String|用户登录的资源的名称。|
|resourceId|String|用户登录的资源的 ID。|
|riskDetail|riskDetail|提供风险用户、登录或风险事件的特定状态背后的“原因”。 可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 <br>**注意：** 此属性的详细信息需要 Azure AD Premium P2 许可证。 其他许可证返回值 `hidden` 。|
|riskEventTypes|riskEventType 集合|与登录相关的风险事件类型。 可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。|
|riskEventTypes_v2|String collection|与登录关联的风险事件类型列表。 可能的值 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` ：、、、、、、、、 `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` 或 `leakedCredentials` `investigationsThreatIntelligence`  `generic` `unknownFutureValue` 。|
|riskLevelAggregated|riskLevel|聚合的风险级别。 可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 对于所有其他客户，将返回 `hidden`。|
|riskLevelDuringSignIn|riskLevel|登录期间的风险级别。 可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 对于所有其他客户，将返回 `hidden`。|
|riskState|riskState|报告风险用户、登录或风险事件的状态。 可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|status|[signInStatus](signinstatus.md)|登录状态。 包括错误代码和错误描述 (登录失败时的错误) 。|
|userDisplayName|String|启动登录的用户的显示名称。|
|userId|String|启动登录的用户的 ID。|
|userPrincipalName|String|启动登录的用户的用户主体名称。|

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
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "isInteractive": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": ["string"],
  "riskEventTypes_v2": ["String"],
  "resourceDisplayName": "string",
  "resourceId": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
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

