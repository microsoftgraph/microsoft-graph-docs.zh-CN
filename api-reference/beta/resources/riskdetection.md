---
title: riskDetection 资源类型
description: 表示 AzureAD 租户中的所有风险检测。
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: af77e46c688d514f3a7b49aff3c785712706f3e2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960346"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关 Azure AD 租户中检测到的风险的信息。 

Azure AD 根据[](riskyuser.md)各种信号和机器学习持续评估[](signin.md)用户风险以及应用或用户登录风险。 此 API 提供对 Azure AD 环境中的所有风险检测的编程访问权限。

有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)

>[!NOTE]
>必须具有 Azure AD Premium P1 或 P2 许可证才能使用风险检测 API。

## <a name="methods"></a>Methods

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskDetection](../api/riskdetection-list.md) | [riskDetection](riskdetection.md) 集合|列出风险检测及其属性。|
|[获取 riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|获取特定的风险检测及其属性。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|id|string|风险检测的唯一 ID。 |
|requestId|string|与风险检测相关联的登录请求 ID。 如果风险检测未与登录相关联，则此属性为 null。|
|correlationId|string|与风险检测关联的登录的相关 ID。 如果风险检测未与登录相关联，则此属性为 null。 |
|riskEventType|string|检测到的风险事件的类型。 可能的值为 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` 、、、、、、、、 `leakedCredentials` `investigationsThreatIntelligence` 和 `generic` `adminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` 。 |
|riskType|riskEventType|风险事件类型列表。<br />**注意：** 此属性已弃用。 请 **改为使用 riskEventType。** |
|riskState|riskState|检测到有风险的用户或登录的状态。 可能的值为 `none` `confirmedSafe` `remediated` `dismissed` `atRisk` 、、、 和 `confirmedCompromised` `unknownFutureValue` 。 |
|riskLevel|riskLevel|检测到的风险级别。 可能的值为 `low` `medium` `high` `hidden` `none` `unknownFutureValue` 、、、。 <br />**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden` 。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可能的值为 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` 、、、、、、、、、 `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` 。 <br />**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden` 。|
|source|string|风险检测的来源。 例如，`activeDirectory`。 |
|detectionTimingType|riskDetectionTimingType|实时/脱机 (检测到的风险) 。 可能的值为 `notDefined` `realtime` `nearRealtime` `offline` `unknownFutureValue` 、、。 |
|活动|activityType|指示检测到的风险链接到的活动类型。 可能的值为 `signin` `user` `unknownFutureValue` 、、。 |
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
