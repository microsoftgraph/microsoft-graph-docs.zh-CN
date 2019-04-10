---
title: riskUserActivity 资源类型
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 258cd61b55d0ac8d19f83682fe34d53cc4b233b0
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2019
ms.locfileid: "31688496"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="5b268-102">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b268-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="5b268-103">属性</span><span class="sxs-lookup"><span data-stu-id="5b268-103">Properties</span></span>

| <span data-ttu-id="5b268-104">属性</span><span class="sxs-lookup"><span data-stu-id="5b268-104">Property</span></span>       | <span data-ttu-id="5b268-105">类型</span><span class="sxs-lookup"><span data-stu-id="5b268-105">Type</span></span>    |<span data-ttu-id="5b268-106">描述</span><span class="sxs-lookup"><span data-stu-id="5b268-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b268-107">eventTypes</span><span class="sxs-lookup"><span data-stu-id="5b268-107">eventTypes</span></span> | <span data-ttu-id="5b268-108">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="5b268-108">riskEventType collection</span></span> |<span data-ttu-id="5b268-109">可能的值是 unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、leakedCredentials、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、mcasImpossibleTravel、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="5b268-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="5b268-110">介绍</span><span class="sxs-lookup"><span data-stu-id="5b268-110">detail</span></span>     | <span data-ttu-id="5b268-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5b268-111">riskDetail</span></span>  | <span data-ttu-id="5b268-112">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="5b268-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5b268-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b268-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": [{"@odata.type":"microsoft.graph.riskEventType"}],
    "detail": "string"
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
