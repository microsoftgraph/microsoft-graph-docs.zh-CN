---
title: riskDetection 资源类型
description: 风险检测
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e52fb1b67d82091360f83383d941552316d107b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449003"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

命名空间：microsoft.graph 表示有关 Azure AD 租户中检测到的风险的信息。 

Azure AD 根据[](riskyuser.md)各种信号和机器学习持续评估[](signin.md)用户风险以及应用或用户登录风险。 此 API 提供对 Azure AD 环境中的所有风险检测的编程访问。

有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)

>[!NOTE]
>必须具有 Azure AD Premium P1 或 P2 许可证才能使用风险检测 API。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskDetections](../api/riskdetection-list.md)|[riskDetection](../resources/riskdetection.md) 集合|获取 [riskDetection](../resources/riskdetection.md) 对象及其属性的列表。|
|[获取 riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|读取 [riskDetection](../resources/riskdetection.md) 对象的属性和关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|活动|activityType|指示检测到的风险链接到的活动类型。 . 可取值为：`signin`、`user`、`unknownFutureValue`。|
|activityDateTime|DateTimeOffset|发生风险活动的日期和时间。|
|additionalInfo|String|与 JSON 格式的风险检测相关的其他信息。|
|correlationId|String|与风险检测相关联的登录的相关 ID。 如果风险检测未与登录相关联，则此属性为 null。|
|detectedDateTime|DateTimeOffset|检测到风险的日期和时间。|
|detectionTimingType|riskDetectionTimingType|实时/脱机 (检测到的风险) 。 可取值为：`notDefined`、`realtime`、`nearRealtime`、`offline`、`unknownFutureValue`。|
|id|String|风险检测的唯一 ID。 继承自 [实体](../resources/entity.md)|
|ipAddress|String|提供发生风险的客户端的 IP 地址。|
|lastUpdatedDateTime|DateTimeOffset|上次更新风险检测的日期和时间。|
|location|[signInLocation](../resources/signinlocation.md)|登录的位置。|
|requestId|String|与风险检测相关联的登录请求 ID。 如果风险检测未与登录相关联，则此属性为 null。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskEventType|String|检测到的风险事件的类型。 可能的值是 `unlikelyTravel` ， `anonymizedIPAddress` ， ， ， ， ， ， `maliciousIPAddress` ， `unfamiliarFeatures` `malwareInfectedIPAddress` 和 `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` 。 如果风险检测是高级检测，将显示 `generic`|
|riskLevel|riskLevel|检测到的风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|检测到有风险的用户或登录的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|source|String|风险检测的来源。 例如，"activeDirectory"。 |
|tokenIssuerType|tokenIssuerType|指示检测到的登录风险的令牌颁发者类型。 可取值为：`AzureAD`、`ADFederationServices`、`UnknownFutureValue`。|
|userDisplayName|String|用户的用户主体名称 (UPN)。 |
|userId|String|用户的唯一 ID。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "String (identifier)",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```
