---
title: servicePrincipalRiskDetection 资源类型
description: 表示有关租户中检测到的风险服务主体Azure AD的信息。
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 63eb90a7147394eb6639083f7f965e8759262901
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519935"
---
# <a name="serviceprincipalriskdetection-resource-type"></a>servicePrincipalRiskDetection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关在租户中检测到的风险服务Azure AD的信息。 Azure AD根据各种信号和机器学习持续评估风险。 此 API 提供对环境中所有服务主体风险检测的Azure AD访问权限。

继承自 [实体](../resources/entity.md)。

有关风险事件详细信息，请参阅Azure Active Directory [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)。 

>**注意：** 必须具有证书或 P2 Azure AD Premium P1才能使用 servicePrincipalRiskDetection API。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 servicePrincipalRiskDetections](../api/identityprotectionroot-list-serviceprincipalriskdetections.md)|[servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md) 集合|列出服务主体风险检测及其属性。|
|[获取 servicePrincipalRiskDetection](../api/serviceprincipalriskdetection-get.md)|[servicePrincipalRiskDetection](../resources/serviceprincipalriskdetection.md)|获取特定服务主体风险检测及其属性。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|活动|activityType|指示检测到的风险链接到的活动类型。  可能的值包括 `signin`、`unknownFutureValue`、`servicePrincipal`。 请注意，必须使用此可 `Prefer: include-unknown-enum-members` 变化枚举 (请求) 获取以下 [值](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)： `servicePrincipal`。 |
|activityDateTime|DateTimeOffset|发生风险活动的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|additionalInfo|字符串|与风险检测相关的其他信息。 此字符串值表示为转义引号的 JSON 对象。 |
|appId|String|关联的应用程序的唯一标识符。|
|correlationId|String|与风险检测关联的登录活动的关联 ID。 此属性是 `null` 风险检测未与登录活动相关联时。|
|detectedDateTime|DateTimeOffset|检测到风险的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|detectionTimingType|riskDetectionTimingType|检测到的风险（实时或脱机）的时间) 。 可能的值包括 `notDefined`、`realtime`、`nearRealtime`、`offline`、`unknownFutureValue`。|
|id|String|风险检测的唯一标识符。 继承自 [实体](../resources/entity.md)。|
|ipAddress|String|提供发生风险的客户端的 IP 地址。|
|keyIds|String collection|与风险 (关联的) 凭据的唯一标识符和 GUID 值。|
|lastUpdatedDateTime|DateTimeOffset|上次更新风险检测的日期和时间。|
|location|[signInLocation](signinlocation.md)|从其中启动登录的位置。 |
|requestId|String|与风险检测关联的登录活动的请求标识符。 此属性是 `null` 风险检测未与登录活动相关联时。 支持 `$filter`（`eq`）。|
|riskDetail|riskDetail|检测到的风险的详细信息。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden`。 <br/>可能的值包括 `none`、`hidden`、`unknownFutureValue`、`adminConfirmedServicePrincipalCompromised`、`adminDismissedAllRiskForServicePrincipal`。 请注意，必须使用此可`Prefer: include-unknown-enum-members`变化枚举 (请求) 获取以下[值：](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`adminConfirmedServicePrincipalCompromised`、 `adminDismissedAllRiskForServicePrincipal`。|
|riskEventType|字符串|检测到的风险事件的类型。 可能的值是：、`investigationsThreatIntelligence`、`generic`、`adminConfirmedServicePrincipalCompromised`、`suspiciousSignins`、`leakedCredentials``unknownFutureValue`。 支持 `$filter`（`eq`）。|
|riskLevel|riskLevel|检测到的风险级别。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden`。 可能的值包括 `low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|检测到的风险服务主体或登录活动的状态。 可能的值包括 `none`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。|
|servicePrincipalDisplayName|String|    服务主体的显示名称。|
|servicePrincipalId|String|服务主体的唯一标识符。 支持 `$filter`（`eq`）。|
|source|字符串|风险检测的来源。 例如，`identityProtection`。|
|tokenIssuerType|tokenIssuerType|指示检测到的登录风险的令牌颁发者类型。 可能的值是：、`AzureAD``UnknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipalRiskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalRiskDetection",
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
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String",
  "keyIds": [
    "String"
  ],
  "additionalInfo": "String"
}
```

