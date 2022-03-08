---
title: riskDetection 资源类型
description: 表示 AzureAD 租户中的所有风险检测。
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 231141c3ff679af50b5f42652c64b3da18edc005
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335211"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关租户中检测到的风险Azure AD的信息。 

Azure AD根据[各种信号和](riskyuser.md)机器学习持续评估用户风险以及应用或[](signin.md)用户登录风险。 此 API 提供对环境中的所有风险检测的编程Azure AD访问。

有关风险事件详细信息，请参阅Azure Active Directory [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)。

>[!NOTE]
>必须具有一个Azure AD Premium P1 P2 许可证才能使用风险检测 API。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskDetection](../api/riskdetection-list.md) | [riskDetection](riskdetection.md) 集合|列出风险检测及其属性。|
|[获取 riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|获取特定的风险检测及其属性。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|id|string|风险检测的唯一 ID。 |
|requestId|字符串|与风险检测相关联的登录请求 ID。 如果风险检测未与登录相关联，则此属性为 null。|
|correlationId|string|与风险检测关联的登录的相关 ID。 如果风险检测未与登录相关联，则此属性为 null。 |
|riskEventType|字符串|检测到的风险事件的类型。 可能的值是 、`unlikelyTravel``anonymizedIPAddress``maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、、`generic``adminConfirmedUserCompromised``investigationsThreatIntelligence`、`mcasSuspiciousInboxManipulationRules``investigationsThreatIntelligenceSigninLinked``mcasImpossibleTravel``maliciousIPAddressValidCredentialsBlockedIP`和 。`unknownFutureValue` <br/> 有关每个值详细信息，请参阅 [riskEventType 值](#riskeventtype-values)。|
|riskState|riskState|检测到有风险的用户或登录的状态。 可能的值为 、`none``remediated``confirmedSafe`、`dismissed``atRisk`、 `confirmedCompromised`和 。`unknownFutureValue` |
|riskLevel|riskLevel|检测到的风险级别。 可能的值为 、`low``medium``high`、`hidden``none`、。 `unknownFutureValue` <br />**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden`。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可能的值为 、`none``userPerformedSecuredPasswordChange``adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、、`adminConfirmedSigninCompromised``unknownFutureValue``userPassedMFADrivenByRiskBasedPolicy``adminDismissedAllRiskForUser``hidden``adminConfirmedUserCompromised`、 。 <br />**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden`。|
|source|字符串|风险检测的来源。 例如，`activeDirectory`。 |
|detectionTimingType|riskDetectionTimingType|实时/脱机 (检测到的风险) 。 可能的值为 、`notDefined``offline``realtime``nearRealtime`、。 `unknownFutureValue` |
|活动|activityType|指示检测到的风险链接到的活动类型。 可能的值为 、、`signin``user``unknownFutureValue`。 |
|tokenIssuerType|tokenIssuerType|指示检测到的登录风险的令牌颁发者类型。 可取值为：`AzureAD`、`ADFederationServices` 和 `unknownFutureValue`。 |
|ipAddress|string|提供发生风险的客户端的 IP 地址。 |
|location|[signInLocation](signinlocation.md)|登录的位置。 |
|activityDateTime|DateTimeOffset|发生有风险活动的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|detectedDateTime|DateTimeOffset|检测到风险的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z` |
|lastUpdatedDateTime|DateTimeOffset|上次更新风险检测的日期和时间。 |
|userId|string|用户的唯一 ID。  DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|userDisplayName|string|用户名。 |
|userPrincipalName|string|用户的用户主体名称 (UPN)。 |
|additionalInfo|string|与 JSON 格式的风险检测相关的其他信息。 |
|riskType (已弃) |riskEventType|风险事件类型列表。<br />**注意：** 此属性已弃用。 请 **改为使用 riskEventType** 。 |

### <a name="riskeventtype-values"></a>riskEventType 值

| 成员 | 说明 |
|--|--|
| unlikelyTravel | 标识两个源自地理位置较远的位置的登录，如果给定过去的行为，至少其中一个位置对于用户可能也是非典型位置。  |
| 匿名IPAddress | 指示从匿名 IP 地址登录，例如，使用匿名浏览器或 VPN。 |
| maliciousIPAddress | 指示从已知恶意 IP 地址登录。 已弃用并且不再生成用于新检测。 |
| unfamiliarFeatures | 指示特征偏离过去登录属性的登录。 |
| malwareInfectedIPAddress | 指示从感染了恶意软件的 IP 地址登录 |
| suspiciousIPAddress | 标识登录时已知是恶意 IP 地址的登录名。 |
| leakedCredentials | 指示用户的有效凭据已被泄露。 这种共享通常通过公开发布在深色 Web 上、粘贴网站，或在黑市上交易和销售凭据完成。 当 Microsoft 泄露的凭据服务从深色 Web、粘贴网站或其他源获取用户凭据时，会针对 Azure AD 用户的当前有效凭据检查这些凭据以查找有效匹配。 |
| investigationsThreatIntelligence | 指示给定用户不常见的登录活动，或与基于 Microsoft 内部和外部威胁情报源的已知攻击模式一致的登录活动。 |
| generic | 指示用户未启用 Identity Protection。 |
| adminConfirmedUserComprom一 | 指示管理员已 [确认用户受到威胁](../api/riskyusers-confirmcompromised.md)。 |
| mcasImpossibleTravel | 由 Microsoft Defender for Cloud Apps (MDCA) 。 标识两个用户活动 (一个或多个会话) 源自地理位置较远的位置，其时间短于用户从第一个位置前往第二个位置的时间，这表示其他用户使用的是同一凭据。 |
| mcasSuspiciousInboxManipulationRules | 由 Microsoft Defender for Cloud Apps (MDCA) 。 标识可疑电子邮件转发规则，例如，如果用户创建了一个收件箱规则，将所有电子邮件的副本转发到外部地址。|
| investigationsThreatIntelligenceSigninLinked | 标识基于威胁情报的已知攻击模式不常见的活动 |
| maliciousIPAddressValidCredentialsBlockedIP | 指示使用来自恶意 IP 地址的有效凭据进行登录。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |


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
