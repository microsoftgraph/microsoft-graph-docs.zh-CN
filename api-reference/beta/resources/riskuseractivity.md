---
title: riskUserActivity 资源类型
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 258cd61b55d0ac8d19f83682fe34d53cc4b233b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563013"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="fb4bc-102">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb4bc-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="fb4bc-103">属性</span><span class="sxs-lookup"><span data-stu-id="fb4bc-103">Properties</span></span>

| <span data-ttu-id="fb4bc-104">属性</span><span class="sxs-lookup"><span data-stu-id="fb4bc-104">Property</span></span>       | <span data-ttu-id="fb4bc-105">类型</span><span class="sxs-lookup"><span data-stu-id="fb4bc-105">Type</span></span>    |<span data-ttu-id="fb4bc-106">说明</span><span class="sxs-lookup"><span data-stu-id="fb4bc-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fb4bc-107">eventTypes</span><span class="sxs-lookup"><span data-stu-id="fb4bc-107">eventTypes</span></span> | <span data-ttu-id="fb4bc-108">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="fb4bc-108">riskEventType collection</span></span> |<span data-ttu-id="fb4bc-109">可能的值是 unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、leakedCredentials、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、mcasImpossibleTravel、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="fb4bc-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="fb4bc-110">介绍</span><span class="sxs-lookup"><span data-stu-id="fb4bc-110">detail</span></span>     | <span data-ttu-id="fb4bc-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="fb4bc-111">riskDetail</span></span>  | <span data-ttu-id="fb4bc-112">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="fb4bc-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="fb4bc-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb4bc-113">JSON representation</span></span>

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
