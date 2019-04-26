---
title: riskUserActivity 资源类型
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1685c58697f9de52e209d508c1ec104b9c044e8d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343561"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="8c0ef-102">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c0ef-102">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="8c0ef-103">属性</span><span class="sxs-lookup"><span data-stu-id="8c0ef-103">Properties</span></span>

| <span data-ttu-id="8c0ef-104">属性</span><span class="sxs-lookup"><span data-stu-id="8c0ef-104">Property</span></span>       | <span data-ttu-id="8c0ef-105">类型</span><span class="sxs-lookup"><span data-stu-id="8c0ef-105">Type</span></span>    |<span data-ttu-id="8c0ef-106">说明</span><span class="sxs-lookup"><span data-stu-id="8c0ef-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8c0ef-107">eventTypes</span><span class="sxs-lookup"><span data-stu-id="8c0ef-107">eventTypes</span></span> | <span data-ttu-id="8c0ef-108">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="8c0ef-108">riskEventType collection</span></span> |<span data-ttu-id="8c0ef-109">可能的值是 unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、leakedCredentials、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、mcasImpossibleTravel、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="8c0ef-109">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="8c0ef-110">介绍</span><span class="sxs-lookup"><span data-stu-id="8c0ef-110">detail</span></span>     | <span data-ttu-id="8c0ef-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8c0ef-111">riskDetail</span></span>  | <span data-ttu-id="8c0ef-112">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="8c0ef-112">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="8c0ef-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c0ef-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": ["String"],
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
