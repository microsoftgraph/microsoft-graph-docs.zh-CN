---
title: riskDetection 资源类型
description: 风险检测
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7ad9c9a7ec23efdc86470f8ea3ed5245173cd1d1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896873"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

命名空间： microsoft. graph 表示有关 Azure AD 租户中检测到的风险的信息。 

Azure AD 会根据各种信号和机器学习持续评估[用户风险](riskyuser.md)和应用或用户[登录](signin.md)风险。 此 API 提供对 Azure AD 环境中所有风险检测的编程访问。

有关风险事件的详细信息，请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)。

>[!NOTE]
>您必须具有 Azure AD 高级 P1 或 P2 许可证，才能使用风险检测 API。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskDetections](../api/riskdetection-list.md)|[riskDetection](../resources/riskdetection.md)集合|获取[riskDetection](../resources/riskdetection.md)对象及其属性的列表。|
|[获取 riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|读取[riskDetection](../resources/riskdetection.md)对象的属性和关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|activity|activityType|指示检测到的风险所链接到的活动类型。 . 可取值为：`signin`、`user`、`unknownFutureValue`。|
|activityDateTime|DateTimeOffset|风险活动发生的日期和时间。|
|additionalInfo|String|与以 JSON 格式进行的风险检测相关联的其他信息。|
|correlationId|String|与风险检测相关联的登录的相关 ID。 如果风险检测未与登录相关联，则此属性为 null。|
|detectedDateTime|DateTimeOffset|检测到风险的日期和时间。|
|detectionTimingType|riskDetectionTimingType|检测到的风险的时间段（实时/脱机）。 可取值为：`notDefined`、`realtime`、`nearRealtime`、`offline`、`unknownFutureValue`。|
|id|String|风险检测的唯一 ID。 继承自[entity](../resources/entity.md)|
|ipAddress|String|提供从其发生风险的客户端的 IP 地址。|
|lastUpdatedDateTime|DateTimeOffset|上次更新风险检测的日期和时间。|
|location|[signInLocation](../resources/signinlocation.md)|登录的位置。|
|请求|String|与风险检测相关联的登录请求 ID。 如果风险检测未与登录相关联，则此属性为 null。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskEventType|String|检测到的风险事件的类型。 可能的值为、、、、、、、、、、、、 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` 和 `unknownFutureValue` 。|
|riskLevel|riskLevel|检测到的风险的级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|检测到的有风险的用户或登录的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|source|String|风险检测的来源。 例如，"activeDirectory"。 |
|tokenIssuerType|tokenIssuerType|指示检测到的登录风险的令牌颁发者的类型。 可取值为：`AzureAD`、`ADFederationServices`、`UnknownFutureValue`。|
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

