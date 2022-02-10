---
title: riskServicePrincipalActivity 资源类型
description: 表示由 Identity Protection 确定Azure AD服务主体Azure AD活动。
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d73f77adbc44833a489270b64e51006eaab49896
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519978"
---
# <a name="riskserviceprincipalactivity-resource-type"></a>riskServicePrincipalActivity 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
表示由 Identity Protection 确定Azure AD服务主体Azure AD活动。 

## <a name="properties"></a>属性

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|riskEventType|String|检测到的风险事件的类型。 可能的值是：、`unlikelyTravel``maliciousIPAddress``unfamiliarFeatures``anonymizedIPAddress`、、`malwareInfectedIPAddress`、`suspiciousIPAddress`、、 。 `leakedCredentials``investigationsThreatIntelligence``generic``adminConfirmedUserCompromised``mcasImpossibleTravel``mcasSuspiciousInboxManipulationRules``investigationsThreatIntelligenceSigninLinked``maliciousIPAddressValidCredentialsBlockedIP``unknownFutureValue`|
| detail     | riskDetail  | 检测到的风险的详细信息。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden`。 <br/>可能的值是：、`none``adminGeneratedTemporaryPassword``userPerformedSecuredPasswordReset``userPerformedSecuredPasswordChange`、、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、 。 `adminConfirmedSigninCompromised``hidden``adminConfirmedUserCompromised``unknownFutureValue``adminConfirmedServicePrincipalCompromised``adminDismissedAllRiskForServicePrincipal` 请注意，必须使用此可`Prefer: include-unknown-enum-members`变化枚举 (请求) 获取以下[值：](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`adminConfirmedServicePrincipalCompromised`、 `adminDismissedAllRiskForServicePrincipal`。|

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskServicePrincipalActivity"
}-->
```json
{
    "riskEventTypes": ["String"],
    "detail": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "",
  "tocPath": "",
  "suppressions": []
}
-->

