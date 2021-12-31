---
title: authenticationRequirementPolicy 资源类型
description: Azure AD要求用户在访问资源之前通过 MFA 检查。 如果需要 MFA 检查，则此资源标识需要 MFA 的策略。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 287a946321e72bb2ff5002c0ed21ad0d1267b313
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647202"
---
# <a name="authenticationrequirementpolicy-resource-type"></a>authenticationRequirementPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD要求用户在访问资源之前通过 MFA 检查。 如果需要 MFA 检查，则此资源标识需要 MFA 的策略。 


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|detail|String|提供有关 requirementProvider 中标识的功能的其他详细信息。|
|requirementProvider|requirementProvider|标识此Azure AD要求 MFA 的功能。 可取值为：`user`、`request`、`servicePrincipal`、`v1ConditionalAccess`、`multiConditionalAccess`、`tenantSessionRiskPolicy`、`accountCompromisePolicies`、`v1ConditionalAccessDependency`、`v1ConditionalAccessPolicyIdRequested`、`mfaRegistrationRequiredByIdentityProtectionPolicy`、`baselineProtection`、`mfaRegistrationRequiredByBaselineProtection`、`mfaRegistrationRequiredByMultiConditionalAccess`、`enforcedForCspAdmins`、`securityDefaults`、`mfaRegistrationRequiredBySecurityDefaults`、`proofUpCodeRequest`、`crossTenantOutboundRule`、`gpsLocationCondition`、`riskBasedPolicy`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationRequirementPolicy",
  "requirementProvider": "String",
  "detail": "String"
}
```
