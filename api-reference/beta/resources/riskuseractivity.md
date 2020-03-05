---
title: riskUserActivity 资源类型
description: author
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1601f34b7d54a2c5304f3b20b04b8cb4c69c6323
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521066"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="a9458-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9458-103">riskUserActivity resource type</span></span>

<span data-ttu-id="a9458-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a9458-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="a9458-105">属性</span><span class="sxs-lookup"><span data-stu-id="a9458-105">Properties</span></span>

| <span data-ttu-id="a9458-106">属性</span><span class="sxs-lookup"><span data-stu-id="a9458-106">Property</span></span>       | <span data-ttu-id="a9458-107">类型</span><span class="sxs-lookup"><span data-stu-id="a9458-107">Type</span></span>    |<span data-ttu-id="a9458-108">说明</span><span class="sxs-lookup"><span data-stu-id="a9458-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9458-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="a9458-109">eventTypes</span></span> | <span data-ttu-id="a9458-110">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="a9458-110">riskEventType collection</span></span> |<span data-ttu-id="a9458-111">可能的值是 unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、leakedCredentials、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、mcasImpossibleTravel、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="a9458-111">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="a9458-112">介绍</span><span class="sxs-lookup"><span data-stu-id="a9458-112">detail</span></span>     | <span data-ttu-id="a9458-113">riskDetail</span><span class="sxs-lookup"><span data-stu-id="a9458-113">riskDetail</span></span>  | <span data-ttu-id="a9458-114">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="a9458-114">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a9458-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9458-115">JSON representation</span></span>

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
