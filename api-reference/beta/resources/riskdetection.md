---
title: riskDetection 资源类型
description: 表示 AzureAD 租户中的所有风险检测。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 231d75798fb8c58e678fbe26a16c2bbb2299290c
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349343"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关 Azure AD 租户中检测到的风险的信息。 

Azure AD 将根据各种信号和机器学习持续评估用户和登录风险。 此 API 提供对 Azure AD 环境中所有风险检测的编程访问。

有关风险事件的详细信息, 请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。

>[!NOTE]
>您必须具有 Azure AD 高级 P2 许可证才能使用风险检测 API。

## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 riskDetection](../api/riskdetection-list.md) | [riskDetection](riskDetection.md)集合|列出风险检测及其属性。|
|[获取 riskDetection](../api/riskdetection-get.md) | [riskDetection](riskdetection.md)|获取特定的风险检测及其属性。|

## <a name="properties"></a>属性

| 属性   | 类型|说明|
|:---------------|:--------|:----------|
|`id`|`string`|风险检测的唯一 ID。 |
|`requestId`|`string`|与风险检测相关联的登录请求 ID。 如果风险检测未与登录相关联, 则此属性为 null。|
|`correlationId`|`string`|与风险检测相关联的登录的相关 ID。 如果风险检测未与登录相关联, 则此属性为 null。 |
|`riskType`|`riskEventType`|检测到的风险事件的类型。 可能的值是 unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、leakedCredentials、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、mcasImpossibleTravel、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP 和向 unknownfuturevalue。 |
|`riskState`|`riskState`|检测到的有风险的用户或登录的状态。 可能的值为 none、confirmedSafe、已修正、已消除、atRisk、confirmedCompromised 和向 unknownfuturevalue。 |
|`riskLevel`|`riskLevel`|检测到的风险的级别。 可能的值为 low、medium、high、hidden、none、向 unknownfuturevalue。 |
|`riskDetail`|`riskDetail`|检测到的风险的详细信息。 可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。 |
|`source`|`string`|风险检测的来源。 例如, "activeDirectory"。 |
|`detectionTimingType`|`riskDetectionTimingType`|检测到的风险的时间段 (实时/脱机)。 可能的值包括 notDefined、实时、nearRealtime、offline 和向 unknownfuturevalue。 |
|`activity`|`activityType`|指示检测到的风险所链接到的活动类型。 可能的值为 "登录"、"用户"、"向 unknownfuturevalue"。 |
|`tokenIssuerType`|`tokenIssuerType`|指示检测到的登录风险的令牌颁发者的类型。 可能的值是 AzureAD、ADFederationServices 和向 unknownfuturevalue。 |
|`ipAddress`|`string`|提供从其发生风险的客户端的 IP 地址。 |
|`location`|[`signInLocation`](signinlocation.md)|登录的位置。 |
|`activityDateTime`|`datetimeoffset`|风险活动发生的日期和时间。 |
|`detectedDateTime`|`datetimeoffset`|检测到风险的日期和时间。 |
|`lastUpdatedDateTime`|`datetime`|上次更新风险检测的日期和时间。 |
|`userId`|`string`|用户的唯一 ID。 |
|`userDisplayName`|`string`|用户名。 |
|`userPrincipalName`|`string`|用户的用户主体名称 (UPN)。 |
|`additionalInfo`|`string`|与以 JSON 格式进行的风险检测相关联的其他信息。 |

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
