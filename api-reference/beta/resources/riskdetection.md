---
title: riskDetection 资源类型
description: 表示 AzureAD 租户中的所有风险检测。
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5e27d1df57ac4242f74cca746b7dc8890f004c7a
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060484"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关Azure AD租户中检测到的风险的信息。 

Azure AD根据各种信号和机器学习持续评估[用户风险](riskyuser.md)、应用或用户[登录](signin.md)风险。 此 API 提供对Azure AD环境中的所有风险检测的编程访问。

有关风险事件的详细信息，请[参阅Azure Active Directory标识保护](/azure/active-directory/identity-protection/overview-identity-protection)。

>[!NOTE]
> 1. 必须具有Azure AD Premium P1或 P2 许可证才能使用风险检测 API。
> 2. 风险检测数据的可用性受[Azure AD数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的约束。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskDetection](../api/riskdetection-list.md) | [riskDetection](riskdetection.md) 集合|列出风险检测及其属性。|
|[获取 riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|获取特定的风险检测及其属性。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|id|string|风险检测的唯一 ID。 |
|requestId|string|与风险检测关联的登录的请求 ID。 如果风险检测未与登录关联，则此属性为 null。|
|correlationId|string|与风险检测关联的登录的相关 ID。 如果风险检测未与登录关联，则此属性为 null。 |
|riskEventType|string|检测到的风险事件的类型。 可能的值是`unlikelyTravel`，、`anonymizedIPAddress`、`maliciousIPAddress`、`malwareInfectedIPAddress``unfamiliarFeatures`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence``adminConfirmedUserCompromised``generic`、、`mcasSuspiciousInboxManipulationRules``investigationsThreatIntelligenceSigninLinked``mcasImpossibleTravel`、`maliciousIPAddressValidCredentialsBlockedIP`和 。`unknownFutureValue` <br/> 有关每个值的详细信息，请参阅 [riskEventType 值](#riskeventtype-values)。|
|riskState|riskState|检测到的风险用户或登录的状态。 可能的值是`none`，、`confirmedSafe`、`remediated`、`atRisk``dismissed`和 `confirmedCompromised``unknownFutureValue`。 |
|riskLevel|riskLevel|检测到的风险级别。 可能的值是`low`， ， `high``medium`， `hidden`， ， `none`。 `unknownFutureValue` <br />**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 `hidden`P1 客户。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可能的值是`none`，`adminGeneratedTemporaryPassword`、、`userPerformedSecuredPasswordReset``userPerformedSecuredPasswordChange`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy``adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、 `adminConfirmedUserCompromised``unknownFutureValue` <br />**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 `hidden`P1 客户。|
|source|string|风险检测的来源。 例如，`activeDirectory`。 |
|detectionTimingType|riskDetectionTimingType|检测到的风险的计时 (实时/脱机) 。 可能的值是`notDefined`， ， `nearRealtime``realtime`， ， `offline`。 `unknownFutureValue` |
|活动|activityType|指示检测到的风险链接到的活动类型。 可能的值是 `signin`， `user`. `unknownFutureValue` |
|tokenIssuerType|tokenIssuerType|指示检测到的登录风险的令牌颁发者类型。 可取值为：`AzureAD`、`ADFederationServices` 和 `unknownFutureValue`。 |
|ipAddress|string|提供发生风险的客户端的 IP 地址。 |
|location|[signInLocation](signinlocation.md)|登录位置。 |
|activityDateTime|DateTimeOffset|发生风险活动的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|detectedDateTime|DateTimeOffset|检测到风险的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z` |
|lastUpdatedDateTime|DateTimeOffset|上次更新风险检测的日期和时间。 |
|userId|string|用户的唯一 ID。  DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|userDisplayName|string|用户名。 |
|userPrincipalName|string|用户的用户主体名称 (UPN)。 |
|additionalInfo|string|与 JSON 格式的风险检测相关联的其他信息。 |
|riskType (已弃用) |riskEventType|风险事件类型的列表。<br />**注意：** 此属性已弃用。 请改用 **riskEventType** 。 |

### <a name="riskeventtype-values"></a>riskEventType 值

| 成员 | 说明 |
|--|--|
| unlikelyTravel | 标识两个来自地理遥远位置的登录，根据过去的行为，其中至少有一个位置可能对用户来说也是非典型的。  |
| anonymizedIPAddress | 指示来自匿名 IP 地址的登录，例如，使用匿名浏览器或 VPN。 |
| maliciousIPAddress | 指示已知为恶意的 IP 地址的登录。 已弃用并且不再为新检测生成。 |
| unfamiliarFeatures | 指示具有与过去登录属性相差的特征的登录。 |
| malwareInfectedIPAddress | 指示来自已感染恶意软件的 IP 地址的登录 |
| suspiciousIPAddress | 标识登录时已知为恶意的 IP 地址的登录名。 |
| leakedCredentials | 指示用户的有效凭据已泄露。 这种共享通常通过在深色 Web 上公开发布、粘贴网站或在黑市上交易和销售凭据来完成。 当 Microsoft 泄露的凭据服务从深色 Web、粘贴站点或其他源获取用户凭据时，会根据Azure AD用户当前的有效凭据检查这些凭据以查找有效的匹配项。 |
| investigationsThreatIntelligence | 指示针对给定用户的异常或与基于 Microsoft 内部和外部威胁情报源的已知攻击模式一致的登录活动。 |
| 通用 | 指示用户未启用标识保护。 |
| adminConfirmedUserCompromised | 指示管理员已 [确认用户已遭入侵](../api/riskyusers-confirmcompromised.md)。 |
| mcasImpossibleTravel | 由 Microsoft Defender for Cloud Apps (MDCA) 发现。 标识一个或多个会话 (两个用户活动，) 在比用户从第一个位置到第二个位置所用的时间短的时间段内从地理上遥远的位置出发，指示另一个用户使用相同的凭据。 |
| mcasSuspiciousInboxManipulationRules | 由 Microsoft Defender for Cloud Apps (MDCA) 发现。 标识可疑的电子邮件转发规则，例如，如果用户创建了一个收件箱规则，该规则将所有电子邮件的副本转发到外部地址。|
| investigationsThreatIntelligenceSigninLinked | 根据威胁情报标识已知攻击模式异常的活动 |
| maliciousIPAddressValidCredentialsBlockedIP | 指示使用来自恶意 IP 地址的有效凭据进行登录。 |
| unknownFutureValue | 可变枚举 sentinel 值。 请勿使用。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskDetection"
}-->

```json
{
 "id": "string",
    "requestId": "string",
    "correlationId": "string",
    "riskType": {"@odata.type": "microsoft.graph.riskEventType"},
    "riskState": {"@odata.type": "microsoft.graph.riskState"},
    "riskLevel": {"@odata.type": "microsoft.graph.riskLevel"},
    "riskDetail": {"@odata.type": "microsoft.graph.riskDetail"},
    "source": "string",
    "detectionTimingType": {"@odata.type": "microsoft.graph.riskDetectionTimingType"},
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"},
    "tokenIssuerType": {"@odata.type": "microsoft.graph.tokenIssuerType"},
    "ipAddress": "string",
    "location": {"@odata.type": "microsoft.graph.signInLocation"},
    "activityDateTime": "string (timestamp)",
    "detectedDateTime": "string (timestamp)",
    "lastUpdatedDateTime": "string (timestamp)",
    "userId": "string",
    "userDisplayName": "string",
    "userPrincipalName": "string",
    "additionalInfo": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskDetections resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
