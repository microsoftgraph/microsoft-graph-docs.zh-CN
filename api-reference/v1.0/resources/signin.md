---
title: signIn 资源类型
description: 详细介绍租户（目录）的用户和应用程序登录活动。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 367be35ffc1c37b04f2c3f5f1c70139e4562c870
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533716"
---
# <a name="signin-resource-type"></a>signIn 资源类型

命名空间：microsoft.graph

详细介绍租户（目录）的用户和应用程序登录活动。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 signIn](../api/signin-list.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|
|[获取 signIn](../api/signin-get.md) | [signIn](signin.md) |读取 signIn 对象的属性和关系。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|appDisplayName|字符串|Azure 门户中显示的应用程序名称。|
|appId|字符串|表示 Azure Active Directory 中的应用程序 ID 的唯一 GUID。|
|appliedConditionalAccessPolicy|[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)集合|提供由相应登录活动触发的条件访问策略列表。|
|clientAppUsed|String|标识用于登录活动的旧客户端。  包括浏览器、Exchange Active Sync、新式客户端、IMAP、MAPI、SMTP 和 POP。|
|conditionalAccessStatus|string| 报告激活的条件访问策略的状态。 可能的值是`success`： `failure`、 `notApplied`、和`unknownFutureValue`。|
|correlationId|字符串|启动登录时从客户端发送的请求 ID;用于对登录活动进行故障排除。|
|createdDateTime|DateTimeOffset|启动登录的日期和时间（UTC）。 示例：2014年1月1日午夜，报告`'2014-01-01T00:00:00Z'`为。|
|deviceDetail|[deviceDetail](devicedetail.md)|发生登录的设备信息;包括设备 ID、操作系统和浏览器。 |
|id|字符串|表示登录活动的唯一 ID。|
|ipAddress|字符串|用于登录的客户端的 IP 地址。|
|isInteractive|Boolean|指示登录是否为交互式登录。|
|location|[signInLocation](signinlocation.md)|提供登录所源于的城市、州和国家/地区代码。|
|resourceDisplayName|字符串|用户登录到的资源的名称。|
|resourceId|String|用户登录到的资源的 ID。|
|riskDetail|riskDetail|提供风险用户、登录或风险事件的特定状态背后的“原因”。 可取值包括：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。 值 `none` 表示到目前为止尚未对用户或登录执行任何操作。 <br>**注意：** 此属性的详细信息需要 Azure AD Premium P2 许可证。 其他许可证返回值`hidden`。|
|riskEventTypes|riskEventTypes|与登录相关联的风险事件类型。 可取值为：`unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic` 和 `unknownFutureValue`。|
|riskLevelAggregated|riskLevel|聚合风险级别。 可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 对于所有其他客户，将返回 `hidden`。|
|riskLevelDuringSignIn|riskLevel|登录过程中的风险级别。 可取值为：`none`、`low`、`medium`、`high`、`hidden` 和 `unknownFutureValue`。 值 `hidden` 表示用户或登录未启用 Azure AD Identity Protection。 **注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 对于所有其他客户，将返回 `hidden`。|
|riskState|riskState|报告有风险的用户、登录或风险事件的状态。 可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|status|[signInStatus](signinstatus.md)|登录状态。 可取值包括 `Success` 和 `Failure`。|
|userDisplayName|字符串|启动登录的用户的显示名称。|
|userId|字符串|启动登录的用户的 ID。|
|userPrincipalName|字符串|启动登录的用户的用户主体名称。|

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
  "riskEventTypes": "string",
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
